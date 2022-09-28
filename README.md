
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
