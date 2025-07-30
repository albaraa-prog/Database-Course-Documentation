# Task 1: Comparison – Flat File Systems vs. Relational Databases  

This section compares **Flat File Systems** and **Relational Databases** across key aspects such as structure, redundancy, relationships, usage, and drawbacks.

---

## 1. Structure  
- **Flat File Systems:**  
  - Organize data as plain text or binary files in directories.  
  - No inherent data model — data is often stored in tabular form (e.g., CSV) or custom formats.  
  - Example: NTFS (New Technology File System), EXT (Extended File System).  

- **Relational Databases:**  
  - Data is stored in structured **tables** (rows & columns).  
  - Follows a **schema** with defined data types and relationships.  
  - Example: MySQL, Oracle, MS SQL Server.  

---

## 2. Data Redundancy  
- **Flat File Systems:**  
  - High risk of **data duplication** because files are independent and lack normalization.  
  - Updating a value in one file does **not** automatically update it in others.  

- **Relational Databases:**  
  - **Reduced redundancy** through **normalization** and centralized data storage.  
  - Data is consistent across multiple applications.  

---

## 3. Relationships  
- **Flat File Systems:**  
  - **No direct relationships** between data in different files.  
  - Relationships must be managed manually by application code.  

- **Relational Databases:**  
  - Supports **relationships** using **primary keys**, **foreign keys**, and **joins**.  
  - Enables complex queries across multiple tables.  

---

## 4. Example Usage  
- **Flat File Systems:**  
  - Used for **simple storage** like configuration files, log files, or small standalone applications.  
  - Example: Storing user preferences in `.txt` or `.json` files.  

- **Relational Databases:**  
  - Used for **enterprise applications** requiring structured data, such as banking systems, e-commerce platforms, and CRMs.  
  - Example: Customer data management in MySQL.  

---

## 5. Drawbacks  
- **Flat File Systems:**  
  - **Limited security** features.  
  - **Difficult to maintain** with large datasets.  
  - **Poor scalability** and lacks concurrent access support.  

- **Relational Databases:**  
  - **More complex** to set up and manage.  
  - **Higher cost** for licensing and infrastructure.  
  - Requires **specialized knowledge** for design and maintenance.  

---

## Visual Comparison Table

| Feature              | Flat File Systems                  | Relational Databases              |
|----------------------|-----------------------------------|-----------------------------------|
| **Structure**        | Files in directories              | Tables with schema               |
| **Data Redundancy**  | High                              | Low (Normalized)                 |
| **Relationships**    | Manual (no built-in support)      | Built-in (Keys & Joins)          |
| **Example Usage**    | Config/log files                  | Banking, CRM, E-commerce         |
| **Drawbacks**        | Low security, poor scalability    | Complex setup, higher cost       |

---

# Task 2: DBMS Advantages – Mind Map

<img width="812" height="486" alt="taask2 drawio" src="https://github.com/user-attachments/assets/f507e60b-6662-47ff-a868-93899a29104f" />

---

