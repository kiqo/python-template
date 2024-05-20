# TODO-my-project-Project

TODO Update description - this is currently just a template repository.
TODO find and replace all TODOs via `grep -r TODO .` .


## Setup

Install [pipx](https://pipx.pypa.io/stable/installation/) and [pyenv](https://github.com/pyenv/pyenv?tab=readme-ov-file#installation) and then run the following commands:

```bash
# Install python 3.12 with pyenv
pyenv install 3.12.3
pyenv local 3.12.3
# Verify that correct Python is used
python --version
# Install pre-commit
pipx install pre-commit
# Setup pre-commit for this repository
pre-commit install
# Install uv
pipx install uv
# Setup conda python-venv

# Create a virtual environment with uv and verify that the above Python version is used
uv venv
```

## Run linter, formatter & tests

```bash
# Run linting and formatter
pre-commit run --all-files
```

## Lock dependencies
```bash
uv pip compile pyproject.toml -o requirements.txt     # Read a pyproject.toml file.
```