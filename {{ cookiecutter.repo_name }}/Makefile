.PHONY: clean lint help

##############################
# Global variables
##############################

PROJECT_DIR := $(shell dirname $(realpath $(lastword $(MAKEFILE_LIST))))
PROJECT_NAME = {{ cookiecutter.repo_name }}

ifeq (,$(shell which conda))
HAS_CONDA=False
else
HAS_CONDA=True
endif

##############################
# Commands
##############################
clean: ## Delete compiled Python files and other stuff
	find . -type f -name "*.py[co]" -delete
	find . -type d -name "__pycache__" -delete


lint: ## Lint using flake8
	flake8 src

##############################
# Documentation
##############################
.DEFAULT_GOAL := help

# Taken from <http://marmelab.com/blog/2016/02/29/auto-documented-makefile.html>
help:
	@grep -E '^[a-zA-Z_-]+:.*?## .*$$' $(MAKEFILE_LIST) | sort | awk 'BEGIN {FS = ":.*?## "}; {printf "\033[36m%-30s\033[0m %s\n", $$1, $$2}'

