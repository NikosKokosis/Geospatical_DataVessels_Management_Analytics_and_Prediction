- YourRepoName/
  - Code/
    - Sql_Queries.ipynb
    - EDA_and_DataCleaning.ipynb
    - Data_Enrichment.ipynb
    - Predict_the_Location.ipynb

# Maritime Data Analysis and Prediction Project

## Project Overview

This project focuses on maritime data analysis and prediction, using real data collected from the Automatic Identification System (AIS) antenna located at the University of Piraeus. The goal is to gain insights into vessel movements and develop predictive models for ship trajectories. The project is divided into five main phases, each addressing different aspects of data processing, analysis, and prediction.

## [Phase 1: Database Setup and Data Collection](Code/Sql_Queries.ipynb)

In the initial phase, a database named "thalassaDB" is created to store AIS data. The data is collected from real vessels within the antenna's range, focusing on passenger vessels that have visited Piraeus Port. Velocity filtering is applied to ensure that only vessels in motion are considered. The collected data is then organized and stored in a spatial database.

## [Phase 2: Data Exploration and Database Queries](Code/Sql_Queries.ipynb)

This phase involves exploring the collected data through SQL queries. The database is queried to answer various questions related to vessel information, distances, speeds, and port activities. Additional data, such as port locations and geometries, is manually added to enhance the database's completeness.

## [Phase 3: Exploratory Data Analysis](Code/EDA_and_DataCleaning.ipynb)

In the EDA phase, Python and GeoPandas are employed to perform more complex analyses that may be challenging with SQL alone. This includes examining specific passenger ships' AIS messages, calculating message counts, and analyzing maximum speeds and port proximity for a given day.

## [Phase 4: Data Cleaning and Enrichment](Code/Data_Enrichment.ipynb)

Data cleaning and enrichment are essential for improving data quality and relevance. The project focuses on adding ship-related information like status classification conditions and maximum acceptable speeds based on ship types. Data anomalies, such as duplicate messages or excessive speeds, are identified and removed. The Dataset is further enriched by segmenting vessel routes and identifying navigational statuses over time.

## [Phase 5: Trajectory Prediction](Code/Predict_the_Location.ipynb)

In this phase, trajectory prediction models are developed using advanced techniques like bidirectional Gated Recurrent Units (GRU). The goal is to predict vessel location based on historical data. Evaluation metrics like Root Mean Squared Error (RMSE) are used to assess the predictive performance of the models. The project achieves an RMSE of 23.21, demonstrating the effectiveness of the predictive models.

## Conclusion

This maritime data analysis and prediction project offers valuable insights into vessel movements, speeds, and port activities. By collecting, processing, and analyzing real AIS data and utilizing advanced prediction models, we aim to enhance maritime safety and decision-making. The successful prediction results, which enable us to anticipate vessel locations in the near future, validate the project's significance in the maritime domain.