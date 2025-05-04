# HTMX + Flask Copilot Instructions

## Folder Structure
- Use the following structure for Flask projects:
  - app/
    - templates/
    - static/
      - css/
      - js/
    - models/
    - routes/
    - __init__.py
  - config.py
  - run.py

## Best Practices
- Use Flask's render_template for server-side rendering with HTMX attributes.
- Implement Flask-WTF for form handling and CSRF protection.
- Use Flask's url_for for generating URLs.
- Use Flask's jsonify for JSON responses.
- Implement Flask-SQLAlchemy for database operations.
- Utilize Flask's Blueprint for modular applications.
- Use Flask-Migrate for database migrations.
- Utilize Flask's request object for handling HTMX requests.
- Implement proper error handling and logging.
- Follow Flask's application factory pattern.
- Use environment variables for configuration.
