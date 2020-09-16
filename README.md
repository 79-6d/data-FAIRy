# Data-FAIRy

The FAIRy you summon to do your data laundry!

## Why do we create Data-FAIRy?

We have been cleaning a lot of biological datasets from various expeditions to make the data Findable Accesible Interoperable Reusable (FAIR). We found out that many researchers run into problem in how to manage their data and eventually wasting significant amount of time just to look for information within the sea of data. On the other hand, data managers also feel challenged cleaning out data that is not well structured and difficult to understand.

So we decided to compile our experiences into Data-FAIRy to help both researchers and data managers gain time by learning from each others.

## How to build this book locally 

This material has been written using [bookdown](https://github.com/rstudio/bookdown) and [R](https://cran.r-project.org/). The dependencies of this project is managed using [renv](https://rstudio.github.io/renv/).

To build the book locally, clone the [repo](https://github.com/79-6d/data-fairy.git).

If dependencies are not automatically installed by `renv` when you open `data-fairy.Rproj`, try the following command.

```{r}
renv::restore()
```

then run the following lines to build the book:

```{r}
library(here)
setwd(here())  # set working directory to project root directory 
bookdown::render_book("index.Rmd")
```

And view it with:

```{r}
browseURL("docs/index.html")
```

## License

[Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/)

