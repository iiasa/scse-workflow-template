# Scenario Explorer Workflow Template

Copyright 2021 IIASA

[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)

# Overview

This is a template for project-specific scenario processing workflows.

## Workflow

The module `workflow.py` has a function `main(df: pyam.IamDataFrame) -> pyam.IamDataFrame:`.

Per default, this function takes an **IamDataFrame** and returns it without modifications.
[Read the docs](https://pyam-iamc.readthedocs.io) for more information
about the **pyam** package for scenario analysis and data visualization.

**Important**: Do not change the name of the module `workflow.py` or the function `main`
as they are called like this by the Job Execution Service.
Details can be found [here](https://github.com/iiasa/ece/wiki/Setup-a-new-Scenario-Explorer-Instance#job-execution-service).

## Project nomenclature

The folder `definitions` can contain the project nomenclature,
i.e., list of allowed variables and regions, for use in the validation workflow.
See the **nomenclature** package for more information
([link](https://github.com/iamconsortium/nomenclature)).