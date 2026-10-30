# Topic 4: Introduction to reliable data architectures

## What is an Architecture Diagram?
- Explains the abstract idea for your system
- How stakeholders will interact with it
- The constraints of the system
- Is often drawn as layers

## What is a Design Diagram?
- Normally does not have stakeholders, constraints or layers
- Focuses on one part of the system and shows its building blocks

## What is a Data Lake?
A data lake is a centralized repository designed to store vast amounts of raw data in its native format, whether structured, semi-structured or unstructured. This approach allows organizations to ingest data from diverse sources without the need for immediate transformation, making it ideal for big data analytics, machine learning and real-time monitoring.

## What is a Data Warehouse?
A data warehouse is a centralized relational database that stores structured and processed data, optimized so organizations can query and analyze data efficiently for  business intelligence. It integrates data from various operational systems, providing a unified view for business intelligence, reporting and decision support.

## What is a Data Mart?
A data mart is a focused subset of a data warehouse, tailored to serve the specific needs of a particular business unit, department or user group. By concentrating on a single subject area, data marts provide streamlined access to relevant data, enhancing performance and user autonomy.

## Different Flowchart shapes and their meaning:


<img width="858" height="314" alt="image" src="https://github.com/user-attachments/assets/edd46908-8231-4b8a-b044-ee375da2cdcb" />


## Collaborate activity 

Scenario:  NextGen Fitness is a company that provides personalised fitness tracking and coaching services through a mobile app and wearable devices.  The system collects data from the wearable devices, stores it in a database, and uses machine learning algorithms to provide personalised coaching advice to users.  The system also allows users to connect with personal trainers for additional guidance and support.

Instructions: 
- Create a basic flowchart or architecture diagram for the NextGen Fitness system
-  Include the following actors: Users (fitness enthusiasts), Personal trainers, Wearable devices, Mobile app and Machine learning algorithms
-  Include the following containers: User interface, Data storage, Data processing, Personalised coaching module and Personal trainer communication module
-  Show the flow of data and interactions between the actors and containers

My Flowchart built in Lucidchart:

<img width="748" height="848" alt="image" src="https://github.com/user-attachments/assets/871a4527-3642-495b-a114-88bbe8661570" />


## What is TOGAF and why do we use it?
TOGAF (The Open Group Architecture Framework) is a framework used to plan, design, implement and manage an organisation’s IT systems in line with its business goals. It is useful because it provides a common structure and language for different teams to communicate effectively, align technology with business needs and ensure systems work together efficiently.


## Apply Task 1:

I picked Scenario 2 to make a use case diagram via Lucidchart: 

Scenario 2: Financial Institution's Customer Data Platform A large financial institution aims to develop a comprehensive customer data platform to enhance its services and personalise customer experiences. The platform should integrate data from multiple sources, including core banking systems, credit card transactions, investment portfolios, and customer interactions across various channels (e.g., online banking, mobile apps, and branch visits). The system should enable the bank to gain a 360-degree view of each customer, support targeted marketing campaigns, and facilitate risk assessment and fraud detection. 

<img width="1072" height="733" alt="image" src="https://github.com/user-attachments/assets/4a2832e6-b85e-4ffc-bd16-8c9f09bd74e5" />


## Apply Task 2:

### Applying TOGAF Principles to Data Governance During a Matillion-to-dbt Migration.

#### High-level data governance plan:

1. Purpose

The aim of this plan is to maintain data quality and consistency during SJP's migration from Matillion to dbt. TOGAF principles will be used to establish clear responsibilities, standardise processes and ensure migrated data remains accurate and reliable.

2. Governance structure and responsibilities

Data Governance Lead: Oversees governance standards and resolves major issues.

Data Owner: Ensures data meets business requirements and approves its use.

Data Steward: Maintains data definitions, documentation and quality standards.

Data Engineer: Rebuilds Matillion transformations in dbt and carries out data quality tests.

Technical Lead: Reviews the technical implementation and approves deployment.

3. Key governance policies

Data quality: Ensure migrated data is accurate, complete and consistent.

Data ownership: Assign responsibility for each important data asset.

Documentation: Record data definitions, transformations and dependencies.

Change management: Review and test changes before they are implemented.

Issue management: Record and investigate data quality problems before deployment.

4. Decision-making process

Each migrated data model should follow a consistent process:

Identify and document the existing Matillion transformation.

Rebuild the transformation in dbt.

Run data quality tests and compare the results.

Investigate and correct any unexpected differences.

Obtain approval from the Data Owner and Technical Lead.

Deploy the model and monitor its ongoing quality.

Models should not be deployed until the required checks and approvals have been completed.

5. Applying TOGAF

The TOGAF Architecture Development Method (ADM) provides a structured approach to the migration:

Preliminary: Establish governance principles and standards.

Phase A: Define the migration objectives.

Phase B: Identify business requirements and responsibilities.

Phase C: Understand data assets and transformations.

Phase D: Consider the technology supporting the migration.

Phases E–F: Plan and implement governance improvements.

Phase G: Ensure the migration follows agreed standards.

Phase H: Monitor and improve the new environment.

6. Monitoring

The framework should be reviewed regularly by monitoring data quality test results, migration errors, documentation and outstanding issues. This helps ensure that data remains reliable after migration.

#### Visual Representation:

<img width="272" height="769" alt="image" src="https://github.com/user-attachments/assets/9c18d969-46e4-4796-99df-0aca84f8f045" />




