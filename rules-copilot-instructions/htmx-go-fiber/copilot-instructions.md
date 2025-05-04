# HTMX + Go Fiber Copilot Instructions

## Folder Structure
- Use the following structure for Go Fiber + HTMX projects:
  - cmd/
    - main.go
  - internal/
    - handlers/
    - models/
    - templates/
  - static/
    - css/
    - js/
  - go.mod
  - go.sum

## Main Application (cmd/main.go)
- Implement logging with Fiber's Logger middleware.
- Follow Fiber's best practices for project structure.
- Use environment variables for configuration.

## Handlers (internal/handlers/)
- Use Fiber's App.Get/Post/etc for routing HTMX requests.
- Implement CSRF protection with Fiber middleware.
- Use Fiber's Context for HTMX-specific headers.
- Use Fiber's template engine for server-side rendering.

## General Best Practices (Go + Fiber)
- Use Fiber's HTML rendering for server-side templates.
- Implement Fiber's routing system for HTMX requests.
- Use Fiber's middleware for request processing.
- Use Fiber's JSON methods for API responses.
- Implement proper error handling with Fiber's error handling.
- Use Fiber's static file serving for assets.
