# Data Directory

This directory contains all data used in the project.

## Structure

- `raw/`: Original, immutable data dumps
- `processed/`: Cleaned and transformed data ready for analysis
- `external/`: Data from third-party sources

## Guidelines

1. **Never commit large data files to Git**
   - Use `.gitignore` to exclude data files
   - Consider using DVC (Data Version Control) for large datasets

2. **Raw Data**
   - Keep raw data immutable
   - Document the source and date of acquisition
   - Use scripts in `scripts/` to download or generate raw data

3. **Processed Data**
   - All processed data should be reproducible from raw data
   - Document the processing steps in notebooks or scripts

4. **External Data**
   - Include attribution and licensing information
   - Document the source URL and access date

## Naming Conventions

- Use descriptive names: `customer_transactions_2024.csv`
- Include dates in ISO format: `YYYY-MM-DD`
- Use underscores for spaces: `my_dataset.parquet`
