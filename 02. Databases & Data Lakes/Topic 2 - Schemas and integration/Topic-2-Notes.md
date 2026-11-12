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
