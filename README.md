# 🛒 SuperMarket Data Cleaning Pipeline

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.8%2B-blue?style=for-the-badge&logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white" alt="Pandas">
  <img src="https://img.shields.io/badge/Jupyter-F37626.svg?style=for-the-badge&logo=Jupyter&logoColor=white" alt="Jupyter">
  <img src="https://img.shields.io/badge/Data_Engineering-Pipeline-success?style=for-the-badge" alt="Data Engineering">
</p>

<!-- Project Banner Image -->
<p align="center">
  ![image alt](https://github.com/Abdelfattah011/SuperMarket_Data_cleaning/blob/d4dc8c9ffd645ad80aad63fa3fa0230cfb91531a/DATA%20PHASES.jpg)
</p>

## 📌 Project Overview

This repository features a robust, multi-step data preprocessing workflow built in Python. The project focuses on transforming raw retail transactional data from a SuperMarket into a structured, high-quality dataset. 

As a fundamental part of the Data Engineering lifecycle, this pipeline ensures data integrity, consistency, and readiness for downstream processes such as loading into a Data Warehouse, building ETL pipelines, or performing Business Intelligence (BI) analytics.

## 🗂️ Dataset Description

The project utilizes a raw dataset (`SuperMarket.csv`) containing historical sales records. The initial state of this data required extensive wrangling to handle inconsistencies, missing values, and sub-optimal formatting to meet professional data engineering standards.

## 🛠️ Step-by-Step Data Pipeline

The cleaning process is thoroughly documented in `Data Cleaning code.ipynb`. To track the transformation at every stage, the pipeline exports an intermediate `.csv` file after each logical step:

### Phase 1: Standardization & Quality Assurance
* **`1. Renamed Data.csv`**: Standardized column headers by replacing spaces with underscores and converting to lowercase for seamless SQL integration.
* **`2. Handle missing values.csv`**: Addressed null values through careful imputation or dropping invalid rows, ensuring zero data leakage.
* **`3. Remove duplicate rows.csv`**: Scanned the dataset for duplicated transactional records and removed them to prevent skewed aggregations.

### Phase 2: Data Optimization
* **`4. Remove unnecessary columns.csv`**: Dropped irrelevant features that do not contribute to business analysis, effectively reducing the dataset's memory footprint.
* **`5. Make sure all columns have correct data types.csv`**: Cast each feature to its correct native data type (e.g., converting date strings to `datetime64`).
* **`6. Sort the data where appropriate.csv`**: Ordered the dataset chronologically based on transaction dates to facilitate time-series tracking.

### Phase 3: Feature Engineering
* **`7. Create a new 3 columns Data.csv`**: Extracted granular insights by splitting existing data (e.g., decomposing a 'Date' column into separate 'Day', 'Month', and 'Year' features).
* **`8. Create a new column called [Name].csv`**: Generated calculated metrics crucial for business analysis, such as engineering a 'Total Revenue' column.

---

## ⚙️ Installation & Setup

Follow these simple steps to get a local copy up and running on your machine:

### 1️⃣ Clone the repository
> Grab a copy of the code to your local environment.

```bash
git clone https://github.com/Abdelfattah011/SuperMarket_Data_cleaning.git
 ```

### 2️⃣ Navigate to the project directory2️⃣ Navigate to the project directory
Move into the newly created project folder.

```bash
cd SuperMarket_Data_cleaning
 ```

### 3️⃣ Install the required dependencies
Ensure you have Python installed, then install the necessary data manipulation libraries.

```bash
pip install pandas numpy jupyter
 ```

## 🎯 Key Skills Demonstrated
This project highlights the following core Data Engineering competencies:

- 🧹 Data Wrangling & Cleaning: Handling missing values, duplicates, and strict data typing.

- ⚙️ Feature Engineering: Creating derived metrics (e.g., Total Revenue) and granular date splitting.

- 🏗️ Pipeline Modularity: Structuring the process into clear, reproducible, and trackable sequential steps.

- 📊 Exploratory Data Analysis (EDA): Preparing raw data for analytical readiness.

- 🐙 Version Control: Managing code and project structure efficiently via Git & GitHub.

👨‍💻 Developed by: Abdelfattah Ahmed Abdelfattah





