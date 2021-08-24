# COVID 19 Must knows ... Coronavirus Pandemic Playbook


## Presentation Name	Presenter Name	        University/College of Boot Camp	  Program
## COVID 19 Must knows	DINAH Essilfie-Bondzie	George Washington University	  Data Analytics


## Module 20 --- Project Group 4 --- George Washington / Trilogy Data Analysis Bootcamp


# Demo Day this Wednesday, August 25:  Boot Camp Participant
# Data Analysis
# Dinah Bondzie



## Situation

We were at the end of the 6 months of Data Analysis Boot Camp and we knew we would have to work on a 
Group Project.  The course instructor put us in groups of 6 and in breakout rooms, in the zoom class.
The assignment in the breakout room was to:

1. 	Decide on your overall project
	-	We decided on: Coronavirus Pandemic Playbook

2. 	Select your question
	-	What is the population per state at the beginning and end of the pandemic?
	-	How has race played a role in the spread of the COVID-19 pandemic?
	-	Could the level of poverty and inequality affect the spread of COVID-19?
	-	Did having medical insurance play a role in the cure and deaths?
	-	During periods of Covid-19 case spikes, were there geographical or state areas that trended with these spikes?
	-	Did political affiliation of areas have an influence on the number of Covid cases prior to vaccine distribution?
	NOTE: We knew that the questions may change over the course of the project.


3. 	Share this decision with the class
	-	In the breakout room, the instructor picked out our group leader, who presented our project decition to the class
	`	We created a GitHub Ripository for the group




## Task



1.	Selected topic Reason 
	-	Coronavirus Pandemic Playbook
	`	To measure the response to the infectious diseases COVID19
	`	Target Variable: number of COVID-19 Cases / State Population
	`	To determine which social, economic, and political factors contributed to the spread of COVID-19
	-	Machine learning algorithm to predict which factors contributed the most to the spread of respiratory diseases like COVID-19


