## Environments - conda cheatsheet

Download miniconda at [https://docs.conda.io/en/latest/miniconda.html](https://docs.conda.io/en/latest/miniconda.html)

### Listing and using installed environments

* `conda env list` - List all environments on your machine
* `conda activate foo` - Activate the environment called `foo`
* `conda deactivate` - Deactivate the environment you are currently using

### Creating and deleting environments

* `conda create --name foo Python=3.6 scipy=1.9 jupyter` - Create an evironment called `foo` using Python 3.6, scipy 1.9 and the latest version of jupyter 
* `conda create --name bar --clone foo` - Create an enviroment called bar that's a clone of the foo environment
* `conda remove --name foo --all` - Removes the environment called foo

## Package management

* `conda install scipy` - Installs the latest version of scipy into the active environment
* `conda remove scipy` - Uninstalls scipy from the active environment

### Creating and using environment files

Environment files contain full descriptions of environments and can be shared to allow others to use the same environment as you.

* `conda env export > environment.yml` - Create `environment.yml` describing the currently active environment
* `conda env create -f environment.yml` - Create an environment from the description in environment.yml
