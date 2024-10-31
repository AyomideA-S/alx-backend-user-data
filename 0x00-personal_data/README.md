# 0x00-Personal_Data

## Description

A Python project that securely logs user data by redacting sensitive personal information. It connects to a MySQL database, retrieves user records, and ensures PII is masked in the logs.

## Installation

1. Clone the repository.
2. Install dependencies:

    ```bash
    pip install mysql-connector-python
    ```

3. Set environment variables:
    - `PERSONAL_DATA_DB_USERNAME`
    - `PERSONAL_DATA_DB_PASSWORD`
    - `PERSONAL_DATA_DB_HOST`
    - `PERSONAL_DATA_DB_NAME`

## Usage

Run the main script:

```bash
python filtered_logger.py
```
