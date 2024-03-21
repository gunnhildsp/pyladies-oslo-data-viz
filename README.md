# data_viz_pyladies

An example project

## Development

Dependencies for the project are managed with poetry. To install all dependencies, run:

```shell
poetry install
```

It's recommended to install and use Pre-commit hooks to ensure code quality. Pre-commit can for
example be installed with pip or [pipx](https://pypa.github.io/pipx/installation/) (recommended):

It's recommended to install and use Pre-commit hooks to ensure code quality. Pre-commit is one of
the dev-dependencies of this project, so it was installed when you entered the command above, but
the hooks still need to be installed with the following command:

```shell
poetry run pre-commit install
```

After installation, Pre-commit will run a series of checks on each commit. These checks are defined
in `.pre-commit-config.yaml`. If Pre-commit finds an issue, it will usually (depending on the hook)
fix it automatically. You will have to add the changes to the staging area and commit again:

```shell
git add .
git commit
```

Pre-commit can also be run manually:

```shell
poetry run pre-commit run --all-files
```

It's a good idea to update the Pre-commit hooks regularly:

```shell
poetry run pre-commit autoupdate
```

Tests can be run with pytest:

```shell
poetry run pytest
```
