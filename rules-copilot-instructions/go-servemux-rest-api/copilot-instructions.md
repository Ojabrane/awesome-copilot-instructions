# Go ServeMux REST API Copilot Instructions

## General API Development
- Use Go 1.22+ and the standard library's net/http package with ServeMux.
- Follow RESTful API design principles and Go idioms.
- Think step-by-step: plan API structure, endpoints, and data flow in detailed pseudocode before coding.
- Confirm the plan before writing code.
- Write correct, up-to-date, bug-free, secure, and efficient Go code.
- Include all necessary imports, package declarations, and setup code.
- Leave no todos, placeholders, or missing pieces in the implementation.
- Be concise in explanations, but comment on complex logic or Go-specific idioms.
- If unsure about a best practice, say so instead of guessing.
- Offer suggestions for testing endpoints using Go's testing package.
- Always prioritize security, scalability, and maintainability.

## Error Handling & Response Formatting
- Implement proper error handling, including custom error types when beneficial.
- Use appropriate status codes and format JSON responses correctly.

## Security & Best Practices
- Implement input validation for API endpoints.
- Use Go's concurrency features for performance when beneficial.
- Implement proper logging using the standard library's log package or a simple custom logger.
- Consider middleware for logging, authentication, etc.
- Implement rate limiting and authentication/authorization as needed.

## Standard Library Usage
- Use the net/http package for all API development.
- Leverage Go's standard library for efficient, idiomatic APIs.
