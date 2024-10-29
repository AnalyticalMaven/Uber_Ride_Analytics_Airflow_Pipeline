![image](https://github.com/user-attachments/assets/36585762-b229-4759-ab56-30cb00ecb965)


Project Overview
Purpose: An ETL pipeline designed for analyzing trips and bookings data from a ride-hailing company.
Goal: Generate insights to optimize operations and support data-driven decision-making.

Key Components

Data Ingestion:
Utilizes Apache Sqoop to import data from a MySQL database to HDFS.
Facilitates moving large volumes of data efficiently into a distributed storage system.

Data Organization:
Creates structured directories in HDFS to store the imported data cleanly.
Establishes Hive tables on the ingested data for easier querying and management.

Partitioning:
Partitions the Hive tables based on key dimensions (e.g., city, car type) to optimize performance.
Enhances query speed and efficiency in data retrieval for analytics.

Data Cleansing:
Leverages Apache Spark to filter out invalid records from the dataset.
Ensures data quality and reliability for accurate analysis.

Analytics and Insights:
Runs analytical queries using Spark to generate key insights:
Identifies car types with the highest number of trips per city.
Calculates trip throughput rates (number of trips/number of bookings) for each city.


Benefits

Scalability: 
Designed to handle large datasets efficiently, making it suitable for big data environments.
Automation: Airflow orchestrates the entire pipeline, ensuring tasks run smoothly and on schedule.
Data-Driven Decisions: Provides valuable insights that help optimize ride-hailing operations and enhance service quality.




