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

# Task 3: Roles in a Database System

In a database project, different roles ensure that the system is designed, implemented, and maintained effectively. Below are the key roles:

## **1. System Analyst**
- **Responsibilities:**  
  - Gathers and analyzes business requirements.  
  - Acts as a bridge between business stakeholders and technical teams.  
  - Defines the overall scope and objectives of the database system.  

## **2. Database Designer**
- **Responsibilities:**  
  - Designs the conceptual, logical, and physical database models.  
  - Ensures that the database structure supports business needs.  
  - Defines relationships, keys, and constraints to maintain data integrity.  

## **3. Database Developer**
- **Responsibilities:**  
  - Implements the database design using SQL and other database technologies.  
  - Creates stored procedures, functions, triggers, and views.  
  - Optimizes queries for better performance.  

## **4. Database Administrator (DBA)**
- **Responsibilities:**  
  - Manages database installations, configurations, and upgrades.  
  - Ensures data security, backup, and recovery strategies.  
  - Monitors performance and tunes the database for efficiency.  

## **5. Application Developer**
- **Responsibilities:**  
  - Builds applications that interact with the database.  
  - Implements user interfaces and integrates database operations.  
  - Ensures application-level data validation and processing.  

## **6. BI (Business Intelligence) Developer**
- **Responsibilities:**  
  - Designs and develops reporting and analytics solutions.  
  - Extracts insights from data using dashboards, reports, and visualizations.  
  - Works with ETL (Extract, Transform, Load) processes for data warehousing.  

---

# Privileges and Roles in DBMS

In Database Management Systems (DBMS), **security** ensures that data is confidential, accurate, and accessible only to authorized users, often summarized by the **CIA triad** (Confidentiality, Integrity, Availability).  

## **Authentication vs Authorization**
- **Authentication:** Verifying the identity of a user or process.  
- **Authorization:** Granting permission to access specific database objects in a controlled manner.  

Authorization types:
- **Read-only**
- **Read and write**
- **Execute**

---

## **Privileges**
Privileges define what actions a user can perform on database objects.  

### **Types of Privileges**
1. **Database Privileges:**  
   - Permission to execute SQL statements or access another user's object.  
   - Example: `CREATE SESSION` to connect to the database.  

2. **System Privileges:**  
   - Rights to perform actions on the entire system.  
   - Example: `CREATE`, `ALTER`, `DROP` (affecting database objects globally).  
   - Used for **DDL (Data Definition Language)** statements.  

3. **Object Privileges:**  
   - Rights to perform specific actions on a table, function, or package.  
   - Example: `SELECT`, `INSERT`, `DELETE`, `UPDATE`.  
   - Used for **DML (Data Manipulation Language)** statements.  

### **Differences Between System and Object Privileges**
| **System Privileges** | **Object Privileges** |
|-----------------------|------------------------|
| Granted by Database Administrators. | Granted by object owners. |
| Apply to the entire system. | Apply to specific objects. |
| Used to permit/prevent DDL statements. | Used to permit/prevent DML statements. |
| Allow managing database and servers. | Allow performing actions on database objects. |

---

### **Syntax for Privileges**
- **Granting System Privilege:**  
  ```sql
  GRANT CREATE SESSION TO user1;
