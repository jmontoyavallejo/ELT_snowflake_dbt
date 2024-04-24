# dbt framework project for python with Snowflake

This repository provides a set of tools and resources to streamline your data transformation workflows using the python framework dbt, specifically targeting snowflake as the database backend.

## Requirements

* Python
* DBT (Data Build Tool)
* Snowflake Account

# Overview

## Snowflake setup for dw, role, db and schema

Configuring Snowflake with the necessary roles, databases, and schemas for data warehouse operations.

[![Image Title](assets/images/snowflake_setup.png)](https://github.com/jmontoyavallejo/ELT_dbt_bigquery_project/blob/main/assets/images/bigquery.png)

## **Building Dimensional Models and Facts Models**

Implementing dimensional modeling techniques to create dimension tables and fact tables within Snowflake using DBT.

![1714000741231](assets/images/lineage_graph.png)

## **Building Macros for Functions**

Utilizing DBT's macro functionality to create reusable functions for common data transformations and calculations.


## **Building General Tests and Individual Tests**

Implementing data quality tests and integrity checks at both the general and individual level to ensure the accuracy and reliability of the data.

![1714000637094](assets/images/tests.png)

## Final result in snowflake

All tables and views have been successfully created in the Snowflake data warehouse based on the defined data models and transformations.

![1714001010705](assets/images/snowflake.png)

## **Generating the Docs automatically**

Utilizing DBT's documentation generation features to automatically generate comprehensive documentation for the data models, tests, and macros implemented in the project.

![1714000611418](assets/images/dct_docs.png)


## Usage

**Setup Snowflake Environment and python env**:

* Ensure that Snowflake is properly configured with the required roles, databases, and schemas as specified in the project configuration files.
* Create a python env using *python3 -m vevn dbt-env* and then *pip install -r requirements.txt*
* Create a DBT profile  called data_pipeline, here i leave a guide to do it https://docs.getdbt.com/docs/core/connect-data-platform/connection-profiles

**Run DBT Commands** :

* Execute the necessary DBT commands:
  * `dbt run or dbt run -s <specific table> ` to run the whole project or specific tables
  * `dbt test` to run the tests
  * `dbt docs generate` to generate documentation.

## Contributing


If you would like to contribute to this repository, feel free to fork the project and submit a pull request. We welcome contributions from the community and appreciate any help that we can get.
