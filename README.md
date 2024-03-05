# Home Sales Data Analysis with SparkSQL

## Overview

In this project, I leveraged SparkSQL to analyze a dataset of home sales. The goal was to extract insightful metrics about the sales data, utilizing Spark's capabilities for data processing and analysis. Through this challenge, I honed my skills in handling large datasets, optimizing query performance, and effectively using SparkSQL for real-world data analysis tasks.

## Process

Using SparkSQL, I answered several key questions about the dataset, such as the average sale price of homes based on various criteria, including bedroom count, year built, and view rating. Notably, I focused on:

-   Average sale price for four-bedroom homes sold each year.
-   Average sale price of homes built in each year, with specific configurations (three bedrooms, three bathrooms, two floors, and size criteria).
-   Average sale price of homes per "view" rating, specifically for homes priced at or above $350,000.

To optimize the analysis, I utilized caching for the `home_sales` table, compared runtime performance between cached and uncached data, and experimented with data partitioning based on the "date_built" field.

## Key Takeaways

-   I successfully determined the average sale prices for homes under various conditions, rounded to two decimal places.
-   By caching the temporary table `home_sales`, I noted a performance improvement in query execution time, validating the effectiveness of caching in Spark.
-   Partitioning the data based on the "date_built" field and analyzing the performance offered insights into optimizing large dataset queries.
-   The uncaching process and verification of the `home_sales` table's cache status underscored the importance of resource management in Spark.

To summarize, this challenge not only bolstered my understanding of SparkSQL but also highlighted Spark's powerful tools for data analysis and optimization. 
