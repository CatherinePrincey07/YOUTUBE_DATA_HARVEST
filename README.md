# Youtube_Data

# YouTube Data Harvesting and Warehousing.

## Introduction 

* YouTube, the online video-sharing platform, has revolutionized the way we consume and interact with media. Launched in 2005, it has grown into a global phenomenon, serving as a hub for entertainment, education, and community engagement. With its vast user base and diverse content library, YouTube has become a powerful tool for individuals, creators, and businesses to share their stories, express themselves, and connect with audiences worldwide.

* This project extracts the particular youtube channel data by using the youtube channel id, processes the data, and stores it in the MongoDB database. It has the option to migrate the data to postgreSQL from MongoDB then analyse the data and give the results depending on the customer questions.

## Developer Guide 

### 1. Tools Install

* Virtual code.
* Visual Studio Code.
* Python 3.12.2 or higher.
* PostgreSQL.
* MongoDB.
* Youtube API key.

### 2. Requirement Libraries to Install

* pip install google-api-python-client, pymongo, psycopg2, pandas, streamlit.
 
### 3. Import Libraries

**Youtube API libraries**

* from googleapiclient.discovery import build
* import pymongo
* import psycopg2
* import pandas as pd
* import streamlit as st

### 4. E T L Process

#### a) Extract data

* Extract the particular youtube channel data by using the youtube channel id, with the help of the youtube API developer console.

#### b) Process and Transform the data

* After the extraction process, takes the required details from the extraction data and transform it into JSON format.

#### c) Load  data 

* After the transformation process, the JSON format data is stored in the MongoDB database, also It has the option to migrate the data to PostgreSQL database from the MongoDB database.

### 5. E D A Process and Framework

#### a) Access PostgreSQL DB 

* Create a connection to the PostgreSQL server and access the specified PostgreSQL DataBase by using psycopg2 library and access tables.

#### b) Filter the data

* Filter and process the collected data from the tables depending on the given requirements by using postgreSQL queries and transform the processed data into a DataFrame format.

#### c) Visualization 

* Finally, create a Dashboard by using Streamlit and give dropdown options on the Dashboard to the user and select a question from that menu to analyse the data and show the output in Dataframe Table.


## User Guide

#### Step 1. Data collection zone

* Search **channel_id**, copy and paste in **Enter the channelid** box and click the **Collect and store data** button in the **Data collection zone**.

#### Step 2. Data Migrate zone

* click the **Migrate to SQL** button to migrate the specific channel data to the pgadmin4 database from MongoDB .

#### Step 3. Channel Data Analysis zone

* **Select a Question** from the dropdown option you can get the **results in Dataframe format.**.


## Video link:

