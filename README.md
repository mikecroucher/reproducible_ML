# Reproducible data science

## Slides

The slides are in **presentation/index.html**. On your local macginem, Navigate to that folder and open index.html in a browser.  See the online version at 

## External resources

**GitHub Repos**

* [PCA_demo](https://github.com/mikecroucher/pca_demo) The PCA demonstration used to motivate sharing of environments
* [Bob's repo](https://github.com/mikecroucher/Bobs_code]) Repo created from the slide motivating the use of version control

**NAG Numerical Library**

* [NAG Library for Python](https://www.nag.co.uk/nag-library-python)- All MLI delegates can have a free, personal-use license for one-year

**Academic Papers**

* [The (black) art of runtime evaluation: Are we comparing algorithms or implementations?](https://link.springer.com/article/10.1007/s10115-016-1004-2) - Demonstrating that the difference between the best and worst implementations of ML algorithms can be more than **10,000 times**. Even when only considering mature frameworks

## Version Control - Learn git

* [Software Carpentry lesson on git](http://swcarpentry.github.io/git-novice/)
* [Download and install git](https://git-scm.com/)

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
