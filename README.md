# Format Fusion

**Format Fusion** is a CLI tool for converting various data formats: JSON, YAML, and images to Base64.

[![Python checks](https://github.com/Nottezz/format-fusion-cli/actions/workflows/python-check.yaml/badge.svg?branch=main)](https://github.com/Nottezz/format-fusion-cli/actions/workflows/python-check.yaml)
[![PyPI version](https://img.shields.io/pypi/v/cli-format-fusion)](https://pypi.org/project/cli-format-fusion/)

---

## Installation

```bash
pip install cli-format-fusion
```

---
## Available Commands

Format Fusion supports the following conversions:

| Conversion     | Command                        | Options                 |
| -------------- | ------------------------------ | ----------------------- |
| JSON → YAML    | `format-fusion yaml`           | `--reverse`, `--output` |
| YAML → JSON    | `format-fusion yaml --reverse` | `--output`              |
| Image → Base64 | `format-fusion image`          | `--output`              |


> All commands support the --output option to specify the output file path.
---
### Usage Examples

#### JSON → YAML
```bash
# Convert JSON to YAML
format-fusion yaml D:\response_api.json
```
Result: an `output.yaml` file will be created in the current directory.

---
#### YAML → JSON
```bash
# Convert YAML back to JSON
format-fusion yaml D:\response_api.yaml --reverse
```
Result: an `output.json` file will be created.

---
#### Specify Output Path
```
# Save the converted file to a specific location
format-fusion yaml D:\response_api.json --output D:\data.yaml
```
Result: the file will be saved to the specified path `D:\data.yaml`.

---
#### Image → Base64
```
# Convert an image to Base64 and save to a file
format-fusion image D:\screenshot.png --output D:\screenshot.txt
```

Result: a file `screenshot.txt` will be created containing the Base64-encoded content.

---
## Useful Resources

[Issue Tracker](https://github.com/Nottezz/format-fusion-cli/issues)
