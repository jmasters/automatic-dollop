# automatic-dollop

Towards a better workflow.

## Development Helpers

* black: code formatter
* flake8: source code checker that uses `PyFlakes`, `pycodestyle`
* mypy: static type checking for annotations

# Local Setup
## For automatic checks with each commit

```bash
conda create --name auto-dollop python=3
conda install black flake8 mypy
pip install pre-commit
pre-commit install
```

## Local config

* .gitignore
* .pre-commit-config.yaml: To allow automatic running of `flake8`, `black`, `mypy` with each commit (local)
* pyproject.toml: configuration for `black` (local)
* setup.cfg: configuration for `flake8` and `mypy` (local)

## Manual Usage
```bash
black .
flake8
mypy .
```

# Github Config

* ci.yaml: Enables github to run the `flake8`, `black`, `mypy` checks as a second line of defense (not local)
