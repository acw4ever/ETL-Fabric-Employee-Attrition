# Data-Crunching
This project builds a Microsoft Fabric data pipeline to automate ingestion and transformation of HR data from reports received trough Outlook and a local HR system, cutting manual processing time and improving data quality for downstream reporting.
## Overview
Purpose: Build an automated, maintainable data pipeline in Microsoft Fabric to ingest two primary sources—email reports (Outlook) and local HR system extracts—and perform standardized transformations so downstream analytics and reports are delivered faster and with consistent quality. Primary benefit: reduce manual effort and end-to-end processing time while improving traceability and repeatability.

## Architecture
Insert or link to a diagram showing the ETL workflow (can be a PNG/JPG/Markdown diagram).

## Technologies Used
- Python (pandas, sqlalchemy)
- PostgreSQL
- Docker (optional)
- Airflow (optional)
- [Any other relevant tools]

## Pipeline Steps

### 1. Extract
Explain how data is collected.  
Example:  
Extracts raw data from `data/sales.csv`.

### 2. Transform
Describe cleaning, logic, and transformation steps.  
Example:  
- Removes duplicates  
- Fills missing values  
- Aggregates monthly sales  

### 3. Load
Explain where the transformed data goes.  
Example:  
Loads cleaned data into `sales_data` table in PostgreSQL.

## How to Run

1. Clone the repo:
    ```
    git clone https://github.com/yourusername/etl-sales-pipeline.git
    cd etl-sales-pipeline
    ```

2. Install dependencies:
    ```
    pip install -r requirements.txt
    ```

3. Set up database connection settings in `config.yaml` or environment variables.

4. Run the ETL script:
    ```
    python etl_pipeline.py
    ```

## Project Structure
```
etl-sales-pipeline/
├── data/
│   └── sales.csv
├── etl_pipeline.py
├── requirements.txt
├── config.yaml
├── tests/
│   └── test_transform.py
├── docs/
│   └── architecture.png
└── README.md
```

## Testing
Describe how to run tests:
```
pytest tests/
```

## License
[MIT License] or other as appropriate.

## Credits
Mention collaborators, data sources, and referenced projects.

## Contact
Email or LinkedIn for professional inquiries.
