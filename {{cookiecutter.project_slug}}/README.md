# {{cookiecutter.project_name}}

{{ cookiecutter.description }}

## Developer

### Install poetry

    $ curl -sSL https://install.python-poetry.org | POETRY_VERSION=1.3.2 python3 -

### Install dependencies

    $ poetry install

### Init git and install pre-commit

    $ git init
    $ poetry run pre-commit install
    $ poetry run pre-commit run --all-files

