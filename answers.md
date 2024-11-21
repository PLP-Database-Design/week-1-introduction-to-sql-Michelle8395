# Components of a Database Management System (DBMS)

A **DBMS** consists of several components that work together to manage and control access to databases. The main components include:

- **Database Engine**: The core component of the DBMS that manages how data is stored, retrieved, and updated in the database.
- **Database Schema**: The structure of the database, including tables, relationships, and constraints.
- **Query Processor**: Interprets and processes SQL queries, translating them into executable commands.
- **Transaction Manager**: Ensures that database transactions are executed in a way that guarantees the ACID properties (Atomicity, Consistency, Isolation, Durability) for data integrity and reliability.
- **Database Manager**: Handles the management of database objects, including tables, indexes, and views, and ensures efficient data storage.
- **Data Dictionary**: A repository that contains metadata about the database schema, describing the structure of the data, relationships, constraints, etc.
- **User Interface**: Provides an interface for users and administrators to interact with the DBMS. This can be a graphical user interface (GUI) or a command-line interface.

---

# What is a Relational Database? Give 4 Examples

A **relational database** is a type of database that stores data in tables, which are composed of rows (records) and columns (fields). Each table represents a different entity type, and the relationships between the entities are maintained through keys (primary and foreign keys).

Examples of **relational databases** include:
1. **MySQL**
2. **PostgreSQL**
3. **Microsoft SQL Server**
4. **Oracle Database**

---

# State and Explain Three Classifications of SQL

1. **Data Query Language (DQL)**:
   - Used to query the database and retrieve data. The primary command is `SELECT`.
   - Example: `SELECT * FROM employees;`

2. **Data Definition Language (DDL)**:
   - Used to define, modify, or delete database objects like tables, schemas, and indexes.
   - Examples: `CREATE`, `ALTER`, `DROP`
   - Example: `CREATE TABLE employees (id INT, name VARCHAR(100));`

3. **Data Manipulation Language (DML)**:
   - Used to insert, update, delete, or retrieve data from tables.
   - Examples: `INSERT`, `UPDATE`, `DELETE`
   - Example: `INSERT INTO employees (id, name) VALUES (1, 'Alice');`

---

# What is the Difference Between a Primary Key and a Foreign Key?

- **Primary Key**:
  - A **primary key** is a unique identifier for each record in a table. It ensures that each row in the table is unique and cannot have `NULL` values.
  - Example: In a table of employees, the `employee_id` field might be the primary key.

- **Foreign Key**:
  - A **foreign key** is a field in a table that creates a relationship between the data in two tables. It refers to the primary key of another table and ensures referential integrity.
  - Example: In an `orders` table, the `customer_id` might be a foreign key that refers to the `customer_id` in the `customers` table.

---

# What is an Entity-Relationship Diagram?

An **Entity-Relationship Diagram (ERD)** is a visual representation of the entities (tables) in a database and the relationships between them. It shows how data is structured and connected, helping in designing and organizing the database schema.

- **Entities** are represented as rectangles (tables).
- **Relationships** are represented as diamonds.
- **Attributes** are represented as ovals (columns).

ERDs are used in database design to ensure that relationships are defined correctly before creating the database.

---

# Advantages of Relational Databases

1. **Data Integrity**:
   - Relational databases maintain data consistency through constraints like primary keys, foreign keys, and unique constraints.

2. **Flexibility**:
   - You can query the database in various ways using SQL, providing flexibility in retrieving and manipulating data.

3. **Normalization**:
   - Data is normalized to reduce redundancy, ensuring that each piece of data is stored only once, making the database more efficient.

4. **Security**:
   - Relational databases support user access control and data encryption to protect sensitive information.

5. **Scalability**:
   - Relational databases can scale to handle large volumes of data and transactions, especially with optimization techniques and indexing.

---

# Four Types of Data Types Used to Store Data in Tables

1. **Integer** (`INT`):
   - Used to store whole numbers without decimals.
   - Example: `age INT`

2. **Varchar** (`VARCHAR`):
   - Used to store variable-length strings.
   - Example: `name VARCHAR(100)`

3. **Date/Time** (`DATE`, `TIME`, `DATETIME`):
   - Used to store dates and times.
   - Example: `birthdate DATE`

4. **Float/Double** (`FLOAT`, `DOUBLE`):
   - Used to store floating-point numbers (numbers with decimals).
   - Example: `price FLOAT`

---

# Purpose of a Database Management System (DBMS)

The primary purpose of a **DBMS** is to provide an interface between users and the database, ensuring efficient data storage, retrieval, and management. The DBMS handles the complexities of storing large amounts of data while providing users with an easy-to-use interface for interacting with that data.

- **Key Functions**:
  - **Data Storage**: Efficiently stores and manages large amounts of data.
  - **Data Retrieval**: Allows users to query and retrieve data.
  - **Data Security**: Ensures that data is secure from unauthorized access.
  - **Data Integrity**: Maintains the correctness and consistency of the data.
  - **Concurrency Control**: Manages simultaneous access to data by multiple users.
  - **Backup and Recovery**: Ensures data is regularly backed up and can be recovered in case of failures.

The DBMS abstracts the complexities of database management, making it easier for users and developers to interact with data.
