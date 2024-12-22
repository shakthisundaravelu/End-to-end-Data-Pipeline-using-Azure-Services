# End-to-end data pipeline and analysis of Tokyo Olympic data using Azure services

![image](https://github.com/user-attachments/assets/3ba8773f-5a18-4284-aafa-f4f81b589292)


- Created a storage account in Azure and created two folders to store raw data and transform data

![image](https://github.com/user-attachments/assets/dd00610d-a5d1-486a-a81a-183cf754252a)

- Created and deployed a pipeline in Azure Data Factory to pull the data from GitHub and push it to the Data Lake storage account in Azure under the raw_data folder

![image](https://github.com/user-attachments/assets/4f538083-cdc7-4088-9a2a-bc3861f70042)


- After the pipeline is deployed, the raw data is pulled from the Git Hub Repo and pushed to the Data Lake Gen 2 storage account raw-data folder

![image](https://github.com/user-attachments/assets/99e468a3-790a-40d6-9052-98e6ed3ca63f)


- Integrated and deployed Azure data bricks to process the raw data and store the transformed data in Data Lake Gen 2 for further analysis.
- Deployed a data bricks cluster to run the data transformation using Spark and mounted  the ADLS Gen 2 container to a DBFS path.
- Created an app registration in the Azure portal to link the data lake storage with the Azure data bricks with roles assigned as data storage contributor

![image](https://github.com/user-attachments/assets/2d27ec1c-70a1-4828-a5d9-2a70295d0ce1)


![image](https://github.com/user-attachments/assets/5a579b18-4162-4e19-82d9-dc1e3e74c6e1)

- The transformed data is then mounted to the Data Lake storage under the transformed-data folder

![image](https://github.com/user-attachments/assets/8472ec91-6b45-4a8e-a43f-ad4599cad4b9)


- Deployed Azure Synapse workspace to analyze the transformed data from the Data Lake Gen 2 storage to derive insights

- Created a Lake database inside the Azure Synapse workspace and imported the transformed data as tables for analysis

![image](https://github.com/user-attachments/assets/99f24a81-9d39-4f8e-a0f2-784a12eeb0d1)




- Performed general data analysis using SQL to derive insights on the data and generated graphs as the visualization

- average number of entries by gender for each discipline

![SQL script 3](https://github.com/user-attachments/assets/7a1544f1-5ae8-44f6-b4e7-0a065d0e1c09)

- the total medals won by each country

![SQL script 3 (1)](https://github.com/user-attachments/assets/31be3351-29fe-44df-b1f8-979d75131c84)

- number of athletes from each country

![SQL script 3 (2)](https://github.com/user-attachments/assets/0c1e616e-cca5-4c03-87d5-258a357457ef)




