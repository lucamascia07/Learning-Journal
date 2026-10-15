# Data Fundamentals

## Learning Notes

### Topic 1: Fundamentals of the Data-Driven Enterprise
#### The 5 V's of data characteristics are:
- Volume - Sheer size of the data
- Variety - Refers to the different types of data and their sources
- Velocity - Speed at which data is gathered/generated
- Veracity - The reliability and accuracy of the data
- Value - The insights and benifits that can be made from the data

#### Qualative Data includes:
- Binomial - Yes/No
- Nomial - Named data like UK, France, USA
- Ordinal - Has an order such as Small, Medium, Large

#### Quantative Data includes:
- Continuous - Data that is typically measured such as weight, height, distance typically unlimited
- Discrete - Whole numbers that have a limit

#### The three principles of responsible and effective Data Stewerdship are:
- Data Quality
- Data Governance
- Data Ethics

### Topic 2: Introduction to Data Quality

#### Fair stands for:
- Findable
- Accessible
- Interoperable
- Reusable


#### The data quality metrics are:
- Accuracy - How well does the data reflect the real world and are there  any false items
- Inegrity - How well does the data cover the real world and are there any missing items
- Consistency - How well does the data conform to a single standard and are there discrepancies 
- Timeliness - How up to date is the data
- Reliability - Can it overall be depended on to make decisions


#### Apply Task 1:

IBM HR Analytics dataset from Kaggle Questions

a. What is the usability score of this dataset and is it “good” or “bad”?

It is 8.82 which is a good rating.

b. How is this usability score calculated?

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

c. What are the two credibility issues with this dataset and why are they important?

It is Source/Provenance and Update Frequency that are being flagged. Source and provenance is important to give an understanding of the data's origin to understand how trustworthy and accurate it is and trace back any potential errors. Update frequency is important to make sure there isn't any outdated data and it may suggest that there is incomplete data or it may not be relevant due to it not being updated regularly. It also could signal a lack of active maintenance of the dataset.

d. How many columns does this dataset have?

It has 35 columns being Age, Attrition, BusinessTravel, DailyRate, Department, DistanceFromHome, Education, EducationField, EmployeeCount, EmployeeNumber, EnvironmentSatisfaction, Gender, HourlyRate, JobInvolvement, JobLevel, JobRole, JobSatisfaction, MaritalStatus, MonthlyIncome, MonthlyRate, NumCompaniesWorked, Over18, OverTime, PercentSalaryHike, PerformanceRating, RelationshipSatisfaction, StandardHours, StockOptionLevel, TotalWorkingYears, TrainingTimesLastYear, WorkLifeBalance, YearsAtCompany, YearsInCurrentRole, YearsSinceLastPromotion and YearsWithCurrManager

e. What is the licence for this dataset and how would you summarise the usage rights in your own words?

The licence is the Database Contents License (DbCL) v1.0, published by Open Data Commons. It allows you to use, copy and modify the datasets contents including for commercial purposes provided you follow the conditions of the license 


MD5 in the dataset stands for message-digest algorithm 5 and it is used to generate a short digital fingerprint from data. Can be useful to see if data has changed or not and if comparision between MD5 is the same it hasn't changed

#### Why does using compression aid sustainability and net-zero goals?
It aids it by reducing the amount of storage space used on servers and the amount of data being transferred across the internet. This reduces bandwidth usage and reduces the amount of phyiscal storage you need as well as energy needed for the storage

#### What is the possible issue in identifying the meaning of the column named 'YearsSinceLastPromotion', especially when interpreting the value of '0' in one of the fields?
Column name is unclear as it could mean if it is 0 that someone has never been promoted or they were promoted in this current year.

#### Compare the contents of the column 'Over18' and 'OverTime', what data quality issue can you identify?
Answer format isn't standardised with there being Y and N or Yes and No so could cause issues when comparing and making queries from it.

#### What are some possible issues with the data quality of 'MonthlyIncome' and 'Monthly Rate'?
There could be missing values or duplicate values and mainly just confusion around the unclear name of Monthly Rate

#### How would you validate the 'EmployeeNumber' column and what needs paying special attention to?
I would validate it by checking they are all numeric , unique and not NULL and in particular if there are any duplicate values.








