# Capstone Project – Model Building

## Project Overview
This capstone project demonstrates the design and implementation of an end-to-end data pipeline and analytical data model. The goal of the project is to simulate a real-world data engineering workflow, including data collection, cleaning, enrichment, validation, loading, and visualization.

The project uses synthetic data to represent customer purchase activity and prepares it for analytical use.

---

## Dataset Description
The dataset was generated using Mockaroo and contains information related to customer purchases. The key fields include:

- CustomerID: Unique customer identifier
- Name: Customer name
- Age: Customer age
- Country: Customer country
- PurchaseAmount: Amount spent by the customer
- PurchaseDate: Date of purchase

The raw dataset is stored in the `data/raw` directory and all processed datasets are saved in the `data/cleaned` directory.

---

## Data Pipeline Overview
The data pipeline consists of the following steps:

1. **Data Collection**  
   Synthetic data is generated using Mockaroo and saved as a CSV file.

2. **Data Cleaning**  
   Duplicate records are removed, missing values are handled, and data types are standardized.

3. **Data Enrichment**  
   New features such as age groups and purchase categories are created to support analysis.

4. **Data Validation**  
   Validation rules are applied to ensure data quality, including valid age ranges and positive purchase amounts. Validation results are logged.

5. **Data Loading**  
   The final validated dataset is loaded into a SQLite database for analytical querying.

---

## Data Modeling
The project uses a simple analytical data model where the main table represents customer transactions. Customer attributes such as age and country are combined with transactional data such as purchase amount and purchase date.

This model supports analytical queries such as:
- Total sales by country
- Average purchase amount by age group
- Sales trends over time

An entity relationship diagram (ERD) is included in the `diagrams` folder.

---

## Tools and Technologies
- Python
- Pandas
- SQLite
- Mockaroo
- Draw.io
- Power BI / Tableau
- GitHub

---

## Project Structure
``# capstone-project
