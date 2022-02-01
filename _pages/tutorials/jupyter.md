---
permalink: /tutorials/jupyter/
title: Jupyter
sidebar:
  nav: "tutorials"
---

# Jupyter

Jupyter is an environment for easy prototyping and display of Julia, Python and R code.

## Setup

### Conda installation

First we must create / configure the environment from which you will launch the notebooks (see the conda tutorial). Ideally, it should be the environment where your code runs, but it can be your base environment if you like, in which case you need to run the following command in the desired environment:

```shell
conda install nb_conda nb_conda_kernels
```

### List of available extensions

For Jupyter: https://jupyter-contrib-nbextensions.readthedocs.io/en/latest/index.html

For JupyterLab: https://jupyterlab.readthedocs.io/en/stable/user/extensions.html

### Making kernels visible

If you launch the notebook from a dedicated launcher environment, thanks to the `nb_conda_kernels` package, other Conda environments be seen by the launcher. But first, run these commands in each one of your other environments:

```shell
conda install ipykernel
python -m ipykernel install --user --name myenv --display-name "Python (myenvname)"
```

## SSH

With the following command, you can start a distant notebook on the server:

```shell
jupyter notebook --no-browser --port=9090
```

Which you can then access from your computer:

```shell
ssh -N -L localhost:8080:localhost:9090 server
```

Then go to http://localhost:8080/ in your favorite browser and enter the token you see in the distant shell.
