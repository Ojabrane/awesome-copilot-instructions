# Flutter Development Copilot Instructions

## Code Style and Structure
- Write concise, efficient, and maintainable code.
- Modularize widgets and functions into reusable components to avoid duplication.
- Use descriptive variable names (e.g., isLoading, hasError).

## Directory Structure (under /lib)
- /models/: Data models and type definitions
- /viewmodels/: State management and business logic
- /views/widgets/: Reusable widgets
- /views/screens/: Per-screen widgets
- /services/: Service classes for API calls and data access
- /utils/: Helper functions and constants

## Naming Conventions
- Use snake_case for files, directories, and packages.
- Use UpperCamelCase for class names, enums, typedefs, and type parameters.
- Use lowerCamelCase for variables, functions, and class members.

## Imports
- Import order: dart: libraries first, then third-party packages, then project files.
- Use snake_case for import prefixes.

## Dart Usage
- Use static typing and type inference for type safety.

## UI and Styling
- Use Material widgets.
- Apply consistent theming with ThemeData.

## Performance Optimization
- Prefer StatelessWidget when state is not required.
- Use const constructors for immutable widgets.

## State Management
- Use Riverpod for efficient state management.
- Manage state in the ViewModel and link to the View.

## Architecture
- Follow MVVM (Model-View-ViewModel) architecture.

## Key Rules
- Limit lines to 80 characters for readability.
- Use braces {} for all flow control structures.
- Use comments to aid understanding and maintenance.
- Use single quotes for strings consistently.
