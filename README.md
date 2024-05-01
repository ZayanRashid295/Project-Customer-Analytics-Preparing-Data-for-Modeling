# Efficient Storage Solution for Customer Dataset

## Overview
This repository contains a proof-of-concept solution for efficiently storing and managing a large customer dataset provided by Training Data Ltd. The dataset is aimed at predicting whether students are looking for a new job or not. The solution focuses on optimizing the storage format of the dataset to reduce computational overhead and improve processing times for predictive modeling tasks.

## Dataset Description
The dataset, named `customer_train.csv`, is a subset of Training Data Ltd.'s customer dataset. It includes anonymized student information and their job-seeking status during training. Below is a brief description of the columns present in the dataset:

- `student_id`: A unique ID for each student.
- `city`: A code for the city the student lives in.
- `city_development_index`: A scaled development index for the city.
- `gender`: The student's gender.
- `relevant_experience`: An indicator of the student's work relevant experience.
- `enrolled_university`: The type of university course enrolled in (if any).
- `education_level`: The student's education level.
- `major_discipline`: The educational discipline of the student.
- `experience`: The student's total work experience (in years).
- `company_size`: The number of employees at the student's current employer.
- `last_new_job`: The number of years between the student's current and previous jobs.
- `training_hours`: The number of hours of training completed.
- `job_change`: An indicator of whether the student is looking for a new job (1) or not (0).

## Solution Approach
To address the challenge of efficiently storing and managing the large customer dataset, the following steps were implemented:

1. **Data Compression**: Utilized efficient data compression techniques to reduce the storage space required by the dataset without compromising data integrity.
2. **Columnar Storage**: Organized the dataset into a columnar storage format, which improves query performance by storing each column separately, allowing for faster data retrieval and processing.
3. **Parquet File Format**: Converted the dataset into the Parquet file format, a columnar storage file format optimized for use with distributed computing frameworks like Apache Spark. Parquet files offer efficient storage and retrieval of data, especially for analytical workloads.
4. **Partitioning**: Partitioned the dataset based on relevant attributes such as city or gender, if applicable, to further enhance query performance and optimize data access.

## Usage
To utilize the efficient storage solution for the customer dataset, follow these steps:

1. Clone the repository to your local machine.
2. Place the `customer_train.csv` dataset file in the designated directory.
3. Run the provided scripts to preprocess and convert the dataset into the optimized Parquet format.
4. Use the resulting Parquet files for predictive modeling tasks or analysis.

## Dependencies
- Python 3.x
- Pandas
- PyArrow


For any questions or inquiries, please contact at **zayan.rashidrana@studentambassadors.com**
