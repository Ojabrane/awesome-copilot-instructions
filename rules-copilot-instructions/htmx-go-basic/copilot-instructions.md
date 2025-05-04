# HTMX + Go Copilot Instructions

## Folder Structure
- Use the following structure for Go + HTMX projects:
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

## Best Practices (Go)
- Use html/template for server-side rendering.
- Implement http.HandlerFunc for HTMX requests.
- Use gorilla/mux for routing if needed.
- Use encoding/json for JSON responses.
- Implement proper error handling and logging.
- Use context for request cancellation and timeouts.
- Follow Go's idiomatic error handling.
- Implement graceful server shutdown.
- Use Go modules for dependency management.

## Best Practices (HTML)
- Use semantic HTML5 elements with HTMX attributes.
- Implement proper CSRF protection.
- Utilize HTMX extensions as needed.
- Use hx-boost for full page navigation.
