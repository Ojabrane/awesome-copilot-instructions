# Convex Copilot Instructions

## General Development
- Prioritize correct schema definition using the `v` validator.
- Refer to https://docs.convex.dev/database/types for available types.
- Be aware of system fields: `_id` and `_creationTime` are automatically generated.

## Schema Design
- Use built-in system fields and data types as documented.
- Use the `v` validator builder for defining schema types (see: https://docs.convex.dev/api/modules/values#v).
- Follow the example schema for structuring, index creation with `.index()`, and field validation.
- Do not manually add indices for `_id` and `_creationTime`—these are handled by Convex.
