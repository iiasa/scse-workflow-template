# Scenario Explorer Workflow Template
This is the template for setting up custom scenario processing workflows.

As it stands this template simply features one module `workflow.py` with a single function `main(df: pyam.IamDataFrame) -> pyam.IamDataFrame:`. Since this is a template this function simply takes a pyam IamDataFrame (details about the pyam and the IamDataFrame can be found [here](https://pyam-iamc.readthedocs.io/en/latest/data.html)) and returns it unmodified.

**Important**: Do not change the name of the module `workflow.py` or the function `main` inside as they are called like this by the Job Execution Service (details can be found [here](https://github.com/iiasa/ece/wiki/Setup-a-new-Scenario-Explorer-Instance#job-execution-service))
