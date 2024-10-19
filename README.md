# Adding a New Benchmark to DuckDB

## Introduction
This repository hosts all the necessary resources for the Advanced Data Systems ASSG2 ``"Adding a New Benchmark to DuckDB"``.

## Table of Contents
- [Introduction](#introduction)
- [Project Structure](#project-structure)
  - [Code](#code)
  - [Data](#data)
  - [Additional Folders](#additional-folders)
- [Installation](#installation)
- [Usage](#usage)

## Project Structure

### Code
- `main.ipynb`: Main Jupyter Notebook where all the analyses are performed.

### Data
Located in the **"data"** folder:
- Directory containing the .tbl files for each SF, however, due to the size of .tbl files they are not pushed to GitHub.
- This folder is supposed to have three folders inside of it (sf1, sf5, sf10) each containing five .tbl files generated via the dbgen provided in the ASSG (to be able to run the whole notebook the files need to be generated by your side).

### Additional Folders
- `"databases"`: Due to the size of the .db files pushing them to the repo was ignored, however, three distinct databases get generated when the notebook is run.
- `"images"`: Directory where images used in the report can be found.
- `"results"`: Directory where the query profiling informations of each query ran with specific scale factor and thread count are.


## Installation
Ensure Python 3.12.6 is installed (other versions might work as well, however this is the one I used) and then run:
- `pip install -r requirements.txt`

## Usage
To run the notebook and recreate results:
1. Run the whole `main.ipynb` notebook.