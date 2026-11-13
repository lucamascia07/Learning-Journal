#  Topic 2 - Schemas and integration

## Prepare E-Learning:

A Primary key is a unique identifier for records in a table. No two records can have the same primary key.

A Foreign key is fields in a table that match the primary key of another table, creating a link between the two tables.

### Snowflake

At work, the main database platform I use is Snowflake. Snowflake is a cloud-native data platform used for storing, transforming, and analysing large volumes of data. As part of my Data Engineering and Analytics apprenticeship, I use Snowflake in conjunction with dbt to build and test data models, investigate data quality rules, and support reporting and analytics activities. This has given me practical experience of working with data in a modern cloud environment.

Snowflake is not an open-source database. It is a proprietary platform developed and maintained by Snowflake Inc., with organisations paying for the storage and computing resources they consume. Despite not being open source, it integrates with many open-source and third-party tools commonly used in data engineering.

Snowflake is a cloud-based platform rather than an on-premise database. Within my organisation, Snowflake is hosted on Amazon Web Services (AWS), which allows data to be stored and processed without the need for physical database servers managed by the company and allows SJP to scale storage and computing resources independently and avoid maintaining physical database servers.

Internal training has been accessible during my apprenticeship for example having access to learning materials like Snowflake warehousing courses provided to me by my rotation manager for Data Engineering, Snowflake/Openflow workshops and webinars, LOTS of documentation via confluence, and guidance from senior colleagues.

## Webinar Notes:

### What is a Star Schema?
A database structure in which a central fact table is surrounded by dimension tables, resembling a star. The fact table contains measurable quantities and foreign keys from dimension tables that describe the data's context. Star schemas typically offer faster query performance for large datasets due to fewer joins.

### What is a Snowflake Schema?
An extension of the star schema where dimension tables are normalized into multiple related tables, resulting in a more complex database structure that resembles a snowflake with branches radiating from a central node. Snowflake schemas provide higher data integrity through normalization, which can simplify maintenance and reduce errors.

### Database Normalisation Report:
Database normalisation organises tables to reduce duplicate data and prevent errors. The progression from First Normal Form (1NF) to Third Normal Form (3NF) builds a clean, reliable structure for storing information.

First Normal Form (1NF) means there must be no attribute that contains more than a single value or no repeating values. Its main advantage is eliminating messy lists inside cells so searching is easy, though it still allows heavy data repetition across rows.

Second Normal Form (2NF) needs to be in 1NF and doesn't have any partial dependencies. In other terms, it cannot have different attributes depending on different parts of the composite key—it has to be the whole key. This reduces duplication by splitting data into linking tables, though it still overlooks indirect links between non-key columns.

Third Normal Form (3NF) needs to be in 2NF and contains no non-key or transitive dependencies. It is where a field relies on another field instead of the primary key. This ensures high data integrity because every fact is stored in one place, though joining multiple tables together can slightly slow down read queries.

In conclusion, Third Normal Form (3NF) is the best choice for most everyday applications. It provides the best balance between preventing data errors and keeping table structures manageable.

### SQL Building Blocks

SQL commands are divided into five main categories:

- **DDL (Data Definition Language)** – Defines and manages the structure of database objects, such as tables and schemas.
  - `CREATE` – Creates new database objects.
  - `ALTER` – Modifies existing database objects.
  - `DROP` – Deletes database objects.
  - `TRUNCATE` – Removes all records from a table while retaining its structure.

- **DML (Data Manipulation Language)** – Used to modify the data stored within database tables.
  - `INSERT` – Adds new records.
  - `UPDATE` – Modifies existing records.
  - `DELETE` – Removes records.

- **TCL (Transaction Control Language)** – Manages transactions to ensure database operations are handled correctly.
  - `COMMIT` – Saves changes made during a transaction.
  - `SAVEPOINT` – Creates a point within a transaction that you can roll back to.
  - `ROLLBACK` – Reverses changes made during a transaction.

- **DQL (Data Query Language)** – Used to retrieve and query data from database tables.
  - `SELECT` – Retrieves data, often using filters (`WHERE`), sorting (`ORDER BY`) and grouping (`GROUP BY`).

- **DCL (Data Control Language)** – Manages user access and permissions within a database.
  - `GRANT` – Gives users permissions to access or modify database objects.
  - `REVOKE` – Removes previously granted permissions.


### SQL Standards and Database Comparison

Different database systems use SQL, but each has its own variations and extensions. This means SQL queries may need changing when moving applications between database systems.

- **Amazon Redshift:** Uses a PostgreSQL-derived SQL dialect but has differences and is optimised for analytical queries and large datasets (OLAP). It is highly scalable and uses pay-as-you-go pricing, making it suitable for data warehousing.

- **PostgreSQL:** Has strong SQL standard support and offers a wide range of features. It is open-source and free to use, highly scalable and suitable for general-purpose applications. Its flexibility makes it a popular choice for developers.

- **MySQL:** Supports standard SQL but also has its own extensions and SQL modes. It is open-source and generally cost-effective, making it popular for web applications. Some queries may need adjusting when moving to other database systems.

- **Microsoft SQL Server:** Uses T-SQL (Transact-SQL), which extends standard SQL with additional Microsoft-specific features. It is designed for enterprise environments and handles mixed workloads well. Licensing can make it more expensive, although free editions are available.

### Implications and Conclusion

The main consideration when choosing a database is balancing performance, scalability and cost against the application's requirements. Differences in SQL syntax can make migrating between systems more difficult, meaning developers need to consider compatibility when building applications. Database administrators also need to manage permissions, performance, maintenance and configuration.

Overall, PostgreSQL and MySQL are good cost-effective options for general applications, whereas Redshift is better suited to large-scale data warehousing and SQL Server is commonly used in enterprise environments.
   



