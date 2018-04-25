# cookiecutter-reproducible-ngs

A cookiecutter template for reproducible research, tailored for use with next-generation sequencing projects

The template is loosely based on the project structure setup by
[drivendata](http://drivendata.github.io/cookiecutter-data-science/).

### Requirements to use the cookiecutter template:
-----------
 - Python 3.5 or 3.6
 - [Cookiecutter Python package](http://cookiecutter.readthedocs.org/en/latest/installation.html) >= 1.4.0: This can be installed with pip by or conda depending on how you manage your Python packages:

``` bash
$ pip install cookiecutter
```

or

``` bash
$ conda config --add channels conda-forge
$ conda install cookiecutter
```


### To start a new project, run:
------------

    cookiecutter https://github.com/percyfal/cookiecutter-reproducible-ngs


### The resulting directory structure
------------

The directory structure of your new project looks like this: 

```
project_name/                <- top-level project folder
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
    ├── snakemake            <- snakemake workflow files
    └── python_module        <- Python module directory, by default named by the project
```

### Installing development requirements
----------------------------------------

    pip install -r requirements.txt
