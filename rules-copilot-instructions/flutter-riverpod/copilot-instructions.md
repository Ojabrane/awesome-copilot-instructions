# Flutter Riverpod Copilot Instructions

## Tech Stack
- AI Model: GPT-4
- Frontend: Flutter ^3.22.0
- State Management: Riverpod ^2.6.1
- BaaS: Firebase

## Project Structure & Naming
- Follow this directory structure for features:
  - lib/features/<feature>/data/models/
  - lib/features/<feature>/data/<feature>_repository.dart
  - lib/features/<feature>/presentation/screens/
  - lib/features/<feature>/presentation/controllers/
  - lib/features/<feature>/presentation/widgets/
  - lib/features/<feature>/domain/models/
  - lib/features/<feature>/domain/use_cases/
  - lib/features/<feature>/shared/models/
- Top-level:
  - lib/shared/providers/, lib/shared/widgets/, lib/shared/models/, lib/shared/services/
  - lib/models/, lib/providers/, lib/core/network/, lib/core/errors/, lib/core/di/
  - app.dart (root widget), main.dart (entry point)
- Naming:
  - Files: snake_case
  - Classes: PascalCase
  - Variables/Functions: camelCase

## Key Principles
- Feature isolation: keep feature code self-contained
- Separation of concerns: separate data, logic, and UI
- Single responsibility: one purpose per class/file
- DRY: avoid code duplication
- Prefer feature-specific placement

## AI Assistant Execution Process
- Summarize main tasks concisely
- Review tech stack and constraints before implementation
- Identify requirements, constraints, and potential challenges
- List and order execution steps
- Analyze for duplicate or similar functionality before coding
- Execute steps one by one, reporting progress
- Adhere to directory structure and naming conventions
- Verify results after each step, isolate and fix errors
- Record verification results and evaluate deliverables
- Confirm consistency with instructions and check for duplicates
- Report final results in the specified format
- Confirm unclear points before work, report important decisions, and propose solutions for unexpected problems
- Do not make changes not explicitly instructed
- UI/UX design changes are prohibited unless justified and approved
- Do not change tech stack versions without approval
