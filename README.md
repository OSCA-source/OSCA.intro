# Introduction to the OSCA book

This repository contains a Bioconductor package to deploy the **Introduction** subbook of the **Orchestrating Single-Cell Analysis** book.
To build:

1. Install all relevant packages in the `DESCRIPTION`:

    ```r
    BiocManager::install(remotes::local_package_deps(dependencies=TRUE))
    ```

2. Then, run the usual **bookdown** invocation in `inst/book`, for example:

    ```r
    bookdown::render_book("index.Rmd")
    ```

3. Or, do `R CMD build` on the package itself to compile the book during the vignette build process.

To contribute reports, follow standard procedure: fork and PR.
