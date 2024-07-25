# Versioning

Software versioning tracks and communicates changes in software. It can also be applied to documents and data, among others.

## Description

Code is often a living thing. Changes are made in order to add new capabilities, fix errors or things that don’t work well, and stay up to date with changes in other software that the code needs to run (dependencies). Applying a standardized versioning scheme has many benefits, a few of which are:

* communicating that something has changed
* communicating how big of a change was made
* using a specific state (version) of the code for reproducibility of the output or successful operation in a particular environment
* tracing when or how a particular problem was introduced

_What is the difference between versioning and version control?_
This is a common and valid question, since tools like Git can be used for both.

* *Versioning* is the practice of designating different states of code. This tends to occur at a relatively coarse level, rolling up many changes and assigning a specific version identifier that provides information about the changes.
* *Version control* is applied at a very fine level. Each and every change is tracked character by character and line by line, and you can go back to previous states of the code and/or see the full history of changes.

There are many different versioning schemes in practice. Rather than appending a "_v2" to your file name, there are sophisticated yet simple versioning schemes along with free tools that do most of the work. See the resources below for links to descriptions of major schemes as well as free tools.

Two of the most common versioning techniques are Semantic versioning (a.k.a SemVer) and Calender Versioning (a.k.a CalVer). We generally recommend for most projects to use SemVer, but both versioning techniques are described bellow.


### Semantic Versioning
Semantic versioning is a versioning scheme that uses three numbers separated by periods: `Major.Minor.Patch`.
* The `Major` number is incremented when breaking changes are made.
* The `Minor` number is incremented when new features are added in a backwards-compatible manner.
* The `Patch` number is incremented when backwards-compatible bug fixes are made.
* Some notable projects that use SemVer include [R](https://cran.r-project.org/), [Python](https://www.python.org/), and [Docker](https://www.docker.com/).


### Calendar Versioning
Calendar versioning is a versioning scheme that uses the date of the release as the version number. For example, `2021.06` could represent a release made in June, 2021. You can then add additional releases years later such as `2021.06.1`, `2021.06.2`, etc.
This is the strategy that projects such as Ubuntu uses to version their releases. The advantage is that it is easy to know when the initial release was made, but the downside is that you lose information about the size of the patch and how big of a change it is.


### Integration with Version Control

There are many ways to integrate versioning with version control software like Git. Here are a few common practices:

* Tagging - You can tag specific commits in Git with a version number. This is a good way to keep track of what version of the code was used for a particular release or analysis.
* Version Control Systems - Many version control systems have built-in support for versioning. For example, Git has the concept of tags and branches, which can be used to keep track of different versions of the code.


## Resources

### Versioning schemes and practices
* Wikipedia page on [Software Versioning](https://en.wikipedia.org/wiki/Software_versioning)
* [Semantic versioning](https://semver.org/), a.k.a Semver - a commonly used versioning scheme that we recommend
* [FAIR Software](https://fair-software.nl/) - recommendations for open software

### Free tools
* [Git](https://git-scm.com/) and [Github](https://github.com/) - see our [Resource Guide](https://fluxnet-open-source.readthedocs.io/en/latest/resources-guide/git.html) and [Tutorial](https://fluxnet-open-source.readthedocs.io/en/latest/tutorials/git/index.html)!
* [Zenodo](https://zenodo.org/) - Host data and software alike, with versioning and creating DOIs for software and data
* [Github-Zenodo integration](https://github.com/zenodo/zenodo)
* [Bitbucket](https://bitbucket.org/product/) - Git-based software hosting platform
* [Apache Subversion](https://subversion.apache.org/) - Another flavor of version control software
