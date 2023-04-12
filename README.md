# Food-Security-Data
Data Mining on the 2021 Food Security Data from US Census Bureau. Different classification algorithms are done on unit of observation being individuals within a housing unit. 

Dataset is from https://www.census.gov/data/datasets/time-series/demo/cps/cps-supp_cps-repwgt/cps-food-security.html#cpssupps. Includes population survey, industry classification codes, etc.
Grouped into family attributes and person attributes.

*list of attributes below

HUTYPEA
TYPE A NON INTERVIEW REASON
The reasons why the household is not attending the interview. Ex. 1 no one home 2 temporarily absent
6-5
HRNUMHOU
TOTAL NUMBER OF PERSONS LIVING IN THE HOUSEHOLD
The people in each household. Minimum 0 and maximum 16
6-6
HUBUS
DOES ANYONE IN THIS HOUSEHOLD HAVE A BUSINESS OR A FARM
Yes for business or farm in the household and no for normal employment.
6-8
PRMJIND1
MAJOR INDUSTRY RECODE - JOB 1
Each code represent one major field of industry type. Ex. 1 Agriculture, forestry, fishing, and hunting. 2 Mining
6-64

HEFAMINC 
FAMILY INCOME:
*EXPLANATION HERE* 
It is the combined income of all family members for 12 months. data entries are on a scale of 1-16 with different values. ex. 1 less than $5000, 2 $5000-$7499. 
6-4

HEHOUSUT
TYPE OF HOUSING UNIT:
What kinds of environment is the household living in? Ex. 1 house, apartment, flat 2 hu in nontransient hotel, motel, etc.
 6-3

HRHHID
*HOUSEHOLD IDENTIFIER
A unique identifier for each household (used to group person data into same household)
6-1
PUCHINHH
CHANGE IN HOUSEHOLD COMPOSITION
The number of people in the household. Ex. 1 person added, 2 person added-ure
6-16
PEMLR
MONTHLY LABOR FORCE RECODE
The status of employment. Ex. 1 employed-at work, 2 employed-absent
6-21
PUBUS1
LAST WEEK DID YOU DO ANY UNPAID WORK IN THE FAMILY BUSINESS OR FARM
Unpaid in family business or farm.
6-22
GEREG
REGION
Ex. 1 northeast 2 midwest
6-9
GEDIV 
DIVISION
Ex. 1 New England 2 Middle Atlantic
6-9 
PRNMCHLD
NUMBER OF OWN CHILDREN <18 YEARS OF AGE
 Children in household
6-75
HUPRSCNT 
NUMBER OF ACTUAL AND ATTEMPTED PERSONAL CONTACTS
Number of contacts on a scale of 1-9
6-7  
GTMETSTA 
METROPOLITAN STATUS
Status as whether the city they live in yes 1, no 2, or unidentified 3
6-11 
GTCBSASZ
METROPOLITAN AREA (CBSA) SIZE 
Size of metropolitan in increments 0-7 intervals of 250,000
6-11 

Person Attributes: 

PRTAGE
PERSONS AGE
Actual year in age, generalize 80-84 as 80 and 85+ as 85
6-13
PEMARITL
MARITAL STATUS
Four valid entries for marriage status (including w/ or w/o spouse)
6-13
PESEX
SEX
Binary data for Male (1) and Female (2)
6-14
PEEDUCA
HIGHEST LEVEL OF SCHOOL COMPLETED OR DEGREE RECEIVED
Numeric entries from 31-46 that includes the different highest degree of education completed (less than 1st grade to doctorate degree)
6-14
PUCHINHH
CHANGE IN HOUSEHOLD COMPOSITION
The member changes in the household, the income might change if an adult.
6-16
PEMLR
MONTHLY LABOR FORCE RECODE
7 numeric entries for what status person(s) has in the workforce (working, not working, etc.)
6-21
PUWK
LAST WEEK, DID YOU DO ANY UNPAID WORK IN THE FAMILY BUSINESS OR FARM
5 numeric entries for yes, no, retired, disabled, and unable to work
6-22
PUBUS2OT
DO YOU RECEIVE ANY PAYMENTS OR PROFITS FROM THE BUSINESS
Binary data for Yes (1) and No (2)
6-22
PURETOT
RETIREMENT STATUS
Data entry for whether they are currently retired (1) or not (2)
6-23
PUDIS1
DOES YOUR DISABILITY PREVENT YOU FROM ACCEPTING ANY KIND OF WORK DURING THE NEXT SIX MONTHS
Binary data for Yes (1) and No (2)
6-24
PULAYDT
HAS YOUR EMPLOYER GIVEN YOU A DATE TO RETURN TO WORK
Binary data for Yes (1) and No (2)
6-32
PRCITSHP 
CITIZENSHIP STATUS
5 statuses that include native and foreign born
6-20
PTDTRACE
RACE
26 race entries and combination of races (ex. White-Asian)
6-15
PRMJOCC1 
MAJOR OCCUPATION RECODE - JOB 1
General occupation in 10 different categories from 1-11
6-65

Unit of observation is individuals within housing unit.
Class attribute: HRFS12M1(Household Food Security Scale, 12-Month Reference Period 7-41 )

Classification Algorithms used: Random Forest, IBk, Naive Bayes, OneR, and J48
Attribution selection with Gain Ratio, OneR, Information Gain, Chi square, and Symmetrical Uncertainty

![image](https://user-images.githubusercontent.com/104241091/231598277-7b6993fd-4b46-4b85-9d34-401d97bb90ff.png)

Results

![image](https://user-images.githubusercontent.com/104241091/231598433-40a0cf5e-0af6-408a-83ff-785a3d0b66d1.png)

![image](https://user-images.githubusercontent.com/104241091/231598502-706e49e1-5bd1-4f34-abb5-46135bd880ea.png)





