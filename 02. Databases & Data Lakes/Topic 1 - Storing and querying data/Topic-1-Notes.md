# Topic 1: Topic 1 - Storing and querying data

## Prepare E-Learning:

1. Falling storage costs allow SJP to retain and analyse larger amounts of data, improving decision-making, identifying business trends and increasing operational efficiency across departments.
2. HDFS, key-value stores and Parquet offer different ways to store and access data, and using them appropriately at SJP could improve data accessibility, processing efficiency and analytical capabilities, although each has different limitations depending on the use case.
3. For the Data Control Tower Power BI observations I do at SJP, Parquet could efficiently store structured data for analysis and reporting, while key-value stores could enable quick access to individual data quality records; I could seek further insights from the data engineer or stakeholder responsible for the Data Control Tower.
4. For a data migration project at SJP, a data lake could store raw data from multiple sources, a data warehouse could organise it for reporting and analysis, and an ODS could provide up-to-date operational data; I could seek further insight from a data engineer or solution architect.
5. SJP manages multiple relational databases across its systems, and improving how customer and financial data is structured through normalisation could reduce duplication, improve data quality and support more accurate reporting; I could discuss potential improvements with a data engineer or the data platform team
6. SJP primarily uses cloud-based storage to manage sensitive customer, financial and business data; a hybrid cloud approach could improve scalability, accessibility and flexibility while maintaining security and regulatory compliance, although it introduces additional costs and security considerations, which I could discuss with a data engineer or IT architect.

## Apply Task
### Screenshots of my Database and Schema, Defined normalised tables with primary/foreign keys, Defaults and Checks, Seed reference data, Sanity checks to verify constraints 
<img width="1861" height="890" alt="image" src="https://github.com/user-attachments/assets/39f587ce-e9ee-45c2-8007-4dca79e997d9" />

<img width="1891" height="801" alt="image" src="https://github.com/user-attachments/assets/e5eb21a7-1301-48fc-a397-fb421f1faaa6" />

### Review Questions:
1. Business rules: CHECK makes sure values are valid, UNIQUE stops duplicates (like email addresses), and FOREIGN KEY makes sure records link to something that exists. Keeping these in the database helps prevent incorrect data being entered.
2. Defaults: Columns like created_at and marketing_ok have defaults. This means they automatically get a value if one isn't provided, reducing missing data and making things more consistent.
3. Soft deletes: I would change the customer table by adding a deleted_at column. Instead of permanently deleting a customer, we could mark them as deleted by setting a date. This means their data is still stored but can be excluded from normal queries.

