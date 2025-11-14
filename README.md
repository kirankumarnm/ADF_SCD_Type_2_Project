****ADF_SCD_Type_2_Project****



🔷 Project Overview

This project showcases an end-to-end implementation of Slowly Changing Dimension (SCD) Type 2 using Azure Data Factory Data Flows.
Source data is ingested from Azure Blob Storage, transformed using a series of Data Flow transformations, and finally loaded into the ADLS Gen2 curated zone.

To accurately implement SCD Type 2, hash-based comparison logic was used to detect changes between incoming and existing records. New and updated records were processed accordingly to maintain historical data integrity.

ADF Data Flow Activities Utilized

Source – Reads data from Blob Storage

Derived Column – Creates hash keys and applies transformation logic

Alter Row – Identifies insert and update conditions required for SCD Type 2

Select – Manages column mappings and renaming

Exists – Checks for record presence in the target dimension table

Sink – Loads the processed data into ADLS Gen2

This implementation highlights practical experience in building scalable ETL pipelines, designing SCD Type 2 flows, and leveraging Azure Data Factory to manage historical data efficiently.

***Architecture***

<img width="1745" height="412" alt="DataFlow_ADF_SCD_Type2" src="https://github.com/user-attachments/assets/bec6f958-142a-4208-b30a-fb4849033e89" />


