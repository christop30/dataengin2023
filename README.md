Peer Review for DE

# airflow-dag-covid19
Basic data pipeline to handle covid19 data sources utilizing Python and Airlflow.

## Setup Steps

1 pip3 install airflow

2. estructure in dag

owid_to_bq.py
owid_covid_dag/
--------------extract.py
--------------transform.py
--------------load.py

Ghrap on Airflow

![image](https://user-images.githubusercontent.com/31247855/215329871-2b46d5ee-bbc1-4642-8bdf-a767516985f6.png)

Create a Schema in Google Cloud

![image](https://user-images.githubusercontent.com/31247855/215330175-1fde5a42-2126-4c64-ac1c-b432067695cf.png)

![image](https://user-images.githubusercontent.com/31247855/215330109-1cd77003-750c-449f-a3af-fd86375ff086.png)

# If you run airflow locally install 

pip install google-cloud-bigquery[pandas,pyarrow]
