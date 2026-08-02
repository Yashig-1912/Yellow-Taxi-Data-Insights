#🚖 Uber End-to-End Data Engineering Project
A comprehensive end-to-end data engineering pipeline built to process, model, and visualize New York City TLC yellow taxi trip data using modern cloud infrastructure, orchestration tools, and data warehousing.

##🏗️ Architecture Diagram
The following diagram illustrates the high-level flow of the pipeline—from ingesting the raw dataset into Mage AI for orchestration, loading it into Google BigQuery as a data warehouse, and finally connecting it to Data Studio for visualization:

<img width="960" height="540" alt="architecture" src="https://github.com/user-attachments/assets/997bea12-4be5-4ce5-952d-a47815cf06af" />


##📊 Table Distribution & Data Modeling (Star Schema)
To optimize query performance and analytical efficiency, the raw dataset was restructured using a dimensional modeling approach (star schema). The table distribution schema below outlines how the fact and dimension tables relate to each other:

<img width="1760" height="1206" alt="data_model" src="https://github.com/user-attachments/assets/4b4be337-bd11-4db1-8bae-5bd1c5d790c6" />


Fact Table (tbl_analytics): Stores core transactional metrics like trip distance, fare amounts, rate codes, and foreign keys.

Dimension Tables: Store descriptive attributes such as pickup/dropoff datetimes, passenger counts, payment types, and geographic coordinate lookups.

##🛠️ Tech Stack & Tools
Programming Language: Python (Pandas)

Orchestration / ETL: Mage AI

Cloud Infrastructure: Google Cloud Platform (GCP) Compute Engine

Data Warehouse: Google BigQuery

Visualization: Data Studio (Looker Studio)

##📸 Project Screenshots
1. Mage AI Pipeline Interface
The orchestrator handling the data ingestion, transformation blocks, and exports:

<img width="1462" height="770" alt="Screenshot 2026-08-02 170148" src="https://github.com/user-attachments/assets/24e296f1-a254-4056-8c65-067822087e18" />


2. BigQuery Dataset Tables
The structured tables successfully loaded into the Google BigQuery data warehouse:

<img width="706" height="840" alt="Screenshot 2026-08-02 164455" src="https://github.com/user-attachments/assets/c4d919f1-3628-4cc3-a85c-21eea3af981e" />


3. Final Looker / Data Studio Dashboard
The interactive dashboard visualizing trip metrics, pickup/dropoff locations, and temporal insights:

<img width="920" height="676" alt="Screenshot 2026-08-02 164400" src="https://github.com/user-attachments/assets/620b595c-e100-45b3-99e4-8173e8ff22b5" />

##Credits and Attributions
* **Architecture and Distribution Diagrams**: Sourced from [Darshil Parmar](https://github.com/darshilparmar)'s original project [repository](https://github.com/darshilparmar/uber-etl-pipeline-data-engineering-project)
