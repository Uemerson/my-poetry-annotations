
# About

My [poetry](https://python-poetry.org/) annotations.

# Annotations

List poetry settings:

```
$ poetry config --list
```

Set virtualenvs in project:

```
$ poetry config virtualenvs.in-project true
```

Init project, you can use `-n` to skip:
```
$ poetry init
```

Add dependencies to your package/project:
```
$ poetry add your_dependecy
```

Remove dependencies to your package/project:
```
$ poetry remove your_dependecy
```

The easiest way to activate the virtual environment is to create a new shell with poetry shell:

```
$ poetry shell
```

To deactivate the virtual environment and exit this new shell type `exit`

If you use a tool like pyenv to manage different Python versions, you can set the experimental virtualenvs.prefer-active-python option to true. Poetry will then try to find the current python of your shell.

For instance, if your project requires a newer Python than is available with your system, a standard workflow would be:

```
$ pyenv install 3.9.8
$ pyenv local 3.9.8  # Activate Python 3.9 for the current project
$ poetry install
```

To feeze only requirements

```
$ poetry export --without-hashes --format=requirements.txt > requirements.txt
```

To feeze only dev requirements

```
$ poetry export --only dev --without-hashes --format=requirements.txt > requirements_dev.txt
```
