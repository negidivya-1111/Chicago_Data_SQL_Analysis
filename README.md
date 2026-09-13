# Chicago Census, Crime & Schools SQL Analysis

A SQL-based data analysis project examining socioeconomic, crime, and public school data for the city of Chicago. Built as part of an IBM/Coursera SQL and Python course, this notebook loads three real-world Chicago datasets into a SQLite database and uses SQL queries to answer a series of analytical questions.

## Datasets

The analysis uses three datasets sourced from the [City of Chicago Data Portal](https://data.cityofchicago.org/):

1. **Census Data** — selected socioeconomic indicators by community area, including per capita income, percent of households below the poverty line, and a computed hardship index.
2. **Chicago Public Schools Data** — school-level performance data, including safety scores and school type (elementary, middle, or high school).
3. **Chicago Crime Data** — a subset of recorded crime incidents, including crime type, description, location, and community area.

## What This Notebook Does

1. Loads the three datasets into a local SQLite database (`FinalDB.db`) using `pandas` and `sqlite3`.
2. Connects the Jupyter `ipython-sql` extension to the database for direct SQL querying via `%sql` / `%%sql` magic commands.
3. Answers a series of analytical questions using SQL, including:
   - Total number of recorded crimes
   - Community areas with per capita income below a given threshold
   - Crimes involving minors and kidnapping cases involving children
   - Types of crimes recorded at schools
   - Average safety score by school type
   - Community areas with the highest poverty rate
   - The most crime-prone community area
   - The community area with the highest hardship index (via subquery)

## Tools & Libraries

- Python
- pandas
- sqlite3
- ipython-sql (`%sql` / `%%sql` magic)
- Jupyter Notebook

## How to Run

1. Clone this repository.
2. Open `chicago_datasets_sql_analysis.ipynb` in Jupyter Notebook, JupyterLab, or Google Colab.
3. Run the cells in order from top to bottom — the notebook installs any required libraries automatically via `!pip install`.
