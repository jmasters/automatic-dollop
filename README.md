# automatic-dollop

Towards a better ML workflow.

## Development Requirements

```bash
pip install black flake8 mypy
```
* black: code formatter
* flake8: source code checker that uses `PyFlakes`, `pycodestyle`
* mypy: static type checking for annotations

# Local Setup

```bash
conda create --name auto-dollop python=3
conda install black flake8 mypy
pip install pre-commit
pre-commit install
```
