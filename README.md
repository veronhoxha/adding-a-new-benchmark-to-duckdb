# Adding a New Benchmark to DuckDB

## Introduction
This repository hosts all the necessary resources for the Advanced Data Systems Project 2 titled ``"Adding a New Benchmark to DuckDB"``.

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
Located in the **``"data"``** folder:

- This directory contains three subfolders: ``sf1``, ``sf5``, and ``sf10``, each with five ``.tbl`` files (``customer.tbl``, ``date.tbl``, ``lineorder.tbl``, ``part.tbl``, ``supplier.tbl``) generated using the ssb-dbgen provided in the project. Due to the size of the original ``.tbl`` files, only a sample from each table is available on GitHub for each scaling factor, intended only for testing purposes to enable code execution.
- To run the entire notebook and recreate the results in the report, you must generate the full ``.tbl`` files yourself using the ssb-dbgen tool for SF = 1, 5 and 10.

### Additional Folders
- `"databases"`: Due to the size of the .db files pushing them to the repo was ignored, however, three distinct databases get generated when the notebook is run.
- `"images"`: Directory where images used in the report can be found.
- `"results"`: Directory where the query profiling informations of each query ran with specific scale factor and thread count are.

## Installation
Prerequisites: Ensure Python 3.12.6 is installed on your machine. Other versions might work, but this project was developed with 3.12.6.

**1. Create and Activate a Virtual Environment**

Create a Virtual Environment in the root directory of this project by running the following commands:
  - For macOS/Linux:
      - ``python3 -m venv .venv``
      - ``source .venv/bin/activate``
  - For Windows:
      - ``python -m venv .venv``
      - ``.venv\Scripts\activate``

**2. Install Required Packages**

When the virtual environment is activated, install all necessary packages by running:
  - `pip install -r requirements.txt`

## Usage
To run the notebook and recreate results:
  - Run the whole `main.ipynb` notebook.