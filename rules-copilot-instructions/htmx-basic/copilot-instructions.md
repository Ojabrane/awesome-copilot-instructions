# HTMX Basic Copilot Instructions

## Folder Structure
- Use the following structure for HTMX projects:
  - src/
    - templates/
    - static/
      - css/
      - js/
    - app.py

## General Best Practices
- Use hx-get for GET requests and hx-post for POST requests.
- Utilize hx-trigger for custom events.
- Use hx-swap to control content swapping.
- Implement hx-target to specify swap targets.
- Use hx-indicator for loading indicators.

## Additional Guidelines
- Use semantic HTML5 elements.
- Implement proper CSRF protection.
- Utilize HTMX extensions as needed.
- Use hx-boost for full page navigation.
- Implement proper error handling.
- Follow progressive enhancement principles.
- Use server-side templating (e.g., Jinja2, Handlebars).