2.	Description of the source of data 
	-	Data from CDC and U.S. Census
	-	Social Factors: Sex, Age, Race, Religion
	-	Geographical Factors: Population Density, Number of Commercial Airports, State Land Area, Economic Factors
	-	Median Household Income
	-	Political Factors: State Mandates COVID-19 rules, Political Leaning, 
	-	Lifestyle Factors: Health Insurance Coverage, Exercise Frequency, Social Inclusivity, Work Life Status, Monetary Stability
	-	U.S. Census Data from January 2020 to December 2021: [https://www.census.gov/data/developers/data-sets.html]
	-	US State Data: [https://covidtracking.com/data/download]
	-	CDC Data from January 2020 to December 2021: [https://data.cdc.gov/Case-Surveillance/COVID-19-Case-Surveillance-Public-Use-Data-Profile/xigx-wn5e)


3.	Questions hoped to answer with the data
	-	Which social, economic, geographical, lifestyle or political factors contributed the most the spread of the disease?
	-	Which category of factor contributed the most to the spread of the disease?
	-	Is there a connection between state policy or political leaning (i.e. mask mandate) and the spread of COVID-19 within the state
	-	Do we need to account for the size of the population that didn't have COVID-19 when using a machine learning model?


4.	GitHub Repository
	-	Group GitHub Ripository: [https://github.com/dwwatson1/coronavirus_pandemic_playbook]
	-	Group GitHub Resouse branch: [https://github.com/dwwatson1/coronavirus_pandemic_playbook/tree/main/Resources]
	-	Group Github Image branch: [https://github.com/dwwatson1/coronavirus_pandemic_playbook/tree/main/Images]
	-	Group Github Javacript branch: [https://github.com/dwwatson1/coronavirus_pandemic_playbook/tree/main/Script]
	-	Group GitHub Static branch: [https://github.com/dwwatson1/coronavirus_pandemic_playbook/tree/main/Static/JS]


5.	The main branch should include: README.md
	-	Group Github ReadME file: [https://github.com/dwwatson1/coronavirus_pandemic_playbook/blob/main/README.md]


6.	The README.md should include: Description of the communication protocols, Individual Branches.
	[https://github.com/dwwatson1/coronavirus_pandemic_playbook/blob/main/README.md]
	Technologies Used
	-	Database Storage: pgAdmin - PostgreSQL, AWS RDS
	-	Data Cleaning and Analysis: Juypter Notebook - Pandas
	-	Machine Learning Model: Google Collab Notebook
	-	Presentation of Findings: Tableau Public, GitHub
	Communication Protocol 
	-	Slack Group where we had consistent communication
	-	Zoom meetings
	-	Project Checklist
	-	Group meeting agendas: [https://drive.google.com/drive/folders/1sMOLvKQO-S99917fQL9axuocZujgKNZQ]
	-	Breakout Rooms during BootCamp Zoom Class


7.	Requirements for the individual branches follow: 
	-	At least one branch for each team member
	-	Group Github Individual branches: [https://github.com/dwwatson1/coronavirus_pandemic_playbook]


8.	Machine Learning Model

	The model we chose to use is a supervised random forest regression model. 
	We chose supervised machine learning because we have labeled data (our features in tabular form) and outputs. 
	The input data, or our features, has a paired outcome which is plugged in to train the model to predict outcomes. 
	Supervised machine learning models have target variables, or dependent variables, about which we want to gain a deeper understanding. 
	In our case our target variable is how much effect COVID had on a state's population by looking at the total number of COVID cases divided by the total state population.

	We chose a random forest algorithm because it can handle many input variables of which we have many. 
	The algorithm can run efficiently on large datasets, and most importantly, random forest models can be used to rank the importance of input variables. 
	This fits the question we are trying to answer perfectly: What are the top factors that influence the spread of COVID? 
	A random forest model will help us rank the most influential factors. 
	Since we have a large dataset with many features, as well as both continuous and categorical non-linear variables, a random forest algorithm will be more efficient and more accurate than a simple linear regression. While a large number of trees in a random forest algorithm can be slow requiring a lot of computational power and resources, the advantages outweigh the disadvantages.


9.	Takes in data from the provisional database, Outputs label for input data
	ERD of CDC Data, aggregated for Total per State and for ratio against square miles. and against Census Data
	-	[https://github.com/Dybondzy/COVID_Data_Analysis/blob/main/COVID_MARCH2020_DEC2020_PROJECT4%20ERD.png]
	ERD of CDC Data, aggregated by State, Age Group, Race, and Sex
	-	[https://github.com/Dybondzy/COVID_Data_Analysis/blob/main/COVID_MARCH2020_DEC2020_PROJECT4_CDC%20ERD.png]
	The State Data
	-	[https://github.com/dwwatson1/coronavirus_pandemic_playbook/blob/main/Resources/STATES.csv]
	The options of Age Group
	-	Age group: 0 - 17 years, 18 to 49 years, 50 to 64 years, 65+ years 
	-	[https://github.com/Dybondzy/Covid_19_Pandemic_Must_Know/blob/main/AGE_GROUP.csv]
	
	The options if Race
	-	Race: Black, White, Asian, Multiple/Other, American Indian/Alaska Native, Native Hawaiian/Other Pacific Islander, any possible Unknown 
	-	[https://github.com/Dybondzy/Covid_19_Pandemic_Must_Know/blob/main/RACE.csv]

	The options if Sex
	-	 Sex: MALE, FEMALE 
	-	[https://github.com/Dybondzy/Covid_19_Pandemic_Must_Know/blob/main/SEX.csv]


10.	Database Integration
	CDC Data downloaded in Colab and intergrated into PostgreSQL in PGAdmin
	-	[https://github.com/Dybondzy/COVID_Data_Analysis/blob/Resources/cdc_db_cleaned_part1.zip],
	-	[https://github.com/Dybondzy/COVID_Data_Analysis/blob/Resources/cdc_db_cleaned_part2.zip], 
	-	[https://github.com/Dybondzy/COVID_Data_Analysis/blob/Resources/cdc_db_cleaned_part3.zip], 
	-	[https://github.com/Dybondzy/COVID_Data_Analysis/blob/Resources/cdc_db_cleaned_part4.zip]

	Cencus Data downloaded in Colab and intergrated into PostgreSQL in PGAdmin
	-	Data on agegroup
	-	[https://github.com/Dybondzy/COVID_Data_Analysis/blob/Resources/census_age_no_covid.csv] 
	-	Data on the sex
	-	[https://github.com/Dybondzy/COVID_Data_Analysis/blob/Resources/census_sex_no_covid.csv]
	-	Data on number of airports in the states, the state land area in square miles, and the airport area ration to the land area 
	-	[https://github.com/Dybondzy/COVID_Data_Analysis/blob/Resources/Group4%20Airport%20By%20Area.csv]
	-	Data on the average income of each state 
	-	[https://github.com/Dybondzy/COVID_Data_Analysis/blob/Resources/household_income_by_state.csv]
	-	Data per state on political and social issues: 
	-	[https://github.com/Dybondzy/COVID_Data_Analysis/blob/Resources/state_factors_from_gallup.csv]


11.	Team members will be expected to present a provisional database that stands in for the final database
	-	We agreed that 2 group members, one who managed our group GitHub repository and another who worked on the machine learning, to do the presentation


12.	Sample data that mimics the expected final database structure or schema
	-	The output data from PostgresQL in PGAdmin, used in our analysis
	-	[https://github.com/Dybondzy/COVID_Data_Analysis/blob/Resources/COVID_MARCH2020_DEC2020_TOTALS_PROJECT4.csv]


13.	Draft machine learning model is connected to the provisional database
	-	The supervised random forest regression model as I would explain it
	-	[https://github.com/Dybondzy/COVID_Data_Analysis/blob/Resources/Copy_of_COVID_19_Final_Analysis.ipynb]
	-	The supervised random forest regression model as presented as a group
	-	[https://github.com/Dybondzy/COVID_Data_Analysis/blob/Resources/covid_ml.ipynb]
	-	[https://github.com/Dybondzy/COVID_Data_Analysis/blob/Resources/covid_ml_ratios.ipynb]
	-	The Extra Mile
	-	States Dropped because insufficient data: Michigan, Missouri, Kentucky, Rhode Island, South Dakota, Texas, West Virginia

14.	Dashboard


## Assignement

### Roles
#### Project Manager
David
Database Storage
Dinah
Kimi
Michael
#### Data Cleaning and Analysis
Dinah
Kimi
Michael
#### Machine Learning Model
Michael
#### Presentation of Findings
Yodit (Tableau)
Jack (Tableau)
David (approver) & Team (GitHub)
#### Technologies Used
Database Storage
pgAdmin - PostgreSQL
AWS RDS
#### Data Cleaning and Analysis
Juypter Notebook - Pandas
Machine Learning Model
Google Collab Notebook
#### Presentation of Findings
Tableau Public
GitHub
#### The Extra Mile
Michael and David added to out Machine Learning Model
	-	States Dropped because insufficient data: Michigan, Missouri, Kentucky, Rhode Island, South Dakota, Texas, West Virginia
	-	Recreated Data
	-	[https://github.com/dwwatson1/coronavirus_pandemic_playbook/blob/main/script/no_covid_states.ipynb]
	


## Results
	
Group Interpretaion
	-	Accuracy:
	-	[https://github.com/dwwatson1/coronavirus_pandemic_playbook/blob/main/Resources/accuracy_ratio2.PNG]
	-	[https://github.com/dwwatson1/coronavirus_pandemic_playbook/blob/main/Resources/accuracy_ratio.PNG]
	-	[https://github.com/dwwatson1/coronavirus_pandemic_playbook/blob/main/Resources/accuracy.PNG]
	-	Results:
	-	[https://github.com/dwwatson1/coronavirus_pandemic_playbook/blob/main/Resources/results_ratio2.PNG]
	-	[https://github.com/dwwatson1/coronavirus_pandemic_playbook/blob/main/Resources/results_ratio.PNG]
	Data Analysis Results Interpretation on Totals
	-	 (0.44178714821782483, 'covid_age_goup_0_17'),
	-	 (0.07412533360663463, 'POPULATION_DENSITY'),
	-	 (0.0737820324643414, 'covid_no_race'),
	-	 (0.0006129858713567292, 'number_dont_eat_produce_frequently'),
	-	 (0.0004490797066645125, 'number_moderates'),
	-	 (0.0003891074311076836, 'number_insured')
	-	 Which implies to me that Covid19 was spread most by the age group 0 to 17and in densly populated areas
	-	 That record keepers didn't find it necesary to record the race of Covid19 patients
	-	 Covid19 was spread the least among produce eaters, and moderates and those insured 






### SQL work done
[https://github.com/Dybondzy/COVID_Data_Analysis/blob/Resources/Project%204%20Database%20SQL_steps.txt]


