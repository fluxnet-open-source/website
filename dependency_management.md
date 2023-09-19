# Dependency Management

All software requires a platform to run on. It also often depends on additional libraries that must be co-installed on the platform in order to run. Identifying and managing these dependencies ensures that software continues to work over time and allows others to install and use software developed by someone else.

## Resources

### General Documentation
* [Best practices for dependency management](https://cloud.google.com/blog/topics/developers-practitioners/best-practices-dependency-management) (Google)

### Docker
[Docker](https://www.docker.com/) images package together code and dependencies, providing a portable complete system to be able to run the code anywhere, so long as Docker is available. A Dockerfile provides the recipe for recreating a Docker image so that it can be re-created or updated easily. Dockerfiles can be used in conjunction with dependency lists produced by dependency management packages (see Language Resources below) to automatically identify, update, and install dependencies in docker images. Online image repositories such as [Dockerhub](https://hub.docker.com/) and [quay.io](https://quay.io/) allow sharing and versioning of Docker images. 

* [Docker tutorial for beginners](https://docker-curriculum.com/)

### Language Resources

#### Python
* [Conda](https://docs.conda.io/en/latest/): Conda is a popular environment manager in the python community, and it has the advantage of managing non-python dependencies in addition to python dependencies. For example, you can manage dependencies for a multi-language project that requires Python, R, and C libraries. Conda can include a specific Python version as part of the environment which is very useful when code is shared.
* [Pip](https://packaging.python.org/en/latest/tutorials/installing-packages/): pip is the standard package manager for python. Pip is the most widely used package manager for python projects. Pip only installs python packages. Pip can also be used within conda.  
* [Poetry](https://python-poetry.org/): Python packaging and dependency management, can install pip packages. Poetry automatically creates a virtual environment for your project and installs all of the dependencies in that environment. Uses a very good dependency resolver. Can publish your project to pypi. Provides a comprehensive set of features and is therefore good for larger projects. Poetry cannot include a specific Python version as part of the environment, but uses the system Python.

#### R
* [packrat](https://cran.r-project.org/web/packages/packrat/index.html) or [renv](https://cran.r-project.org/web/packages/renv/index.html): These packages automatically detect the R dependencies used by code and record the exact versions used during development. The resultant machine-readable dependency list can be used directly in Dockerfiles to install them in another environment.
  * [Blog description of renv](https://rstudio.github.io/renv/articles/renv.html)
