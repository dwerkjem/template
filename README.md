# Python Programming Lab Template

A prompt-driven [Copier](https://copier.readthedocs.io/) template for creating
small Python programming labs with `uv`, pytest, and Ruff.

## Use the template

Install Copier once:

```bash
uv tool install copier
```

Generate a new lab:

```bash
copier copy gh:dwerkjem/template ./lab7
```

Copier prompts for the project name, package name, author, course, lab number,
description, and Python version.

## Generated starter code

The generated project begins with only one placeholder function:

```python
def lab() -> bool:
    """Replace this placeholder with the lab implementation."""
    return True
```

And one passing test:

```python
def test_lab_passes() -> None:
    assert lab()
```

After generation:

```bash
cd lab7
uv sync --dev
uv run pytest
```
