Generate forms from configuration.

Requirements:

- Read document type configuration.
- Build fields dynamically.
- Build Zod schema dynamically.
- Connect schema to React Hook Form.
- Show inline validation.
- Support:
  - string
  - text
  - enum
  - array
  - boolean
  - date

Changing document type must regenerate:
- fields
- validation schema
- default values