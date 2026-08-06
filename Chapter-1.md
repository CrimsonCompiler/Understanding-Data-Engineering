# Chapter 1

## Data Engineers vs. Data Scientists

To prevent confusion between these two critical roles, it is essential to understand how they contrast and collaborate within the data workflow. In short, **data engineers lay the groundwork that makes data science activity possible**.

### Role Comparison

| Feature | Data Engineer | Data Scientist |
| :--- | :--- | :--- |
| **Workflow Stage** | Ingestion and storage. | Preparation, exploration, visualization, and experimentation. |
| **Primary Focus** | Making data accessible and ready for analysis. | Exploiting data to find insights, run experiments, or build predictive models. |
| **Core Responsibilities** | Ensuring databases are optimized for analysis and building automated data pipelines. | Using pipeline outputs according to their analysis needs. |
| **Expertise** | Software development and architecture. | Analytics and statistics. |
| **Tools & Languages** | Software-oriented Python, Java, SQL (to create, update, and transform databases). | Analytics-oriented Python, R, SQL (to query and request information). |

### Case Study: Spotflix in Action
To illustrate how data engineers enable data scientists, consider their workflow at Spotflix:

* **The Data Engineer (Vivian):** Collects and stores customer, artist, and song data in their respective databases. She ensures the table structures are correct and builds data pipelines that automatically pull listening session data so everything remains up to date.
* **The Data Scientist (Julian):** Uses the easily accessible data from Vivian's pipelines to understand listening patterns and build recommendation engines, without needing to spend excessive time on data preparation.

## The Data Pipeline

To understand data pipelines, it helps to use the analogy that "Data is the new oil". Just as crude oil is extracted, moved, and distilled into various products like kerosene or gasoline, raw data must also be systematically extracted, processed, and distributed. 

### What is a Data Pipeline?
* Data pipelines ensure the data flows efficiently through the organization.
* They automate the processes of extracting, transforming, combining, validating, and loading data. 
* This automation reduces human intervention and errors.
* It also significantly decreases the time it takes for data to flow through the organization.

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/79f93091-e36a-453d-9886-93b4ca05ce78" />


### Case Study: Pipelines at Spotflix
At Spotflix, data pipelines handle massive amounts of information to ensure data scientists have up-to-date and accurate data:
* **Ingestion:** Data is extracted from various sources, including the mobile app, the desktop app, the Spotflix website, and internal HR systems.
* **Storage Routing:** This raw data is first moved from its respective sources into a data lake. 
* **Organization:** From there, pipelines organize the data by moving it into specific databases, such as artists, albums, tracks, playlists, customers, and employees. 
* **Further Processing:** Additional pipelines are used to process data, such as checking if a track is readable and in the correct size, before storing it in a clean tracks database. 

### ETL vs. Data Pipelines
* **ETL (Extract, Transform, Load):** ETL is a popular framework for designing data pipelines where the key principle is that data is processed *before* it is stored. It involves three sequential steps: extracting the data, transforming it, and finally loading this transformed data into a new database.
* **General Data Pipelines:** Broadly, data pipelines move data from one system to another. While they may follow the ETL framework, they do not always have to; for instance, data might be routed directly to visualization tools without undergoing any transformation.


# Exercises

<img width="1920" height="924" alt="image" src="https://github.com/user-attachments/assets/a5256df8-6fba-4a63-8291-9705ba5feb47" />

<img width="1920" height="919" alt="image" src="https://github.com/user-attachments/assets/b191f711-77e9-466b-b09a-06c028db3806" />

<img width="1920" height="922" alt="image" src="https://github.com/user-attachments/assets/eae07890-971f-4f35-8bb8-ecb40a9b4b7d" />

<img width="1915" height="920" alt="image" src="https://github.com/user-attachments/assets/6bba2c78-ae29-4985-b3bb-b6d7a3eb7bd9" />

<img width="920" height="693" alt="image" src="https://github.com/user-attachments/assets/9634f450-5d25-454d-a67a-50594e621750" />

<img width="997" height="683" alt="image" src="https://github.com/user-attachments/assets/a1e5e879-7143-45f7-97b0-202790a30326" />

<img width="1918" height="880" alt="image" src="https://github.com/user-attachments/assets/949284ab-664a-4ce2-948a-d8d2196ed79c" />


