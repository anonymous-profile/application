# Data Migration
## Introduction
The code in this repository is used to migrate fund operation data from hundreds of Excel files into an alternative investment software suite called eFront. This source data is cleaned, transformed and output into an eFront Excel template so that it can be loaded into that software. This repository also contains code used to aggregate the data in various ways so that it can be analysed or sent to stakeholders (who would review/clean/categorise the data as required). 

Initially the requirements were simple and the results were required quickly. Over time the requirements have changed and become increasingly complex. As a result, the code is convoluted and long. It could be restructured into a more concise form, but this has not been done because we don't require this code to be maintained or reused. 

## Key Files
There are lots of different files in this repo. The most relevant files are:
- mig_functions.py: this contains the majority of the code. It contains functions that are used by the other files. There will be docstrings to explain what each function does. 
- investee_fund_ops.py: this file collates all files and calls the relevant functions to migrate data for what are known as 'investee' funds 
- managed_fund_ops.py: this file collates all files and calls the relevant functions to migrate data for what are known as 'investee' funds

