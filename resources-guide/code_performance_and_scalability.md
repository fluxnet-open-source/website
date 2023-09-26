# Code Performance and Scalability

How fast a piece of software runs and how many resources it consumes are typically irrelevant for small applications, such as computing eddy covariance fluxes for one day at one tower. But when performing computations for many towers in near-real-time or over many years or analyzing large remote-sensing datasets, the scalability of software becomes very important to whether the intended application is feasible given resource and time constraints. Optimizing software to maximize speed and minimize resource usage is aided by profiling tools that identify code sections that are responsible for the most time. Implementing good code practices and using packages or functions suited to the task are the means by which to improve scalability.

## Resources

### Language Resources - Code Profiling

#### Python
* [Good coding practices](https://powerfulpython.com/blog/scaling-python/)
* [Memory profiling](https://medium.com/@sonia_samipillai/performance-analysis-of-your-python-program-using-memory-profiler-fa9ea83fe3cd)

#### R
* Best practices for efficient R code [tutorial](https://csgillespie.github.io/efficientR/programming.html)
* Built-in profiling tools [tutorial](https://bookdown.org/rdpeng/rprogdatascience/profiling-r-code.html)
* [Profvis](http://rstudio.github.io/profvis/) package (both time and memory profiling)
  
### Language Resources - Big Data

#### Python
* [Introduction to scaling distributed python applications](https://powerfulpython.com/blog/scaling-python/)

#### R
* [Datacamp courses](https://www.datacamp.com/courses/scalable-data-processing-in-r)
