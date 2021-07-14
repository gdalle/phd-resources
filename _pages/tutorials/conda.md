# Conda environments

## General setup

```shell
conda config --add channels conda-forge
conda config --set channel_priority strict 
```

## New environment

```shell
conda create -n MYENV python
```

Data science packages
```shell
conda install numpy scipy matplotlib seaborn pandas dask numba tqdm
```

Notebook packages
```shell
conda install nodejs jupyter jupyterlab jupyter_contrib_nbextensions ipykernel ipywidgets jupyter_nbextensions_configurator rise
```
