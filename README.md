IPL Data Analysis Using Apache Spark

Overview

This project leverages Apache Spark to process and analyze IPL cricket match data efficiently. Using PySpark, we perform data ingestion, transformation, and exploratory data analysis (EDA) to extract insights into player performances, match statistics, and team trends.

Technologies Used

Big Data Frameworks: Apache Spark (PySpark)

Data Storage: Amazon S3

Programming Language: Python

Data Processing: Spark SQL, DataFrames

Data Visualization: Matplotlib, Seaborn (if applicable)

Dataset

The dataset contains structured IPL match data in CSV format, including ball-by-ball details, match results, player performances, and team statistics. The data is loaded from an Amazon S3 bucket and processed using PySpark.

Project Structure

├── data/                        # Sample dataset (if included)
├── notebooks/                   # Jupyter Notebooks for analysis
│   ├── IPL_DATA_ANALYSIS_SPARK.ipynb
├── scripts/                     # Python scripts for Spark processing
│   ├── data_ingestion.py
│   ├── data_analysis.py
├── README.md                    # Project Documentation

Key Features & Contributions

Designed and implemented a big data pipeline for processing IPL match data.

Ingested structured CSV data from Amazon S3 and optimized it using Spark SQL.

Applied window functions for ranking players and aggregating match performances.

Optimized queries using predicate pushdown and column pruning for efficiency.

Performed exploratory data analysis (EDA) to uncover insights into team performance, batting trends, and bowling statistics.

Installation & Setup

Clone the Repository

git clone <repository_url>
cd ipl-data-analysis-spark

Set Up a Virtual Environment (Optional)

python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

Install Dependencies

pip install -r requirements.txt

Run Spark Locally (Ensure Spark is installed)

pyspark

Running the Analysis

Execute the Jupyter notebook:

jupyter notebook notebooks/IPL_DATA_ANALYSIS_SPARK.ipynb

Or, run Python scripts directly:

python scripts/data_ingestion.py
python scripts/data_analysis.py

Results & Insights

Improved efficiency in large-scale IPL data processing using Spark SQL.

Derived key performance metrics for players and teams based on historical match data.

Optimized Spark queries to handle large datasets efficiently, reducing execution time.

Future Enhancements

Integrate machine learning models for performance prediction.

Deploy a dashboard for interactive data visualization.

Extend analysis to real-time IPL match data streaming.
