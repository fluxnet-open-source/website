# Testing & CI/CD

Software testing is the process of evaluating and verifying your code. It is a way to ensure that your code is doing what you expect it to, preventing bugs, reducing development costs, and improving performance. This process is often done automatically to save time and effort. This is called continuous integration (CI) and continuous delivery/deployment (CD).

## Description

Everyone tests their code. The question is just how manual of a process it is. CI is the idea of automating that process to make your tests reproducible. Automatic testing saves time by putting up some time as you go along to write some tests for various behavior you know should be constant as you make changes, and then you don't have to spend nearly as much time testing your code when you make changes, you just run your tests. And if one of your tests fails, if they are good tests, it points to where in your code the problem is, so it is much faster to find the problem, saving you time. You gain confidence in your code and gain time back in multiple spots.

### What is CI/CD?

CI/CD stands for continuous integration and continuous delivery/deployment.

CI (continuous integration) means code changes are regularly **committed**, **pushed**, **tested**, **merged/integrated** into the project. Generally, differences are relatively small and constantly tested, which minimizes the risk of introducing unwanted behavior and bugs. 

CD (continuous delivery or deployment) means automatically releasing your changes/releases to wherever you release (CRAN, PyPI, conda, binaries on Github, etc.).

### Automatic Testing

There are a few types of automatic tests, but some of the most important are:

#### Unit tests

Unit tests are small tests that test a single unit of code. They usually test only 1 or 2 things, and they test single functions. They are the easiest to write as you write these functions (or even before to help guide the function writing). Writing them once you have a lot of code can often mean you have a lot of code garbled together and hard to separate into single units. They are convenient because if they fail, you know exactly in the code what went wrong (since each is responsible for only 1 or 2 things). They are quick to write, but you usually want a more significant number.

#### Integration tests

Integration tests combine several parts of your system and test that they work together (when integrated). They help test the plumbing, but it is harder to know exactly what went wrong if something fails than with a unit test. Suppose you already have a large amount of code that is harder to separate into units. In that case, it can be easy to write a couple of integration tests to get started to make sure everything keeps working as you work on things. You usually have fewer integration tests than unit tests.

#### End-to-end tests (E2E test)

E2E tests are the least used of the 3. An E2E test is where you try and simulate installing your code in a production (user) environment somehow and ensure it still works. This can be automated or manual. Often this is only necessary if you are finding out from users that your code is passing your other tests in development but isn't working on their machines, and your code is more hardware specific. 

## Resources

Every primary source control website (GitHub, GitLab, bitbucket, etc.) have some way to do automatic testing on their platform. This means you can do your tests locally before you commit and push, as well as set it up to do on every commit or merge. They also all let you set up a way to automatically deploy on their platform (usually on a tag or other release mechanism). 

### Guides

* [R Packages (2e) - 13 Testing basics](https://r-pkgs.org/testing-basics.html)
* [Using anaconda with GitHub actions](https://github.com/marketplace/actions/setup-miniconda)
* [CLEAN code tutorial playlist](https://youtube.com/playlist?list=PLmmYSbUCWJ4x1GO839azG_BBw8rkh-zOj)

### Language Resources

#### Python

* [Pytest](https://docs.pytest.org/): Pytest is a an test writing package in Python. You write tests of your code as a function that you expect to pass and then can run all tests locally at once or in a GitHub workflow automatically.
* [Unit test](https://docs.python.org/3/library/unittest.html): Unit Test is the other most popular test writing package in Python.
* [Coverage](https://coverage.readthedocs.io/) (code coverage): Coverage is a code coverage metric package. Coverage is a metric of how much your tests cover your code. So, 80% of your code's lines were run when you ran all of your tests, and you have 80% coverage. There is a bit more to it than that, but that is the basic idea.

#### R

* [Testthat](https://testthat.r-lib.org): Testthat is the most popular test writing package in R. Similar to Pytest or Unit Test in Python, you write your tests and then can run all tests locally at once or in a GitHub workflow automatically.
* [covr (code coverage)](https://covr.r-lib.org): Covr is a code coverage package similar to Python's Coverage library above.

#### Julia

* [Test.jl](https://docs.julialang.org/en/v1/stdlib/Test/): Test.jl is a test writing package similar to Pytest, Unit Test, and Testthat above but for Julia.
* [Coverage.jl](https://github.com/JuliaCI/Coverage.jl): A coverage package for Julia similar to Python’s coverage and R’s covr.
