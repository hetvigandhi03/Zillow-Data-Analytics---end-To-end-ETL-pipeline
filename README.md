# Zillow-Data-Analytics---end-To-end-ETL-pipeline



https://github.com/hetvigandhi03/Zillow-Data-Analytics---end-To-end-ETL-pipeline/assets/75487912/758fe65d-58dc-4f11-9fff-f9df01161cc2



Built and automated a python ETL process that would :

-  extract real estate properties data from Zillow Rapid API,
-  loads it unto amazon s3 bucket which then triggers a series of lambda functions which then ultimately transforms the data 
- converts into a csv file format and load the data into another S3 bucket using Apache Airflow. 
- Apache airflow will utilize an S3KeySensor operator to monitor if the transformed data has been uploaded into the aws S3 bucket before attempting to load the data into an amazon redshift. 
- After the data is loaded into aws redshift, then we will connect amazon quicksight to the redshift cluster to then visualize the Zillow (rapid data) data.
