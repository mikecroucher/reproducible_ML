# Is Your Research Software Correct?

![NAG Logo](./nag_logo.png)

## Slides

The slides are in **presentation/index.html**. On your local machine, Navigate to that folder and open index.html in a browser.  See the online version at https://mikecroucher.github.io/reproducible_ML/

## External resources

**GitHub Repos**

* [PCA_demo](https://github.com/mikecroucher/pca_demo) The PCA demonstration used to motivate sharing of environments
* [Bob's repo](https://github.com/mikecroucher/Bobs_code) Repo created from the slide motivating the use of version control

**NAG Numerical Library**

* [NAG Library for Python](https://www.nag.co.uk/nag-library-python)

**Academic Papers**

* [The (black) art of runtime evaluation: Are we comparing algorithms or implementations?](https://link.springer.com/article/10.1007/s10115-016-1004-2) - Demonstrating that the difference between the best and worst implementations of ML algorithms can be more than **10,000 times**. Even when only considering mature frameworks
* [Good enough practices in scientific computing](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1005510)

## Version Control - Learn git

* [XKCD comic discusses git](https://explainxkcd.com/wiki/index.php/1597:_Git)
* [Software Carpentry lesson on git](http://swcarpentry.github.io/git-novice/)
* [Download and install git](https://git-scm.com/)
* [GitLab](https://about.gitlab.com/) - GitLab. If you need to host your own in-house replacement for GitHub.
* [Oh Shit! Git](https://ohshitgit.com/) - Hardly anyone knows how to use all of git.  What we do is use the same few commands and google our way out of trouble when things go wrong.  This site covers many cases that you'll run into in practice

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

### XKCD comics I used in the presentation

* [Time taken to automate](https://xkcd.com/1319/)
* [Python lets you fly](https://xkcd.com/353/)

### Note to self

The way you push the `presentation` folder to gh-pages to make the slide deck live is
```
git subtree push --prefix presentation origin gh-pages
```
