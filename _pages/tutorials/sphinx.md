# Sphinx

Sphinx is an automatic documentation generator for Python projects.

All of the following commands should be run from within your project environment.

## Install

```shell
pip install sphinx sphinx_rtd_theme numpydoc recommonmark
```

## Set up

Go to your project directory, where a subfolder `mypackage` contains the code. Create another subfolder next to it called `docs`, open a terminal in it and run:

```shell
sphinx-quickstart
```

Be sure to say 'yes' when asked if you should separate source and build.

In the `source/conf.py` file:

- Uncomment and change the path to the root directory, something along the lines of:

```python
import os
import sys
sys.path.insert(0, os.path.abspath('../..'))
```

- Change the theme:

```python
html_theme = "sphinx_rtd_theme"
```

- Add the necessary extensions:

```python
extensions = [
    'sphinx.ext.autodoc',
    'sphinx.ext.autosummary',
    'sphinx.ext.coverage',
    'sphinx.ext.napoleon',
    'sphinx.ext.todo',
    'sphinx.ext.viewcode',
    'numpydoc',
    'recommonmark',
]
```

If you don't want to add (some) external dependencies in your Sphinx environment, just mock them:

```python
autodoc_mock_imports = ["torch"]
```

## Generate documentation

For the first time, or when the structure of your modules changes, run the following command from the `docs` folder:

```shell
sphinx-apidoc -e -T -M -f -o source/_modules/ ../mypackage/
```

Add the following line to your `source/index.rst` toctree:

```rst
API reference <source/_modules/mypackage>
```

When you want to build the documentation in HTML, just run:

```shell
make html
```

The generated website can be accessed by opening `build/html/index.html`.
