## Chapter 2: Data Structures

In this chapter, we shift our focus to data storage by exploring the three fundamental types of data structures. Understanding these structures is crucial because they determine how data is stored, queried, and utilized.

### 1. Structured Data
* **Characteristics:** Highly organized and follows a rigid, predefined model—much like a spreadsheet with rows and columns. Each column strictly accepts values of a certain data type (e.g., text, date, decimal, or boolean/logical values). It accounts for about 20% of all data.
* **Storage & Querying:** Stored in **Relational Databases**. Because of its rigid structure, tables can be easily connected to one another (e.g., linking an employee table to an office table using an "office" column). It is queried using **SQL** (Structured Query Language).
* **Spotflix Example:** The *Employee Table*. Each row represents a unique employee (identified by a numeric unique ID/index), and columns contain specific details like team and role.

<img width="1154" height="477" alt="image" src="https://github.com/user-attachments/assets/f9842b15-e8bb-451b-9991-5d0ccaf3424c" />


### 2. Semi-Structured Data
* **Characteristics:** Resembles structured data but offers much more flexibility. It maintains a consistent hierarchy or model but does not restrict data to a rigid row-and-column format.
* **Storage & Formats:** Typically stored in **NoSQL databases**. It heavily leverages file formats like **JSON, XML, or YAML**.
* **Spotflix Example:** A *JSON file of favorite artists*. Every user record might contain a first name, last name, and a list of favorite artists. However, the exact number of artists can vary per user (one user might have 4, while another has 2). Relational databases struggle with this variability, but semi-structured formats handle it seamlessly.

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/f52b9322-4a98-4148-84fc-c52ca39c35a8" />

### 3. Unstructured Data
* **Characteristics:** Does not follow a predefined model and cannot be contained in a traditional row-and-column format. While it makes up the vast majority of data generated today, it is notoriously difficult to search and organize.
* **Storage:** Usually stored in **Data Lakes**.
* **Spotflix Example:** The actual media files—audio tracks, text lyrics, album cover pictures, artist profile photos, and music videos.
* **Extracting Value:** Unstructured data is incredibly valuable. Historically hard to exploit, recent advances in **Machine Learning (ML) and AI** have made it possible to analyze this data. For instance, ML algorithms can scan an unstructured audio file to extract its BPM, chord progression, and genre. Alternatively, adding manual tags (metadata) to a song file can transform it into semi-structured data, instantly making it easier to organize and search.
  
<img width="1920" height="1079" alt="image" src="https://github.com/user-attachments/assets/c316496a-f724-466c-863d-f7d1b3898d9f" />



## The Role of SQL in Data Engineering

SQL (Structured Query Language) is to databases what English is to pop music—fundamental and ubiquitous. It is the preferred language for querying **Relational Database Management Systems (RDBMS)**, where multiple tables are systematically connected.

### Why SQL?
* **Powerful Operations:** It allows you to access many records at once and easily group, filter, or aggregate them.
* **Readable Syntax:** Its structure is very close to plain English, making it intuitive to write and understand.
* **Varied Implementations:** There are several SQL dialects/implementations. Switching between them is like switching from American to British English—a few nuances change, but the core logic remains exactly the same.

### How Different Roles Use SQL
While both roles rely heavily on SQL, their day-to-day objectives differ:

* **Data Engineers (Building & Maintaining):** Use SQL to define database architecture and write records. For example, using a `CREATE TABLE` command to build an `employees` table:
  * Defining `employee_id` as an Integer (whole numbers).
  * Defining `first_name` as VARCHAR (variable characters/text up to a specific limit).
  * Defining `full_time` as a Boolean (logical true/false values).
* **Data Scientists (Querying & Analyzing):** Use SQL to extract specific insights. For example, using a `SELECT` statement to pull the first and last names `FROM` the employees table `WHERE` the role title contains a keyword like "Data".

### Understanding Database Schemas
A single table is useful, but a database consists of many tables. The **database schema** is the blueprint that governs how all these tables are related to one another.

**Spotflix Relational Schema Example:**
* **Artists Table:** Contains a unique Artist ID, name, and biography.
* **Albums Table:** Contains an Album ID and an Artist ID. *(Linked to the Artists table via Artist ID).*
* **Songs Table:** Contains a Song ID and an Album ID. *(Linked to the Albums table via Album ID).*
* **Playlists Table:** Contains a Playlist ID and a Song ID. *(Linked to the Songs table via Song ID).*

Because these tables can be connected logically through shared IDs, they form a highly organized **relational** database that is extremely efficient to query.

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/e1f795d0-cd30-4ae3-a34e-a84cac7618c2" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/cdc00e1b-c8d1-49cc-bf16-86fe417f09e3" />

# Exercises

<img width="908" height="650" alt="image" src="https://github.com/user-attachments/assets/75ebafd9-4705-47b7-8617-047a8bf71554" />
<img width="1920" height="921" alt="image" src="https://github.com/user-attachments/assets/91090146-4fcf-47f3-b192-c5284dcd1063" />
<img width="924" height="584" alt="image" src="https://github.com/user-attachments/assets/8ee0d1e3-ca45-46a9-966e-1b45634ea46a" />
<img width="890" height="752" alt="image" src="https://github.com/user-attachments/assets/7bd9340a-861f-4760-8d62-7c89c7fdbaa8" />
<img width="892" height="441" alt="image" src="https://github.com/user-attachments/assets/66cf76dd-cb5c-4b1f-af72-3c393129f32e" />
<img width="1920" height="920" alt="image" src="https://github.com/user-attachments/assets/f77f4ec0-17d6-4556-962a-9261d0ae999c" />


