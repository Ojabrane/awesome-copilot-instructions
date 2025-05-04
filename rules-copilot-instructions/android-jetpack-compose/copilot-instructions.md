# Android Jetpack Compose Copilot Instructions

## Project Structure
- Use a flexible structure, adapting to the project's organization:
  - app/src/main/java/com/package/
    - data/repository, datasource, models
    - domain/usecases, models, repository
    - presentation/screens, components, theme, viewmodels
    - di, utils
  - app/src/main/res/values, drawable, mipmap
  - app/src/test, app/src/androidTest

## General Best Practices
- Adapt to existing architecture while maintaining clean code.
- Follow Material Design 3 guidelines.
- Use clean architecture: domain, data, presentation layers.
- Use Kotlin coroutines and Flow for async operations.
- Implement dependency injection with Hilt.
- Use unidirectional data flow (ViewModel, UI State).
- Use Compose navigation for screens.
- Implement state hoisting and composition.

## Performance Guidelines
- Minimize recomposition with proper keys.
- Use LazyColumn/LazyRow for lazy loading.
- Implement efficient image loading.
- Use proper state management to avoid unnecessary updates.
- Follow lifecycle awareness and memory management.
- Use background processing as needed.

## UI Guidelines
- Use remember and derivedStateOf appropriately.
- Optimize recomposition and Compose modifiers ordering.
- Follow composable function naming conventions.
- Use preview annotations and proper state management (MutableState).
- Handle errors and loading states.
- Use MaterialTheme for theming.
- Follow accessibility and animation best practices.

## Testing Guidelines
- Write unit tests for ViewModels and UseCases.
- Implement UI tests with Compose testing framework.
- Use fake repositories for tests.
- Ensure proper test coverage and use testing coroutine dispatchers.
