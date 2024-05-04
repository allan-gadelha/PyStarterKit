# Python Project Template Essentials

This repository serves as a template for Python projects, providing a basic structure that helps you get started quickly. It includes essential components like testing setup, linting, formatting, and more.

## Features

- **Python Version Management**: Managed with Pyenv.
- **Dependency Management**: Managed with Poetry.
- **Code Formatting**: Code formatting is set up with Black.
- **Linting**: Linting is set up with Flake8.
- **Testing**: Unit tests are set up with Pytest.
- **Pre-commit Hooks**: Pre-commit hooks are set up with Pre-commit.

## Prerequisites

Before you can use this template, you need to have the following tools installed on your machine:

- Python: You can download it from the [official website](https://www.python.org/downloads/).
- Pyenv: You can install it using the instructions in the [Pyenv GitHub repository](https://github.com/pyenv/pyenv#installation).
- Poetry: You can install it using the instructions on the [Poetry website](https://python-poetry.org/docs/#installation).
- Pre-commit: You can install it using the instructions on the [Pre-commit website](https://pre-commit.com/#install).

Once you have these tools installed, you can follow the instructions in the "Getting Started" section to set up your project.

## Getting Started

Here are the steps to create a new project from this template:

1. Click on the "Use this template" button to create a new repository from this template.
2. Clone the new repository to your local machine.
3. Set the Python version for your project with Pyenv by running `pyenv local 3.x.x` (replace 3.x.x with your desired Python version).
4. Install the dependencies with Poetry by running `poetry install`.
5. Install the pre-commit hooks with `pre-commit install`.
6. Rename the project and adjust the settings to fit your needs.

## Usage

Here's how you can use the different features of this template:

- **Python Version Management**: You can set the Python version for your project with the command `pyenv local 3.x.x`.
- **Running Tests**: You can run tests using the command `pytest`.
- **Linting**: You can lint your code using the command `flake8`.
- **Formatting**: You can format your code using the command `black`.
- **Pre-commit Hooks**: Pre-commit will automatically check your code for formatting and linting errors before each commit.

Remember, to enter the Poetry shell, use the command `poetry shell`. This ensures that the correct Python environment and dependencies are used.

To use `black` and `flake8` within a `poetry` shell, first activate the shell with `poetry shell`, then you can run `black` and `flake8` as usual.

## Managing Dependencies with Poetry

Poetry is a tool for dependency management and packaging in Python. It allows you to declare the libraries your project depends on and it will manage (install/update) them for you.

### Adding Dependencies

To add a new dependency to your project, use the `poetry add` command followed by the name of the package you want to add:

```bash
poetry add package-name
```

This will add the package to your pyproject.toml file and install it in your virtual environment.

### Updating Dependencies

To update a dependency to the latest version, use the poetry update command followed by the name of the package:

```bash
poetry update package-name
```

This will update the package in your virtual environment and update the poetry.lock file

### Running files

To run a Python file in your project, use the poetry run command followed by the python command and the path to the file:

```bash
poetry run python path/to/file.py
```

This will ensure that the file is run in the virtual environment with access to the dependencies specified in your pyproject.toml file.

Note: If you're using a `poetry shell` session, you can run Python scripts directly with the `python` command, without needing to prefix it with `poetry run`.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the terms of the MIT license.
