# ID2221-project


## Description
The project attempts to understand what factors most affect salaries for the position of a data scientist. By scraping job postings from Glassdoor, it looks at key factors such as location, required skills, experience level, and company characteristics that produce the largest variation in salaries. This will provide a good overview of what one can expect from a data scientist given many different job characteristics, while enabling employers to make a more reasoned compensation decision. 

## Requirments

Our project was originally developed to run datasets over HDFS system, thus Hadoop (available at: https://hadoop.apache.org/) should be downloaded and properly setup before running the project file. 

## Installation

To get started with the project, follow these simple steps:

1. **Clone the Repository:**

    ```bash
    $ git clone https://github.com/ericbanzuzi/ID2221-project.git
    ```

2. **Create a virtual environment or conda environment using python 3.9+.**

3. **Setup HDFS in your machine**

4. **Install Dependencies:**

   ```bash
   $ pip install -r requirements.txt
   ```

5. **Start the Jupyter notebook in VS Code using you `.venv` or conda environment as the python kernel or using the following command:**

   ```bash
   $ jupyter-notebook .
   ```

   Make sure your python environment is active.

The whole solution is in the `ds_salary_study.ipynb` notebook. 

## Data
The data  comes from Glassdoor through [Kaggle: Jobs Dataset from Glassdoor](https://www.kaggle.com/datasets/thedevastator/jobs-dataset-from-glassdoor). It includes information on job titles, companies, salaries, location, and many other factors related to the role data scientist roles. 


## Analysis approach

1. Collect the data from Kaggle and store it in HDFS to ensure the data is readily available in parallel.
2. Clean and pre-process the data using PySpark.
3. Perform exploratory data analysis (EDA) using Spark SQL from PySpark and Python visualization tools to identify key factors influencing data science salaries.
4. Split the data into training and testing sets, then build and evaluate regression models using Spark MLlib or an appropriate Python library to predict data science job salaries.
5. Visualize results with Python visualization tools.

