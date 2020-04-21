# Is Your Research Software Correct?

![NAG Logo](./nag_logo.png)

## Slides

The slides are in **presentation/index.html**. On your local machine, Navigate to that folder and open index.html in a browser.  See the online version at https://mikecroucher.github.io/reproducible_ML/

## External resources

**Care about your code**

....and those who write it

* [Make your code citable](https://guides.github.com/activities/citable-code/)
* [Hidden REF](https://hidden-ref.org/) - There's more to research than papers but the UK's official measure, The Research Excellence Framework (REF), doesn't reflect this.  The Hidden REF aims to change that! 
* [Research Software Engineers Associaton](https://rse.ac.uk/) - Supporting the people behind research software

**GitHub Repos from this presentation**

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

## Distribute your computational environment, not just the code

* [My Conda cheatsheet](./conda.md) - One way to do it in Python

### XKCD comics I used in the presentation

* [Time taken to automate](https://xkcd.com/1319/)
* [Python lets you fly](https://xkcd.com/353/)

### Note to self

The way you push the `presentation` folder to gh-pages to make the slide deck live is
```
git subtree push --prefix presentation origin gh-pages
```
