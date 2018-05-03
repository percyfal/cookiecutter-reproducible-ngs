{{cookiecutter.project_name}}
==============================

{{cookiecutter.description}}

Project Organization
--------------------

```
{{cookiecutter.project_name}}/                <- top-level project folder
│
├── AUTHORS.md               <- list of authors
├── Dockerfile               <- docker template
├── LICENSE
├── Makefile                 <- makefile with project management rules like `make clean` or `make docs`
├── README.md                <- Top-level README
├── Snakefile                <- Snakemake workflow manager top-level file. The `all` target should collect 
│                               all relevant output files and generate the final results and reports
│
├── config                   <- configuration directory for Snakemake and other things
│
├── data
│   ├── external             <- data from third party sources
│   ├── interim              <- Intermediate data that can be safely deleted
│   ├── metadata             <- metadata describing raw data files
│   ├── processed            <- Final processed data used for analyses
│   └── raw                  <- The original immutable data dump to be treated as read-only.
│
├── docs                     <- A default Sphinx project. See sphinx-doc.org for details.
│
├── environment.yml          <- Conda environment file
│
├── logs                     <- Collection of log outputs, e.g. from cluster managers
│
├── notebooks                <- Jupyter, Rmarkdown and other notebooks.
│
├── opt                      <- for installation of add-on application software packages that are unavailable
│                               via package managers such as conda or pip
│                               (see File System Hierarchy standard, http://www.pathname.com/fhs/pub/fhs-2.3.html)
│
├── references               <- Literature, manuals and other references
│
├── reports                  <- Generated analyses and articles as html, pdf and more.
│   └── figures              <- Graphics for use in reports.
│
├── results                  <- Final results for sharing with collaborators, typically derived 
│                               or copied from data/processed
│
└── src                      <- Project source code
    ├── R                    <- R sources
    ├── scripts              <- shell scripts
    ├── snakemake            <- snakemake workflow files
    └── {{cookiecutter.python_module}}        <- Python module directory, by default named by the project
```

-------------

Project based on the [cookiecutter reproducible ngs project template](https://github.com/percyfal/cookiecutter-reproducible-ngs)

