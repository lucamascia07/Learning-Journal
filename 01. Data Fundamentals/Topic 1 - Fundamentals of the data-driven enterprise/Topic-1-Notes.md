# Topic 1: Fundamentals of the Data-Driven Enterprise
## The 5 V's of data characteristics are:
- Volume - Sheer size of the data
- Variety - Refers to the different types of data and their sources
- Velocity - Speed at which data is gathered/generated
- Veracity - The reliability and accuracy of the data
- Value - The insights and benifits that can be made from the data

## Qualative Data includes:
- Binomial - Yes/No
- Nomial - Named data like UK, France, USA
- Ordinal - Has an order such as Small, Medium, Large

## Quantative Data includes:
- Continuous - Data that is typically measured such as weight, height, distance typically unlimited
- Discrete - Whole numbers that have a limit

## The three principles of responsible and effective Data Stewerdship are:
- Data Quality
- Data Governance
- Data Ethics

## Topic 1 Apply Task 1 and Topic 2 Apply Task 3
I have completed the task and uploaded the excel file to the learning journal. Here is my email explaining my steps I took to get my clean and usable data. 

Hi,

I've combined the data from Mwanza, Pwani and DSM (Ilala) into one dataset called Data. It includes the region, facility name, facility type, ownership type and star rating. I've also created a Schema sheet explaining the fields and the values used.

The steps I took were:

Combined the three sources into one dataset and removed the extra table headings and serial numbers.

Standardised the facility types, changing HOSP to Hospital, HC to Health Centre and DISP to Dispensary.

Changed Mwanza ownership codes 1 to Public and 2 to Private, based on the source legend.

Changed unclear ownership values, including 0 and ??, to Unknown because the source did not explain them.

Corrected ownership spelling and formatting, including changing PRIVITE to Private.

Set missing Pwani ownership values to Unknown because the source did not provide this information.

Kept the star ratings from 0 to 3 and changed unclear ratings to Unknown.

Checked for repeated facility names and removed records that were identical across all five fields. I kept records where any of the fields differed.

Made the formatting consistent and adjusted the columns so the data is easier to read.

I kept some records that still need checking. For example, Busisi in Mwanza appears as both a Dispensary and a Health Centre, and GWATA has ratings of 0 and 1. I kept both records in these cases because I could not confirm which information was correct.

I have assumed that the ratings can be stored together, but I have not confirmed whether the rating criteria are exactly the same across all three regions. I have also used Unknown where information was missing or unclear rather than guessing.

The cleaned dataset and Schema sheet are ready to review. Please let me know if anything needs further checking.

Kind regards,

Luca Mascia
