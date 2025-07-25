# Bazel Copilot Instructions (Bzlmod)

## Bzlmod Adoption Guidelines
- Enable bzlmod by default (`--enable_bzlmod` in `.bazelrc`).
- Declare dependencies in `MODULE.bazel` instead of `WORKSPACE`.
- Prefer using `bazel_dep()` and `use_repo()` over manual `http_archive()` or `git_repository()`.
- Use the central Bazel registry or custom registries for third-party modules.
- Mirror dependencies internally for reproducibility.

## Project Structure & Targets
- Use clean Bazel package layout: every logical directory has a `BUILD.bazel`.
- Create small, focused targets (`*_library`, `*_test`, `*_binary`) that are easy to compose.
- Co-locate `BUILD.bazel` and source code for clarity and maintainability.

## Naming Conventions
- Follow label format: `//package/path:target_name`.
- Name targets descriptively: `web_server_lib`, `auth_service_test`, `tsconfig_build`.
- Avoid ambiguous names like `default`, `main`, or `all`.

## Dependency Management with Bzlmod
- Replace legacy `WORKSPACE` with `MODULE.bazel`:
  ```starlark
  bazel_dep(name = "rules_nodejs", version = "7.4.0")
  use_repo(name = "rules_nodejs")
  ```
- Declare Java, Python, or Go deps using official `rules_*` modules.
- Pin versions centrally; avoid version drift by isolating changes.
- Group reusable third-party deps in a `//third_party` directory, but manage actual fetching via bzlmod.

## Performance & Build Optimization
- Use `--disk_cache` and `--remote_cache` to improve incremental builds.
- Favor hermetic actions: all inputs must be declared, no filesystem/network access.
- Use `.bazelignore` to exclude non-code directories from the build graph.
- Use Bazel's `platforms` and `toolchains` to improve cross-platform reliability.

### TypeScript / Node.js
- Use `rules_js` and `rules_ts` with bzlmod.
- Prefer `ts_project()` and `js_binary()` over custom scripts.
- Use Bazel targets for `eslint`, `prettier`, and bundlers like `esbuild`.

### Java
- Use `rules_java` and `rules_jvm_external` with bzlmod.
- Favor modular targets: `java_library`, `java_binary`, `java_test`.
- Keep `main_class` explicit and structure code with clear `srcs`, `deps`, and `resources`.

### Python / Go
- Use `rules_python`, `rules_go` with bzlmod.
- For Python, declare interpreter versions and isolate virtual environments.
- For Go, leverage Bazel's module system to avoid `go.mod` duplication.

## Testing & Tooling
- Use native Bazel `*_test` rules.
- Define aliases like `//:all_tests` for CI and batch execution.
- Use `buildifier` and `buildozer` to maintain consistent BUILD file formatting.

## CI/CD Integration
- Add Bazel commands in CI workflows:
  - `bazel test //...`
  - `bazel build //frontend/...`
  - `bazel run //tools/lint:eslint`
- Use `bazel query` to inspect dependencies and minimize rebuilds.

## Maintainability Tips
- Use `buildifier` to auto-format and lint `BUILD.bazel` and `MODULE.bazel`.
- Prefer macros for repeated patterns across packages.
- Use `select()` for conditional logic (e.g., OS/platform-specific builds).
- Review `bazel mod deps` and `bazel mod graph` to debug module dependency issues.
