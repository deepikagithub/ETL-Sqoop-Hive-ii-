# ETL-Sqoop-Hive-ii-
The project mainly revolves around Apache Sqoop and Apache Hive 
India Annual Health Survey (AHS) 2012-13

 

The dataset comprises a survey conducted in Empowered Action Group (EAG) states Uttarakhand, Rajasthan, Uttar Pradesh, Bihar, Jharkhand, Odisha, Chhattisgarh & Madhya Pradesh and Assam. These nine states, which account for about 48 percentage of the total population, 59 percentage of Births, 70 percentage of Infant Deaths, 75 percentage of Under 5 Deaths and 62 percentage of Maternal Deaths in the country, are the high focus States in view of their relatively higher fertility and mortality.

 

A representative sample of about 21 million population and 4.32 million households were covered which is spread across the rural and urban area of these 9 states.

 

The objective of the AHS is to yield a comprehensive, representative and reliable dataset on core vital indicators including composite ones like Infant Mortality Rate, Maternal Mortality Ratio and Total Fertility Rate along with their covariates (process and outcome indicators) at the district level and map the changes therein on an annual basis. These benchmarks would help in better and holistic understanding and timely monitoring of various determinants on well-being and health of population particularly Reproductive and Child Health. [Source]

 

Content

 

This dataset contains the data about the below 26 key indicators.

Problem Statement
Ingest the India Annual Health Survey (AHS) 2012-13 data hosted on Amazon RDS into Hadoop correctly and process it to generate the following analyses:

 

Analyses

State wise child mortality rate
State wise fertility rate
Does high fertility correlate with high child mortality?
Find top 2 districts per state with the highest population per household
Find top 2 districts per state with the lowest sex ratios
Such analyses would help in vivid understanding and timely monitoring of different determinants on well-being and health of population particularly Child and Reproductive Health.

 

Guidelines
Ingest data from Amazon RDS to HDFS using Sqoop.

Create an external table in Hive for the ingested data containing all the columns as given in this document. Ingest the data from HDFS to the Hive table. Verify that the ingestion is successfully accomplished.
Create a subset schema in Hive to store the data for the analyses to be done. The schema should be optimized to support ONLY the analyses to be done. You will be graded on your choice of the chosen columns, storage format (Parquet, RC, ORC, CSV), etc. Benchmark the performance of the storage formats before finalizing the one to be used.
Write queries against each category of analyses. Generate the corresponding analyses’ charts on Hue.
