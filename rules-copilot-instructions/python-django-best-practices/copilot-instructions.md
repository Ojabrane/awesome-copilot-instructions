# Python Django Best Practices Copilot Instructions

## Key Principles
- Write clear, technical responses with precise Django examples.
- Use Django's built-in features and tools wherever possible.
- Prioritize readability and maintainability; follow Django's coding style guide (PEP 8).
- Use descriptive variable and function names; follow naming conventions (lowercase_with_underscores).
- Structure projects modularly using Django apps for reusability and separation of concerns.

## Django/Python Guidelines
- Use class-based views (CBVs) for complex views; function-based views (FBVs) for simple logic.
- Use Django ORM for database interactions; avoid raw SQL unless necessary.
- Use Django's built-in user model and authentication framework.
- Use form and model form classes for form handling and validation.
- Follow the MVT (Model-View-Template) pattern strictly.
- Use middleware for cross-cutting concerns (auth, logging, caching).

## Error Handling and Validation
- Handle errors at the view level; use Django's built-in error handling.
- Use Django's validation framework for forms and models.
- Use try-except for exceptions in business logic/views.
- Customize error pages (404, 500) for better UX.
- Use Django signals to decouple error handling/logging from business logic.

## Dependencies
- Django
- Django REST Framework (for APIs)
- Celery (background tasks)
- Redis (caching, task queues)
- PostgreSQL/MySQL (preferred production DBs)

## Django-Specific Guidelines
- Use templates for HTML, DRF serializers for JSON.
- Keep business logic in models/forms; keep views light.
- Use urls.py for clear, RESTful URL patterns.
- Apply Django security best practices (CSRF, SQL injection, XSS protection).
- Use Django's testing tools (unittest, pytest-django).
- Use caching framework for performance.
- Use middleware for common tasks (auth, logging, security).

## Performance Optimization
- Use select_related/prefetch_related for ORM queries.
- Use cache framework with Redis/Memcached.
- Implement DB indexing and query optimization.
- Use async views and Celery for I/O-bound/long-running tasks.
- Optimize static file handling (WhiteNoise/CDN).

## Key Conventions
1. Follow "Convention Over Configuration" to reduce boilerplate.
2. Prioritize security and performance at every stage.
3. Maintain clear, logical project structure for readability and maintainability.

Refer to Django documentation for best practices in views, models, forms, and security.
