# Python CLI Template Knowledge

## Project Overview

A minimal Python CLI application template with modern Python features, type hints, and best practices built in. Uses Hatch for packaging.

## Technology Stack

- **Python 3.10+** — Runtime
- **Hatch** — Build system and environment management
- **Black** — Code formatting (88-char line length)
- **MyPy** — Strict static type checking
- **pytest** — Testing framework

## Project Structure

```
cli/
├── __init__.py       # Package init
└── __main__.py       # Entry point (run with python -m cli)

pyproject.toml        # Project configuration
```

> **Note:** Create a `tests/` directory to add unit tests.

## Key Commands

| Command | Description |
|---------|-------------|
| `python -m cli` | Run the CLI application |
| `pytest` | Run the test suite |
| `black .` | Format code with Black |
| `mypy cli` | Type check with MyPy |

## Building for Distribution

```bash
pip install build
python -m build
pip install dist/*.whl
```

## Verifying Changes

After every change, run:

```bash
pytest && black --check . && mypy cli
```

This will check for:
- Test failures (pytest — requires `tests/` directory)
- Formatting issues (Black)
- Type errors (MyPy strict mode)

## Code Quality Standards

- **Black** — 88-character line length, Python 3.10+ target
- **MyPy** — strict mode, no untyped defs
- **Type hints** — Required for all function signatures

## Dependencies

Install with:
```bash
pip install -e ".[dev]"
```

This includes: black, mypy, pytest, toml