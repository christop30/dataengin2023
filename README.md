Peer Review for DE

Description Problem

We need to take Data from Covid confirm cases from https://github.com/owid/covid-19-data
add some field and load ina BigQuery (Google Cloud)

# airflow-dag-covid19
Basic data pipeline to handle covid19 data sources utilizing Python and Airlflow.

## Setup Steps

1. pip3 install airflow

2. estructure in dag

owid_to_bq.py

owid_covid_dag/

--------------extract.py

--------------transform.py

--------------load.py

Ghrap on Airflow

We have 2 task run_etl and check_bigquery

![image](https://user-images.githubusercontent.com/31247855/215329871-2b46d5ee-bbc1-4642-8bdf-a767516985f6.png)

Create a Schema in Google Cloud

![image](https://user-images.githubusercontent.com/31247855/215330175-1fde5a42-2126-4c64-ac1c-b432067695cf.png)

![image](https://user-images.githubusercontent.com/31247855/215330109-1cd77003-750c-449f-a3af-fd86375ff086.png)

## If you run airflow locally install 

pip install google-cloud-bigquery[pandas,pyarrow]

## Set your credentials in Google Cloud 

![image](https://user-images.githubusercontent.com/31247855/215484617-63c55da4-ad4b-4cd0-a3e0-c7a4906fbabd.png)

In load.py you line 12 you need to set your google cloud environment   table_id = "PROJECTNAME.DATASETNAME.TABLENAME"

![image](https://user-images.githubusercontent.com/31247855/216761403-59fc963d-e8cb-437e-a144-a0ad34c93d29.png)

Now we check our data in BigQuery

![image](https://user-images.githubusercontent.com/31247855/216761416-70363f3c-5e59-4315-83b8-1810cdf0164a.png)

BigQuery Data

![image](https://user-images.githubusercontent.com/31247855/217383402-ce7109e7-fb4f-47ce-86f5-645ba80b38c1.png)

Data Studio Screenshots (Feel free to use the Dashboard in the next link https://lookerstudio.google.com/reporting/e3a1df84-4abd-4ed4-ba4a-8c606aeef06d )

![image](https://user-images.githubusercontent.com/31247855/217383512-a1c8122c-da2f-429c-b0a6-22e4671e256a.png)

![image](https://user-images.githubusercontent.com/31247855/217383847-2d777532-9a6e-4ff4-bb26-70dadbff4146.png)

![image](https://user-images.githubusercontent.com/31247855/217383925-4bb3cf2b-ada5-4d0b-ae7d-adc0b130dd54.png)



