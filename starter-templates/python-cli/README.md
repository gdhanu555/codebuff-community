# Python CLI Template

A minimal Python CLI application template with modern Python features, type hints, and best practices built in.

## Clone this template

```bash
# Create a new project using this template
codebuff --create python-cli my-app
```

## Getting Started

### 1. Create and activate a virtual environment

```bash
python -m venv .venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate
```

### 2. Install dependencies

```bash
pip install -e ".[dev]"
```

### 3. Run the CLI

```bash
python -m cli
```

## Available Commands

| Command | Description |
|---------|-------------|
| `python -m cli` | Run the CLI application |
| `pytest` | Run the test suite |
| `black .` | Format code with Black |
| `mypy cli` | Type check with MyPy |

## Building for Distribution

```bash
# Install build tool
pip install build

# Build the package
python -m build

# Install the built wheel
pip install dist/*.whl
```

## Project Structure

```
my-app/
├── cli/              # Source code
│   ├── __init__.py
│   └── __main__.py   # Entry point
├── pyproject.toml    # Project configuration
└── README.md
```

> **Note:** Create a `tests/` directory to add unit tests.

## Code Quality

This template enforces:
- **Black** formatting (88-character line length)
- **MyPy** strict type checking
- **pytest** for testing

Run all checks (dependencies from dev install):
```bash
pytest && black --check . && mypy cli
```

## Learn More
- [Python Documentation](https://docs.python.org/3/)
- [Black Documentation](https://black.readthedocs.io/)
- [MyPy Documentation](https://mypy.readthedocs.io/)
- [pytest Documentation](https://docs.pytest.org/)
