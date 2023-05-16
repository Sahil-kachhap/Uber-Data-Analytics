# Uber-Data-Analytics
The goal of this project is to perform data analytics on Uber data using various tools and technologies, including GCP Storage, Python, Compute Instance, Mage Data Pipeline Tool, BigQuery, and Looker Studio.

## Architecture
![architecture](https://user-images.githubusercontent.com/54017876/235878391-207dc35f-b1ec-4962-8ef8-830af7afdce1.jpg)

## Data Model
![data_model](https://user-images.githubusercontent.com/54017876/235878547-29a0b380-d2a8-470f-b7be-6fc3bbd26876.jpeg)

## 📌 Steps followed and Learnings 
1. Extracted the data and loaded it into Google Cloud Storage for further processing.
2. Transformed and modelled the data using fact and dimensional data modelling concepts using Python on Jupyter Notebook.
3. Orchestrated the ETL process/data pipeline on Mage and loaded the transformed data into Google BigQuery.
4. Developed a dashboard on Looker Studio.

✅ LEARNING LESSONS
- Initially, I created a cloud instance with 1 CPU and 4GB of memory. However, as I started working on Mage, I experienced significant lag. To overcome this, I created a new instance with 4 CPUs and 16GB of memory instead and performance improved. 👍🏻

- Mage would occasionally shut down unexpectedly. To resolve this, I restarted SSH which prompted me to switch to a different port. It was only after several attempts that I realised that I had to create a new firewall rule to allow access to the new port. 😅

- If all else fails, verify the ephemeral URL as mine changed unexpectedly.

✨ INTERESTING INSIGHTS
- Standard rate code generates the highest revenue indicating its popularity among users. 
- On average, trips to Newark result in the highest tip at $11.
- Credit cards are the preferred mode of payment accounting for a significant 75% of all transactions, followed by cash.
- One-person trips make up the majority, comprising 66% of all recorded journeys. 
- The bustling area around Jackson Ave, near the Queens Plaza station in Long Island City stands out as the top pickup location. 
- The highest fare occurs at 2pm suggesting a peak period of travel. In contrast, the lowest fare is observed at 7am, likely due to off-peak hours.

## Technology Used 
- Python
- Google Cloud Storage
- Mage - modern data pipeline tool
- Google Cloud Compute VM instance
- BigQuery
- Looker Studio

## Dataset Used
TLC Trip Record Data Yellow and green taxi trip records include fields capturing pick-up and drop-off dates/times, pick-up and drop-off locations, trip distances, itemized fares, rate types, payment types, and driver-reported passenger counts.
