# Data Migration
## Introduction
The code in this repository was used to migrate fund operation data from hundreds of Excel files into an alternative investment software suite called eFront. This source data was cleaned, transformed and output into an eFront Excel template so that it can be loaded into that software. Overall, more than 25,000 fund operations were imported. 

![Data Transformation and Upload](https://user-images.githubusercontent.com/92265905/145561735-d5e8baf9-522f-4eee-87f5-cf0b48411f4b.jpg)

The fund operation amounts were often classified using a text field in the source Excel files. This repository also contains code used to aggregate the data in various ways so that it can be analysed or sent to stakeholders so that it could be reviewed, cleaned, classified and checked. 

Disclaimer: The code could be restructured into a more concise form! However, we did not require this code to be maintained or reused after the migration was complete, and as a result the emphasis was on speed rather than maintainability. 

## Key Files
There are lots of different files in this repo. The most relevant files are:
- mig_functions.py: this contains the majority of the code. It contains functions that are used by the other files. There will be docstrings to explain what each function does. 
- investee_fund_ops.py: this file collates all files and calls the relevant functions to migrate data for what are known as 'investee' funds 
- managed_fund_ops.py: this file collates all files and calls the relevant functions to migrate data for what are known as 'investee' funds

