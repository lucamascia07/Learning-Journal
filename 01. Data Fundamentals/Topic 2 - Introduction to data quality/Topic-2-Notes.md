# Topic 2: Introduction to Data Quality

## Fair stands for:
- Findable
- Accessible
- Interoperable
- Reusable


## The data quality metrics are:
- Accuracy - How well does the data reflect the real world and are there  any false items
- Inegrity - How well does the data cover the real world and are there any missing items
- Consistency - How well does the data conform to a single standard and are there discrepancies 
- Timeliness - How up to date is the data
- Reliability - Can it overall be depended on to make decisions


## Apply Task 1 IBM HR Analytics dataset from Kaggle Questions and Tasks:

### a. What is the usability score of this dataset and is it “good” or “bad”?

It is 8.82 which is a good rating.

### b. How is this usability score calculated?

It is calculated by Kaggle based off 3 main sections of competness credibility and compatibility and within them it has checklists and will take an overall percentage of them. They are: 
Completeness 
Subtitle
Tag
Description
Cover Image

Credibility 
Source/Provenance
Public Notebook
Update Frequency

Compatibility 
License
File Format
File Description
Column Description

### c. What are the two credibility issues with this dataset and why are they important?

It is Source/Provenance and Update Frequency that are being flagged. Source and provenance is important to give an understanding of the data's origin to understand how trustworthy and accurate it is and trace back any potential errors. Update frequency is important to make sure there isn't any outdated data and it may suggest that there is incomplete data or it may not be relevant due to it not being updated regularly. It also could signal a lack of active maintenance of the dataset.

### d. How many columns does this dataset have?

It has 35 columns being Age, Attrition, BusinessTravel, DailyRate, Department, DistanceFromHome, Education, EducationField, EmployeeCount, EmployeeNumber, EnvironmentSatisfaction, Gender, HourlyRate, JobInvolvement, JobLevel, JobRole, JobSatisfaction, MaritalStatus, MonthlyIncome, MonthlyRate, NumCompaniesWorked, Over18, OverTime, PercentSalaryHike, PerformanceRating, RelationshipSatisfaction, StandardHours, StockOptionLevel, TotalWorkingYears, TrainingTimesLastYear, WorkLifeBalance, YearsAtCompany, YearsInCurrentRole, YearsSinceLastPromotion and YearsWithCurrManager

### e. What is the licence for this dataset and how would you summarise the usage rights in your own words?

The licence is the Database Contents License (DbCL) v1.0, published by Open Data Commons. It allows you to use, copy and modify the datasets contents including for commercial purposes provided you follow the conditions of the license 


MD5 in the dataset stands for message-digest algorithm 5 and it is used to generate a short digital fingerprint from data. Can be useful to see if data has changed or not and if comparision between MD5 is the same it hasn't changed

### Why does using compression aid sustainability and net-zero goals?
It aids it by reducing the amount of storage space used on servers and the amount of data being transferred across the internet. This reduces bandwidth usage and reduces the amount of phyiscal storage you need as well as energy needed for the storage

### What is the possible issue in identifying the meaning of the column named 'YearsSinceLastPromotion', especially when interpreting the value of '0' in one of the fields?
Column name is unclear as it could mean if it is 0 that someone has never been promoted or they were promoted in this current year.

### Compare the contents of the column 'Over18' and 'OverTime', what data quality issue can you identify?
Answer format isn't standardised with there being Y and N or Yes and No so could cause issues when comparing and making queries from it.

### What are some possible issues with the data quality of 'MonthlyIncome' and 'Monthly Rate'?
There could be missing values or duplicate values and mainly just confusion around the unclear name of Monthly Rate

### How would you validate the 'EmployeeNumber' column and what needs paying special attention to?
I would validate it by checking they are all numeric , unique and not NULL and in particular if there are any duplicate values.

I completed the remaining tasks by preparing the IBM HR Analytics dataset in Excel, retaining only the EmployeeNumber and JobSatisfaction columns. I added Metadata, Schema and Provenance sheets to document the dataset and its structure. I have uploaded the file to the learning journal. Excel file name: Employee Job Satisfaction Dataset.

### This task helped me build on the following KSB'S.:

Knowledge

K4: Frameworks for data quality, covering dimensions such as accuracy, completeness, consistency, timeliness, and accessibility.

K5: The inherent risks of data such as incomplete data, ethical data sources and how to ensure data quality.

K7: Principles of sustainable data products and organisational responsibilities for environmental social governance.

K11: Data and information security standards, ethical practices, policies and procedures relevant to data management activities such as data lineage and metadata management.

K16: Principles of data, including open and public data, administrative data, and research data including the value of external data sources that can be used to enrich internal data.

Skills

S5: Produce and maintain technical documentation explaining the data product, that meets organisational, technical and non-technical user requirements, retaining critical information.

S6: Systematically clean, validate, and describe data at all stages of extract, transform, load (ETL).

S26: Identify data quality metrics and track them to ensure the quality, accuracy and reliability of the data product.

Behaviours

B3: Quality focus that promotes continuous improvement utilising peer review techniques, innovation and creativity to the data system development process to improve processes and address business challenges.

B4: Takes personal responsibility towards net zero and prioritises environmental sustainability outcomes in how they carry out the duties of their role.

## Apply Task 2 

<img width="943" height="1000" alt="image" src="https://github.com/user-attachments/assets/ae38091d-567f-482d-ba26-58d08599c2a0" />

Arrange a shadowing session with a data engineer or a subject matter expert in your organisation to observe how they leverage automated data quality management tools in their workflow.

Gain info on: 

Specific use cases and scenarios where automated data quality management tools are employed
Benefits and challenges of using these tools
Integration with existing data pipelines or workflows
Utilise internal resources like wikis, documentation, and knowledge bases to gather insights on automated data quality management within your organisation



