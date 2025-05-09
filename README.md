![Run Tests](https://github.com/mahbodez/richtqdm/actions/workflows/python-package.yml/badge.svg)
[![PyPI version](https://badge.fury.io/py/richtqdm.svg)](https://badge.fury.io/py/richtqdm)

# richtqdm

A modern and visually appealing replacement for `tqdm`, powered by [Rich](https://github.com/Textualize/rich).  
It automatically adapts to Jupyter notebooks and terminals.

## Features

- Beautiful progress bars using Rich
- Jupyter support
- Custom units (like `it`, `steps`, `samples`)
- tqdm-like API

## Installation

```bash
pip install richtqdm
```

## Usage

```python
from richtqdm import RichTqdm

for i in RichTqdm(range(100), desc="Processing", unit="items"):
    ...
```

## Release

To publish a new version to PyPI and GitHub:

```bash
# Build distribution packages
python -m build

# Upload to PyPI using Twine
twine upload dist/*

# Create a Git tag and push
git tag v${PROJECT_VERSION}
git push origin main --tags
```

## License

MIT License. Developed by Mahbodez.

## Links
- [Repository](https://github.com/mahbodez/richtqdm)
- [Author Profile](https://github.com/mahbodez)
