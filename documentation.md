# Documentation

Documentation of your code and how to use it is a vital tool for software maintenance, re-usability, and getting your software used by more people. It can be the least fun part of writing code, but also the most important part of writing code. Through some simple tools that help with automating documentation, you can make the process of documenting your code easier and more enjoyable.

## Description 

When documenting your code, you want to document it both internally and externally. 

You want to document your code internally for developers through the use of comments, docstrings (function comments), and well named variables or functions so that future developers can more easily navigate the logic of the code (note, future developers may be you in 3 months after you forget why you wrote something a certain way).

You also ideally want to document your code externally in some way for users through a [documentation hosting page service](#where-to-publish-documentation-for-free) and ideally use some sort of [automatic documentation generating](#automatic-code-documentation) tool that makes documentation directly from your code (so your documentation stays in line with your code and does not get out of date as easily and is maybe supplemented with additional handcrafted documents).

Through these two methods, internal and external documentation, you open up your code to be more inevitable to be used by other people and to be contributed to by other developers.

## Resources

### General Documentation

#### Code comments, commenting best practices, docstrings

* [Guide to writing comments](https://stepsize.com/blog/the-engineers-guide-to-writing-code-comments)
* [Tips for not writing bad comments](https://stackoverflow.blog/2021/12/23/best-practices-for-writing-code-comments/) 
* [Python guide to documenting, but broadly aplicable](https://realpython.com/documenting-python-code/)

#### Github, Gitlab, and Bitbucket READMEs
    
* [A helpful tool for generating a README](https://readme.so/)

### Documentation Publishing

#### Automatic code documentation

* [Sphinx](https://docs.readthedocs.io/en/stable/intro/getting-started-with-sphinx.html): Sphinx is an automatic code documentation generator that generates documentation websites automatically from your code docstrings. It is widely used in Python, but can be used to make pages for a large variety of languages.
* [Roxygen](https://cran.r-project.org/web/packages/roxygen2/vignettes/roxygen2.html): Roxygen is an automatic code documentation generator for R projects that uses specially formatted R comments to build documentation directly from your source code.

#### Other documentation publishing tools

* [jupyterbooks](https://jupyterbook.org/en/stable/intro.html): Build documentation websites from Jupyter notebooks (executable code in Python, R, or Julia. Fun fact! The name jupyter actually comes from the combination of JUlia, PYTon and R) and markdown files.

#### Where to publish documentation for free

* [Read the Docs](https://readthedocs.org): A free documentation hosting service that can automatically build documentation from your code using Sphinx, MkDocs, or other tools.
* [MkDocs](https://www.mkdocs.org/): Similar to Read the Docs.
* [Github pages ](https://pages.github.com): Similar to Read the Docs and MkDocs, but hosted on Github and can be built from any static site generator, but doesn't support documentation versioning as easily.
* [Quarto](https://quarto.org/) (for python, julia, R and Observable JS): An open-source scientific and technical publishing system
* [Gitlab pages](https://docs.gitlab.com/ee/user/project/pages/): Similar to Github pages, but hosted on Gitlab.

### Language Resources

#### Python

* [Docstrings](https://realpython.com/documenting-python-code/#documenting-your-python-code-base-using-docstrings): docstrings are a special type of comment at the beginning of functions and classes that describe the function or class.
    * [Pandas docstring guide](https://pandas.pydata.org/docs/development/contributing_docstring.html): Another good docstring guide that also covers extra sections such as providing code examples (that can be doctested).
* [Python Doctest](https://docs.python.org/3/library/doctest.html): Doctest is a documentation and testing tool that lets you write automatic tests in your documentation, so that examples of your code being use show up in your documentation, and some of your tests are as close to your documentation as possible, ensuring your documentation doesn’t get out of date.

#### R

* [Writing R Documentation](https://rstudio.github.io/r-manuals/r-exts/Writing-R-documentation-files.html)
* [R Doctest](https://cran.r-project.org/web/packages/doctest/vignettes/doctest.html) See above for what doctest is.

### Julia

* [Julia Documentation and Writing Julia Documentation](https://docs.julialang.org/en/v1/manual/documentation/)
* [Julia Doctest](https://documenter.juliadocs.org/stable/man/doctests/index.html) See above for what doctest is. 
