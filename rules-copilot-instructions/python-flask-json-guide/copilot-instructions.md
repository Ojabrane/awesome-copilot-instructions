# Python Flask JSON Guide Copilot Instructions

## Project-Specific Guidance
- This project relies on the custom Drawscape Factorio Python module.

## Example Usage
```python
from drawscape_factorio import create as createFactorio
from drawscape_factorio import importFUE5

with open('/path/to/exported-entities.json', 'r') as file:
    json_data = json.load(file)
    data = importFUE5(json_data)
    result = createFactorio(data, {
        'theme_name': 'default',
        'color_scheme': 'main',
        'show_layers': ['assets', 'belts', 'walls', 'rails', 'electrical', 'spaceship']
    })

with open(output_file_name, 'w') as f:
    f.write(result['svg_string'])
```

## General Guidelines
- Use the Drawscape Factorio module for processing and visualizing JSON data.
- Follow the provided code pattern for importing, processing, and exporting data.
- Ensure all file paths and options are set according to project requirements.
- Write clean, maintainable, and well-documented Python code.
