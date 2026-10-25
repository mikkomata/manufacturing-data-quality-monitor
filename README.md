# Manufacturing Data Quality Monitor

A hands-on Python and Pandas project demonstrating data-quality validation and production reporting using fictional Manufacturing Execution System (MES) batch records.

## Project Overview

Manufacturing data can contain missing timestamps, duplicate records, invalid batch durations, and incorrect quantities. These issues can affect production reporting and downstream analysis.

This project simulates a small manufacturing data pipeline that identifies data-quality issues, calculates batch durations, and produces production summaries by manufacturing line.

## Objectives

- Generate and analyze fictional MES batch records.
- Identify missing timestamps and duplicate batch IDs.
- Flag invalid time sequences and negative quantities.
- Calculate batch durations in minutes.
- Separate records requiring review from records passing the implemented validation checks.
- Summarize accepted production records by manufacturing line.
- Export validation reports and production summaries as CSV files.

## Technology Stack

- Python
- Pandas
- Jupyter Notebook
- CSV data files

## Pipeline Workflow

1. **Generate:** Create fictional MES batch records.
2. **Validate:** Check records against defined data-quality rules.
3. **Classify:** Label records as `VALID` or `REVIEW`, with review reasons.
4. **Calculate:** Calculate batch durations for accepted records.
5. **Summarize:** Aggregate batch counts, quantities, and average durations by production line.
6. **Export:** Save validation reports and trusted summaries as CSV files.

## Repository Structure

```text
manufacturing-data-quality-monitor/
├── 01_manufacturing_data_generation.ipynb
├── README.md
└── data/
    ├── mes_batch_records_raw.csv
    ├── data_quality_report.csv
    ├── record_level_validation_report.csv
    ├── batch_duration_analysis.csv
    ├── production_summary_by_line.csv
    ├── trusted_production_summary_by_line.csv
    └── validated_batch_records.csv
```

## Current Results

The current sample dataset contains 21 records. Under the implemented validation rules:

- 15 records pass the current checks.
- 6 records require review.
- Accepted records are summarized by production line.
- Validation and production outputs are exported for further analysis.

These results are specific to the fictional sample dataset and the current validation rules.

## Data Quality Considerations

A record marked `VALID` has passed the checks implemented in this prototype. It is not a guarantee that the record is correct in every business context.

Duplicate batch IDs are flagged for review rather than automatically deleted. The original raw dataset is preserved so that validation decisions remain traceable.

## Planned Enhancements

- Add automated tests and additional validation rules.
- Improve logging and error handling.
- Connect Python to SQL Server.
- Develop a repeatable ETL workflow.
- Add visualizations for manufacturing data-quality metrics.

## Disclaimer

This is an independent learning project using fictional manufacturing data. It does not contain actual company production records.

## Author

MES Engineer | Manufacturing Systems & Data | SQL Server | Power BI | Python
