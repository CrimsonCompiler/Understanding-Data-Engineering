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



# Exercises

<img width="908" height="650" alt="image" src="https://github.com/user-attachments/assets/75ebafd9-4705-47b7-8617-047a8bf71554" />
<img width="1920" height="921" alt="image" src="https://github.com/user-attachments/assets/91090146-4fcf-47f3-b192-c5284dcd1063" />

