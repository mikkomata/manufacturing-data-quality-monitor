
# Manufacturing Data Quality Monitor

## Overview

An independent Python and Pandas project that simulates
a manufacturing data pipeline using fictional MES batch
records.

The project identifies data-quality issues, calculates
batch durations, and generates production summaries by
manufacturing line.

## Objectives

- Identify missing production timestamps.
- Detect duplicate batch records.
- Flag invalid batch chronology.
- Identify negative production quantities.
- Calculate batch durations in minutes.
- Summarize production quantities and batch counts by line.
- Export validation reports and production summaries to CSV.

## Technologies

- Python
- Pandas
- Jupyter Notebook
- CSV

## Project Structure

- `01_manufacturing_data_generation.ipynb`
  - Dataset generation, validation, analysis, and exports.
- `data/`
  - Fictional source data and generated reports.

## Data Disclaimer

All records are fictional and created for educational
and portfolio purposes. No employer production data
is included.

## Current Status

Initial prototype completed. Further improvements
will include record-level validation, SQL Server
integration, and a repeatable data pipeline.
