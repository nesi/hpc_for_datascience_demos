# HPC for Data Science - Demos

This repository contains various notebooks to demonstrate how to run data science
related tasks on NeSI's HPC platform.


## Installation

First, to be able to run the notebooks, you will need to have access to
JupyterLab on the HPC platform, either using the dedicated [JupyterLab module](https://support.nesi.org.nz/hc/en-gb/articles/360001093315-JupyterLab)
or logging in via [Jupyter on NeSI](https://support.nesi.org.nz/hc/en-gb/articles/360001555615-Jupyter-on-NeSI).

Once you are connected to a JupyterLab instance, open a new terminal, via the
Launcher or the File menu.

Then clone this repository:
```
git clone https://github.com/nesi/hpc_for_datascience_demos
```

And install all dependencies in a virtual environment to cleanly isolate this
project from others:
```
cd hpc_for_datascience_demos
touch requirements.txt
make venv_nesi
```
The last command will create a virtual environment in the `venv` folder,
register it as a new kernel named `hpc_for_datascience_demos` and ensure that
it uses the right [environment modules](https://support.nesi.org.nz/hc/en-gb/articles/360001113076-The-HPC-environment-).


## Demos

Make sure to select the `hpc_for_datascience_demos` kernel when running any of
the provided notebooks.

- The [hyperparameters search (basic)](notebooks/hyperparameters_search_basic.ipynb)
  [[html version](https://nesi.github.io/hpc_for_datascience_demos/notebooks/hyperparameters_search_basic.html)]
  notebook shows how to adapt a Scikit-Learn grid search to run in parallel on HPC.
- The [hyperparameters search (NZ RSE 2020)](notebooks/hyperparameters_search_nzrse.ipynb)
  [[html version](https://nesi.github.io/hpc_for_datascience_demos/notebooks/hyperparameters_search_nzrse.html)]
  notebook corresponds to the demo presented at [NZ RSE conference 2020](https://www.rseconference.nz/).
