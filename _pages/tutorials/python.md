---
permalink: /tutorials/python/
title: Python
sidebar:
  nav: "tutorials"
---

If you're looking for something you don't find here, go to [awesome Python](https://github.com/vinta/awesome-python).

## Getting started

### Installation

Python is best installed and used with a scientific package manager called Conda. A complete distribution is available at [Anaconda](https://www.anaconda.com/), but I recommend the smaller [Miniconda](https://docs.conda.io/en/latest/miniconda.html) for most users. A known drawback of Conda is that resolving environments and finding conflicts takes a long time. [Mamba](https://github.com/mamba-org/mamba) is a completely equivalent but much faster alternative, with the exact same syntax.

### Development environment

My advice is to use [VSCode](../tutorials/vscode.md) along with its [Python extension](https://code.visualstudio.com/docs/languages/python). However, some people prefer coding in notebooks, in which case you will need to use [Jupyter](https://jupyter.org/), either with the classic notebook interface or with the more modern Jupyterlab IDE. For beginner developers, [JupyterLab Desktop](https://github.com/jupyterlab/jupyterlab-desktop) may provide an accessible all-in-one experience.

### Reproducible code

To distribute a Python package you developed, please use [Poetry](https://github.com/python-poetry/poetry).

## Useful packages

### The standard library

- [cProfile and pstats](https://docs.python.org/3/library/profile.html): Measures the time spent by your code in each function
- [multiprocessing](https://docs.python.org/3/library/multiprocessing.html): Parallelize computations
- [doctest](https://docs.python.org/3/library/doctest.html): Insert tests in your docstrings
- [itertools](https://docs.python.org/3/library/itertools.html): Build efficient iterators

### Nice-to-have

- [Sphinx](http://www.sphinx-doc.org/en/master/): Automatic document generation from docstrings
- [Black](https://black.readthedocs.io/en/stable/): Python code formatter
- [line_profiler](https://github.com/rkern/line_profiler): Measure the time spent by your code in each line
- [tqdm](https://github.com/tqdm/tqdm): Progress bars for long-running loops

## Mathematics

### Data analysis

- [pandas](https://pandas.pydata.org): 2-dimensional dataframes with lots of built-in analysis utilities
- [matplotlib](https://matplotlib.org): Everything you need for plotting
- [tikzplotlib](https://github.com/nschloe/tikzplotlib): Save your plots as Tikz figures for LaTeX
- [seaborn](https://seaborn.pydata.org): Nice-looking statistical plots

### Scientific computing

- [NumPy and SciPy](https://docs.scipy.org/doc/): Linear algebra, numerical analysis, probability and much more
- [Numba](https://github.com/numba/numba): Speed up your loops!

### Statistics and machine learning

- [scikit-learn](https://scikit-learn.org/stable/): Beginner-friendly machine learning toolbox
- [Pytorch](https://pytorch.org/): A leading library for neural networks
- [StatsModels](https://www.statsmodels.org/stable/index.html): Toolbox for classical statistics and time series
- [Pyro](http://pyro.ai) & [PyMC](https://docs.pymc.io): Probabilistic programming
- [Jax](https://github.com/google/jax): Differentiable programming

### Operations research

- [NetworkX](https://networkx.github.io): Representing and exploring graphs
- [CVXPY](https://www.cvxpy.org): Solving convex optimization problems
- [OR Tools](https://developers.google.com/optimization/): Google's optimization solvers

## Misc

### Web development

- [Flask](http://flask.pocoo.org): Building websites with Python as backend

### Maps

- [Folium](https://python-visualization.github.io/folium/): Visualize and create maps with OpenStreetMap backgrounds
