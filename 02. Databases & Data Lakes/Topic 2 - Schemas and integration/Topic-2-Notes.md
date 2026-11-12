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
