# Climate-Analysis

## Background

The objective of the StopFire initiative is to anticipate and avert fires within Victorian cities. In pursuit of this goal, sensors have been strategically placed across multiple Victorian cities. Despite these efforts, the sheer magnitude of the data has impeded the timely provision of fire predictions using their current methods. Our role as data analysts involves the migration of this data to a NoSQL database, specifically MongoDB for enhanced efficiency. Furthermore, we are entrusted with the creation of an application utilizing Apache Kafka and Apache Spark to streamline the processes of data streaming, storage, and analysis.

## File Description

### 1. PartA.ipynb
This notebook processes data from CSV files, constructs a model, stores it in MongoDB, and performs diverse queries on the database.

### 2. PartB_Producer1.ipynb
This notebook contains a Python program that loads data from climate_streaming.csv and randomly feeds it (with replacement) to the stream every 10 seconds.

### 3. PartB_Producer2.ipynb
This notebook contains a Python program that loads data from hotspot_AQUA_streaming.csv and randomly feeds it (with replacement) to the stream every 2 seconds. AQUA is a satellite from NASA that reports latitude, longitude, confidence, and surface temperature of a location.

### 4. PartB_Producer3.ipynb
This notebook contains a Python program that loads data from hotspot_TERRA_streaming.csv and randomly feeds it (with replacement) to the stream every 2 seconds. TERRA is another satellite from NASA that reports latitude, longitude, confidence, and surface temperature of a location.

### 5. PartB_Streaming_Application.ipynb
This notebook demonstrates an Apache Spark Structured Streaming application that processes data in 10-second batches from three producers.

### 6. PartB_Data_Visualisation.ipynb
This notebook showcases Python programs for visualizing real-time climate data, leveraging pymongo to fetch data from MongoDB collections generated in Streaming_Application.ipynb 
