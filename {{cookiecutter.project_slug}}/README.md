# {{cookiecutter.project_name}}

{{ cookiecutter.description }}

## Developer

### Install poetry

    curl -sSL https://install.python-poetry.org | POETRY_VERSION=1.3.2 python3 -

### Install dependencies

    poetry install

### I{% if cookiecutter.init_git != 'y' %}nit git and i{% endif %}nstall pre-commit
{% if cookiecutter.init_git != 'y' %}
    git init
    git add .
{%- endif %}
    poetry run pre-commit install
    poetry run pre-commit run --all-files

