# spark

Overview

This repository contains basic examples of Spark SQL to help beginners learn how to process and query structured data using Apache Spark.

You'll find simple scripts and queries that demonstrate creating tables, running SQL queries, and working with DataFrames.

Features

Load data from CSV or JSON files.

Create temporary views and run SQL queries.

Perform basic operations like:

SELECT

FILTER

GROUP BY

JOIN

Learn how to use Spark SQL functions like COUNT, SUM, AVG.

Installation

Install Apache Spark (version 3.x recommended) and Java 8/11.

Install Python 3.x (for PySpark):

pip install pyspark


Clone the repository:

git clone https://github.com/yourusername/basic-spark-sql.git
cd basic-spark-sql

Usage
Run a PySpark Script
spark-submit scripts/basic_queries.py

Use Jupyter Notebook

Open the notebook in notebooks/ folder.

Run the cells to see Spark SQL in action.

Example Spark SQL Query
# Create a temporary view
df.createOrReplaceTempView("users")

# Run a SQL query
spark.sql("SELECT country, COUNT(*) as total_users FROM users GROUP BY country").show()

Folder Structure
├── data/              # Sample datasets
├── notebooks/         # Jupyter notebooks
├── scripts/           # PySpark scripts
├── README.md          # Project documentation
└── requirements.txt   # Python dependencies
