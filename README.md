# hmp-669_final
Group Project Description. *DUE FRIDAY 4/26*

Midwestern Health System (MHS) has recently acquired Omega Hospital.  The MHS Executive Committee would like to include Omega in current contract negotiations with two physician groups (a Cardiac group and an Orthopedic group) for a joint venture that has yet to be clearly defined.  The Executive Committee is concerned that, without a clear understanding of historical utilization and intensity patterns, MHS will be unable to fully assess the impact of potential risk-bearing arrangements for which it is about to accept prospective liability.

Background Information
Attention on Medicare risk contracting, and other provider-based risk arrangements highlight the need and usefulness of the ability to turn a set of historical data into meaningful information via database tools.  The crux of the matter is to identify key quantitative information that enables provider groups and health systems to analyze the potential advantages and disadvantages of signing risk contracts.

Current legislative activity is encouraging providers to enter new risk arrangements and effectively reduce the role of the managed care company - an evolving frontier in healthcare management that demands database and forecasting skills on the part of healthcare managers.  In this case, your data analysis of historical utilization, intensity of care, and other factors will be critical to MHS's decisions regarding potential future joint activities. 

**File Summary**
cleaned_tables.html and cleaned_tables.Rmd: uses dplyr/tidyr functions to clean .csv files
all .csv files: obtained from OMEGA.accb. slightly edited in Excel to minimize coding bandwith (removing extra characters and some whitespace)
financial_viability.html and financial_viability.Rmd: to identify financial viability of cardio and ortho

**TODO:**
Step 1: Identification of data and Data cleaning
1. Identify how to break down the information into Cardiac and Ortho (through Major Diagnosis Category) *DONE*
2. Identify relevant database tables to utilize *DONE*
3. Identify and “scrub” duplicate entries
4. Identify any potential referential integrity issues and resolve
5. Identify and resolve any other potential data cleaning issues
	eg: International Distance, of 65535, can throw off averages (often, very high numbers are used in lieu of missing values)
	ADM_TYPE field “0”
	LOS info on DRG table…not the correct data to use as this data is hard coded and does not relate to admin/discharge info on OMEGA

Step 2: Data Relationships
1. Identify primary keys of all tables
2. Connect all data tables using appropriate relationships (1 to 1, 1 to M, etc.)
3. It will be useful to draw an ERD first prior to using the Access database although an ERD is not required

Step 3: Query Writing
1. Joins of Tables
2. Equations/aggregate functions (ie, Averages, Count, Sums)
3. There are a lot of queries to write to answer all the questions—this part takes the longest

Step 4: Data Extraction & Visualization
1. Import files into csv format
2. R data analysis
3. Graphics 

Step 5: Analysis/Writing
1. ‘Look’ at data and understand what it is telling you
	Ex:  Should demographic analysis be at patient level or visit level? 
       Take a look at costs and profits data.
2. Write-up of case
	a. Answer each question
	b. Additional analyses as necessary to support position taken
	c. Overall recommendation
