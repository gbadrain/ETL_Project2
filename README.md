# ETL Mini Project

## Overview
This project focuses on building an ETL (Extract, Transform, Load) pipeline using Python, Pandas, and tools like regular expressions or dictionary methods for data extraction and transformation. The transformed data is used to create CSV files, an Entity-Relationship Diagram (ERD), and a PostgreSQL database for further analysis and exploration.

## Project Goals
1. **Extract** data from the given Excel files.
2. **Transform** data using Python, ensuring it matches the required format.
3. **Load** the cleaned and transformed data into a PostgreSQL database.
4. Practice and enhance ETL-related skills while working collaboratively.

## Repository Content

### 1. Jupyter Notebooks
* **ETL_pipeline_starter.ipynb**:
   * Implements the extraction and transformation logic for the data.
   * Creates the DataFrames for categories, subcategories, campaigns, and contacts.
   * Generates the CSV files required for database creation.
* **Database_setup_starter.ipynb**:
   * Designs the ERD.
   * Creates and populates the PostgreSQL database tables based on the schema.

### 2. Data Files
* **crowdfunding.xlsx**:
   * Source data for categories, subcategories, and campaigns.
* **contacts.xlsx**:
   * Source data for contacts information.
* Generated CSV files:
   * `category.csv`
   * `subcategory.csv`
   * `campaign.csv`
   * `contacts.csv`

## Instructions

### Part 1: Extract and Transform Data
1. **Category and Subcategory DataFrames**:
   * Extract data from `crowdfunding.xlsx`.
   * Create DataFrames with the following columns:
      * `category_id` and `category`
      * `subcategory_id` and `subcategory`
   * Save as `category.csv` and `subcategory.csv`.

2. **Campaign DataFrame**:
   * Extract data from `crowdfunding.xlsx` and transform it.
   * Columns include:
      * `cf_id`, `contact_id`, `company_name`, `description`
      * `goal`, `pledged`, `outcome`, `backers_count`
      * `country`, `currency`, `launch_date`, `end_date`
      * `category_id`, `subcategory_id`
   * Save as `campaign.csv`.

3. **Contacts DataFrame**:
   * Extract data from `contacts.xlsx` using either:
      * Python dictionary methods
      * Regular expressions
   * Split `name` into `first_name` and `last_name`.
   * Save as `contacts.csv`.

### Part 2: Database Creation
1. Inspect and validate the four CSV files (`category.csv`, `subcategory.csv`, `campaign.csv`, `contacts.csv`).
2. Design the **Entity-Relationship Diagram (ERD)**:
   * Represent relationships between categories, subcategories, campaigns, and contacts.
   * Use tools like QuickDBD for visualization.
3. Create the **Database Schema**:
   * Include tables with the necessary primary and foreign keys.
   * Specify data types and constraints.
   * Save as `crowdfunding_db_schema.sql`.

### Part 3: Load Data into PostgreSQL
1. Create a PostgreSQL database named `crowdfunding_db`.
2. Execute the database schema to create the required tables.
3. Import the CSV files into the database tables.
4. Verify the data in each table using `SELECT` statements.

## Exploratory Analysis
Perform further analysis on the loaded data, such as:
1. Analyzing campaign goals and pledged amounts.
2. Identifying patterns in category and subcategory performance.
3. Exploring donor behavior and demographics.

## Results
The pipeline successfully extracts, transforms, and loads the data into a PostgreSQL database. This project demonstrates proficiency in Python, Pandas, and database management, while providing a solid foundation for further analysis.

## Technologies Used
* **Programming Languages**:
   * Python (Pandas, Regular Expressions)
* **Databases**:
   * PostgreSQL
* **Tools**:
   * QuickDBD (for ERD visualization)
   * Jupyter Notebook
   * Excel (for data inspection)

## Sources of Help
* Python Documentation
* Tutorials on Pandas and PostgreSQL
* QuickDBD Documentation
* Microsoft Copilot for problem-solving

## Contact
**Gurpreet Singh Badrain**
