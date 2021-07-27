# COVID_Data_Analysis

## Module 20 --- Project Group 4 --- George Washington / Trilogy Data Analysis Bootcamp
The Project Deliverables were in 4 segments

## First Segment: 
Sketch It Out: Decide on your overall project, select your question, and build a simple model. You'll connect the model to a fabricated database, using comma-separated values (CSV) or JavaScript Object Notation (JSON) files, to prototype your idea.

### Project Overview
Our Group 4 has 6 members.  We had our first meeting in a breakout room, in class (on zoom.)  We bainstormed on several topics.  2 of the group members had already discussed crytocurrencies, and a few other topics were discussed.  I have been curious about the effect of the COVID 19 Pandemic and lessons learned, so I suggested this topic.  After some deliberation, everyone had curious questions on the topic, and agreed that we make our topic: Coronavirus Pandemic Playbook.  David went ahead and created a Githud ripository for our group, and we jotted down some questions that we wanted out project to answer.  It was agreed we would like policy makers to use our data to make management decisions if a similar pandemic was to break out.  We also decided to scrape the net for data collection.

### Questions to answer
We agreed and documented the following questions, in the README file in our Github repository:
[https://github.com/dwwatson1/coronavirus_pandemic_playbook]

=  What is the population per state at the beginning and end of the pandemic?
 
=  How has race played a role in the spread of the COVID-19 pandemic?

=  Could the level of poverty and inequality affect the spread of COVID-19? If so what is the impact?

=  Did having medical insurance play a role in the cure and deaths?

=  What were the top 20 uSAs (Micropolitan Statistical Areas) impacted by Covid-19?

=  During periods of Covid-19 case spikes, were there geographical or state areas that trended with these spikes?

=  Did political affiliation of areas have an influence on the number of Covid cases prior to vaccine distribution?
 
NOTE: We knew that the questions may change over the course of the project.

We documented the possible places for data:

[John Hopkins Coronavirus Data](https://coronavirus.jhu.edu/data/new-cases-50-states)

[U.S. Census Data](https://www.census.gov/data/developers/data-sets.html)

[Additional data source that we are considering](https://docs.google.com/document/d/10i01u6oQAUVCbk5VTL6G0rIsTF9JlO1I90XTCDXWTCA/edit)

[Another possible data APIs](https://blogs.mulesoft.com/dev-guides/track-covid-19/)

[A database that we can consider] (https://covidtracking.com/data/download)

(https://data.cdc.gov/Case-Surveillance/COVID-19-Case-Surveillance-Public-Use-Data-Profile/xigx-wn5e)
https://data.cdc.gov/Case-Surveillance/COVID-19-Case-Surveillance-Public-Use-Data-with-Ge/n8mc-b4w4

https://worldpopulationreview.com/states/state-abbreviations (for states)

 
Project Delivery 1 was the above 


--------------------------------------------------


### My Personal work
In order for me to undertand the project scope and the points that have to be covered in the project: 

A. I download summary national covid totals data from cdc
   [https://covidtracking.com/data/download]
   It was data from January 2020 to July 2021
   
B. Used machine learning on Colab, to clean out the data (eliminating some column with very little data)
   [https://github.com/Dybondzy/COVID_Data_Analysis/blob/Resources/Covid_19_Pandemic_Must_Know.ipynb]
   using the csv file: all_states_history.csv
   [https://github.com/Dybondzy/COVID_Data_Analysis/blob/Resources/all_states_history.csv]
   to create the csv file: cleaned_states_history.csv
   [https://github.com/Dybondzy/COVID_Data_Analysis/blob/Resources/cleaned_states_history.csv]
   

C. Used Postgres in PGAdmin to create summmary data and come up with the output csv
   [https://github.com/Dybondzy/COVID_Data_Analysis/blob/Resources/JAN2020_JUL2021_COVIDDEATH_CONTRIBUTERS.csv]
   [https://github.com/Dybondzy/COVID_Data_Analysis/blob/Resources/JAN2020_JUL2021_COVIDDEATH_BYSTATES.csv]
   After joining the data with data on: States in the US from
   [https://worldpopulationreview.com/states/state-abbreviations]
   
D. I went into Tableau and created some graphs
   [https://github.com/Dybondzy/COVID_Data_Analysis/blob/Images/all_states_history_graph.png]
   (with a few more screen prints in the Images folder)


I made sure the following ruberic points were covered:
  -   Python will be used to clean, prepare, and explore the data, as well as to complete initial analysis. 
  -   Python libraries, JavaScript libraries (such as Data-Driven Documents, or D3, and Plotly), and Tableau can be used to create visuals to help tell your data story.
  -   Use database integration (Postgres, MongoDB, or SQLite) to store your cleaned data. 
  -   Implement machine learning to enhance your topic. 
  -   Your work will need a showcase—use tools such as Tableau or JavaScript to build a dashboard to present your results. 

 
 Then I shared the work I had done with the group, calling for discussion.  Reaction called for a zoom meeting (which I quickly scheduled)
 -    Everyone seemed to want to change the data
 -    We searched the net for more data; scraping
 -    We aggreed on CDC data and I downloaded the data while we discussed it
 -    We agreed that our searches have to include US STATES
 -    We updated Github of the search data (David and Kimi updated the sites for data and Michael updated the Machine Learning section)

I used the following Python code to do some more cleaning:
[https://github.com/Dybondzy/COVID_Data_Analysis/blob/Resources/Clean_Covid_19_Pandemic_Data.ipynb]
and came up with this table for analysis:


Reaction: 
Kimi, David, and Michael were upset about the dates used (Jan 2020 to Jul 2020)
They preferred March 2020 to March 2021, and only wanted to work on data on MD
Michael came up with the table: , for our class presentation
Michael and Kimi created / imported a data dictionary into the ReadME file on our group Github repository
Nick commented that the table was too small and had some questions for Michael on the Machine Learning

This is the table we had for presentation of Deliverable 2:

[https://github.com/Dybondzy/COVID_Data_Analysis/blob/Images/MD_CLEANED%20csv%20file.png]
[https://github.com/Dybondzy/COVID_Data_Analysis/blob/Images/MD_CLEANED%20data%20in%20PGADMIN.png]
[https://github.com/Dybondzy/COVID_Data_Analysis/blob/Images/CREATE%20INPUT%20TABLE.png]
[https://github.com/Dybondzy/COVID_Data_Analysis/blob/Images/EXTRACT%20DATA%20FROM%20INPUT%20TABLE%20AND%20INSERT%20VALUES%20IN%20OUTPUT%20TABLE.png]
[https://github.com/Dybondzy/COVID_Data_Analysis/blob/Images/OUTPUT%20TABLE%20of%20SUMMARY.png]

Comment:
What did I notice in the presentation:  David made the presentation as Project Manager and referred to Michael throughout as having discussions with him.  David made some references to Kimi and Jack, also contributing to the project.  I clearly noticed my name was left out.  This, I pointed out at our next Project 3 Group zoom meeting.  David's reaction was to ask me to do the presentation.  What I meant to say is that, mention my name as part of the group.  (I noticed that this never happened.  I noted it and moved on.  At least the stakeholders (project members,) have accepted the work we all did.)


Then, Michael sent me these files:  for Deliverable 3:

[https://github.com/Dybondzy/COVID_Data_Analysis/blob/Resources/cdc_db_cleaned_part1.zip]
[https://github.com/Dybondzy/COVID_Data_Analysis/blob/Resources/cdc_db_cleaned_part2.zip]
[https://github.com/Dybondzy/COVID_Data_Analysis/blob/Resources/cdc_db_cleaned_part3.zip]
[https://github.com/Dybondzy/COVID_Data_Analysis/blob/Resources/cdc_db_cleaned_part4.zip]
[https://github.com/Dybondzy/COVID_Data_Analysis/blob/Resources/census_age_no_covid.csv]
[https://github.com/Dybondzy/COVID_Data_Analysis/blob/Resources/census_sex_no_covid.csv]

Jack and Kimi and Michael added some downloaded data from from CDC
[https://github.com/Dybondzy/COVID_Data_Analysis/blob/Resources/Group4%20Airport%20By%20Area.csv]
[https://github.com/Dybondzy/COVID_Data_Analysis/blob/Resources/household_income_by_state.csv]
[https://github.com/Dybondzy/COVID_Data_Analysis/blob/Resources/state_factors_from_gallup.csv]

At this point, we had data for Tableau Dashboards and further machine learning analysis 
Yodit and Jack did some work in Tableau
Michael did some neat data analysis in Machine Learning that we were all impressed and anxious to present at our next class meeting.

The output file from our analysis:
[https://github.com/Dybondzy/COVID_Data_Analysis/blob/Resources/COVID_MARCH2020_DEC2020_TOTALS_PROJECT4.csv]


----------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Project Group Delivery 3  

# Coronavirus Pandemic Playbook

## Project Topic, Background, Audience

The term 'pandemic playbook' circulated in the news during the beginning of the COVID-19 pandemic. U.S. President Barack Obama's team had outlined how to respond to infectious diseases and biological incidents so future administrations would be prepared to respond to the next pandemic or biological threat. While the federal government prepared guidelines, state governments from the 50 states + DC were woefully unprepared for a pandemic. The COVID-19 pandemic brought the [deepest recession since the end of WWII](https://www.brookings.edu/research/social-and-economic-impact-of-covid-19/) as the global economy shrunk by 3.5% and [114 million](https://www.weforum.org/agenda/2021/02/covid-employment-global-job-loss/) people lost their jobs in 2020. The impact of this shock is likely to be felt for years to come.

The National Governors Association, a nonpartisan organizations comprised of governors in the U.S., tasked with creating an updated playbook for state governments. They have asked us to provide a comprehensive review of factors that led to the spread of COVID-19 cases in states across the United States. We will be presenting our at the next National Governors Association annual conference in late 2021.

### Project Goal
Drawing on data from CDC, U.S. Census, and many other sources, our goal is to determine which social, economic, and political factors contributed to the spread of COVID-19. There is evidence that if states were more prepared to handle a pandemic, economic performance would not have suffered as it did in 2020. Our nation's governors have the opportunity to learn where our state's weak points were that led to these incredible economic losses and mitigate them in a future pandemic. Our team is confident that our machine learning algorithm will predict which factors contributed the most to the spread of respiratory diseases like COVID-19. The information will valuable for state lawmakers' future economic and social political decisions.

### Project Factors 

Given our audience for the project, the data we've obtained for each factor will be organized by state. 

**Target Variable**
* Number of COVID-19 Cases / State Population

**Social Factors**
* Sex
* Age
* Race
* Religion

**Geographical Factors**
* Population Density
* Number of Commercial Airports / State Land Area

**Economic Factors**
* Median Household Income

**Political Factors**
* State Mandates / COVID-19 rules
* Political Leaning

**Lifestyle Factors**
* Health Insurance Coverage 
* Exercise Frequency
* Social Inclusivity 
* Work Life Status
* Monetary Stability

### Questions to Investigate During Project
1. Which social, economic, geographical, lifestyle or political factors contributed the most the spread of the disease?
2. Which category of factor contributed the most the spread of the disease?
3. Is there a connection between state policy or political leaning (i.e. mask mandate) and the spread of COVID-19 within the state
4. Do we need to account for the size of the population that didn't have COVID-19 when using a machine learning model?

### Roles

* **Project Manager**
    * David
* **Database Storage**
    * Dinah
    * Kimi
    * Michael
* **Data Cleaning and Analysis**
    * Dinah
    * Kimi
    * Michael
* **Machine Learning Model**
    * Michael
* **Presentation of Findings**
    * Yodit (Tableau)
    * Jack (Tableau)
    * David (approver) & Team (GitHub)

### Technologies Used

* **Database Storage**
    * pgAdmin - PostgreSQL
    * AWS RDS
* **Data Cleaning and Analysis**
    * Juypter Notebook - Pandas
* **Machine Learning Model**
    * Google Collab Notebook
* **Presentation of Findings**
    * Tableau Public
    * GitHub

### Communication Protocol 

* [Project Checklist](https://docs.google.com/spreadsheets/d/1G9lvPyMrlkjnYT-qGigKpNdVk72A9Zu0Je7hyy8Q6ug/edit?usp=sharing)
* [Group meeting agendas](https://drive.google.com/drive/folders/1sMOLvKQO-S99917fQL9axuocZujgKNZQ?usp=sharing)

We are meeting twice a week outside of class on Zoom and consistently communicating over Slack. David has established best pratices in GitHub, so we don't overwrite each other's work.

## Data Exploration and Analysis Phases

### Data Exploration and Analysis Overview

We began the project by looking at the entirety of COVID-19 CDC data, which consists of 27 million rows and 19 columns of unique patient information. We quickly realized that if we wanted to replicate the spread of COVID-19 based on any factor, we needed to account for the population that didn't have the disease. We established **Number of COVID-19 Cases / State Population** as our target variable. We found ratio would be easier to handle data-wise than working with large population datasets or creating pseudo population data. Next, we moved on to categorical factors. 

For social factors, we looked at U.S. Census data estimates for information on sex, age, and race. We observed that both datasets had either state abbreviations or states spelled out with their full names. We knew we could join data tables by state, so we focused our efforts on finding geographical, economic, lifestyle and political factors with state columns already available.

### Datasets and Sources

* [Joined and cleaned COVID-19 dataset with factors](https://github.com/dwwatson1/coronavirus_pandemic_playbook/blob/main/Resources/COVID_MARCH2020_DEC2020_TOTALS_PROJECT4.csv) 
* [COVID-19 Cases by Age, Sex, Race](https://github.com/dwwatson1/coronavirus_pandemic_playbook/blob/main/Resources/COVID_MARCH2020_DEC2020_TOTALS_PROJECT4.csv) Source: U.S. Census and CDC
* [U.S. Commercial Airports by State](https://github.com/dwwatson1/coronavirus_pandemic_playbook/blob/main/Resources/Group4%20Airport%20By%20Area.csv) Source: FAA
* [State Mask Mandate Policy/Political Affiliation by State](https://github.com/dwwatson1/coronavirus_pandemic_playbook/blob/main/Resources/state_factors_from_gallup.csv) Source: Gallup
* [Median Household Income by State](https://github.com/dwwatson1/coronavirus_pandemic_playbook/blob/main/Resources/household_income_by_state.csv) Source: U.S. Census

### Description of Data Sources

As stated in the Data Exploration subheading, our original dataset consisted of over 27 million rows of unique patient Covid-19 data sourced from the Center for Disease Control and Prevention (CDC) Case Surveillance Public Use Data. Having analyzed the quality of our data, the Team pivoted to finding additional, specific data that would support our model, have minimum missing data and null values and to answer our investigative questions with a unique perspective. Our primary and final dataset will be constructed by merging primary demographic information from the Center of Disease Control & Prevention (CDC), US census data from US Census Bureau and qualitative survey data from Gallup that will consist of 50 rows of State values and 50-55 columns of factors.  

## Database

### Database Schema ERD

Joining factor data by state (see step 7 below):
![COVID_MARCH2020_DEC2020_PROJECT4%20ERD](https://github.com/dwwatson1/coronavirus_pandemic_playbook/blob/main/Images/COVID_MARCH2020_DEC2020_PROJECT4%20ERD.png)

Joining cleaned CDC data by state (see step 8 below):
![COVID_MARCH2020_DEC2020_PROJECT4_CDC%20ERD](https://github.com/dwwatson1/coronavirus_pandemic_playbook/blob/main/Images/COVID_MARCH2020_DEC2020_PROJECT4_CDC%20ERD.png)

### Building the Database

[Database Storing Overview](https://github.com/dwwatson1/coronavirus_pandemic_playbook/blob/main/Resources/Project%204%20Database%20SQL_steps.txt)

**Steps**

1. We chose input data from CDC from March - December 2020 because March marked when the U.S. declared a state of emergency and December was when the first COVID-19 vaccine dose was administered and U.S. Census data, so we replicate the spread of COVID-19 and account for people who didn't have the disease (as mentioned in the Data Exploration section)
2. Because it was such a large dataset, we split it into 4 parts so cleaning it was more manageable. These parts were imported to the table: CDC_INPUTDB_CLEANED
3. We also used our data from investigating factors into their respective tables: 
   - household_income_by_state into ST_INCOME
   - state_factors_from_gallup into US_POLITICS
   - census_sex_no_covid into CENSUS_SEX
   - census_age_no_covid into CENSUS_RACE
4. After storing the data in pgAdmin - PostgreSQL, we created new tables from CDC_INPUTDB_CLEANED and then segmented age group, state, sex, and race. Here's a review of all the tables we worked with and new columns we created for the final table, for visual, please refer to the ERD above:
   - Table: DATA_AGE_GROUP, COVID_CASES_AGE, New columns: COVID and NO COVID for each group: age_group_0_17, age_group_18_49, age_group_50_64, age_group_65PLUS
   - Table: US_STATES, New columns: none
   - Table: DATA_SEX, COVID_CASES_SEX, NOCOVID_CENSUS_SEX, New columns: COVID and NO COVID for each group: Male, Female
   - Table: DATA_RACE, COVID_CASES_RACE, New columns: COVID and NO COVID for each group: Asian, Black, Multiple/Other, White, American Indian/Alaska Native, Native Hawaiian/Other Pacific Islander, No_identified_race
   - Table: US_POLITICS, New columns: Nearly 30 new political and lifestyle columns with data on information on mask mandates, political party, exercise frequency, sense of community, etc. 
   - Table: AIRPORT_BY_AREA, New columns: total airports, state land area (sq. miles), airport area (airports per sq. mile)
   - Table: ST_INCOME, New columns: median income
5. We identified that we could join all tables using the states column. Using the table: US_STATES, we created the table: COVID_MARCH2020_DEC2020_PROJECT4, of totals per state, with calculated data from the table: CDC_INPUTDB_CLEANED
6. Using the table: US_STATES, we added all the tables with totals, and created the table: COVID_MARCH2020_DEC2020_TOTALS_PROJECT4
7. Next, we joined all tables by **state** to input data from all tables to COVID_MARCH2020_DEC2020_TOTALS_PROJECT4. 
   - Please refer to the **first ERD image** for the visual of this process
8. Simiarly, with the cleaned CDC_INPUTDB_CLEANED table mentioned in **step 2 and step 3**, we joined the tables by state and input the data to COVID_MARCH2020_DEC2020_TOTALS_PROJECT4 as well. 
   - Please refer to the **second ERD image** for the visual of this process
9. We exported our table COVID_MARCH2020_DEC2020_TOTALS_PROJECT4 from pgAdmin to the csv file: [COVID_MARCH2020_DEC2020_TOTALS_PROJECT4](https://github.com/dwwatson1/coronavirus_pandemic_playbook/blob/main/Resources/COVID_MARCH2020_DEC2020_TOTALS_PROJECT4.csv)

### Data Dictionary

![image](https://user-images.githubusercontent.com/79073778/126433251-84f72a83-93df-47fc-9797-425836639f47.png)

## ETL Method

### Extracting the Data
Our main dataset was COVID-19 CDC data, which consists of unique patient information spanning 19 columns and 27 million rows. With such a large dataset, we used Amazon S3 to store the data and used Google Colab with Pyspark to access and load the data.

### Transforming the Data
With the data loaded, we could now transform our data. We first filtered the data to be between March 2020 and December 2020. We chose this date range because March 2020 was when the United States declared COVID-19 a pandemic and December 2020 was when the first vaccine was administered in the United States. After filtering the data by date, we dropped many columns from the dataset for either or both of these reasons: 1) there were too many missing values for the variable to be usable and/or 2) the variable was not useful for our analysis. After dropping the unnecessary columns, the data was left with four variables: res_state, age_group, sex, and race. The dataset also had missing values which were identified in the data as either "Missing", "Unknown", or "NA". We replaced all the "Missing" and "Unknown" values to be "NA" for simplicity in identifying the missing values. The data was then exported to a CSV file where it was then imported into SQL for storage and further querying.

### Loading the Data
We used SQL to store the data and query it so that the data would be organized by state with the values becoming our new features. For example, we now have "Male" and "Female" as features of our data with totals of each for each state, whereas in the base CDC data, "sex" was the feature and "Male" and "Female" were values for the unique patients. The other features we are using were imported from their respective CSV files and joined to this main table. Using the U.S. Census data, we were able to create the features for those who do not have COVID by subtracting the number of people with COVID by the total numbers for each state. For example, to find the total number of females who do not have COVID for the state of Maryland, we subtracted the total number of females with COVID from the total population of the state of Maryland.

### Handling Missing Values
The CDC dataset we used had many missing values for the patients age, sex, and race. This is to be expected as many people opt out of providing such information. Because machine learning models cannot run with null values, we had to find a way to handle the missing values. We came up with four possible strategies:

1. Delete the observations with missing values.
2. Delete the variable.
3. As the features with missing values are categorical variables, we could impute the missing values by using the mode.
4. We can predict the missing values for the categorical variables by using a classification model. We would split the data as such:
  - y_train: rows from data with non null values
  - y_test: rows from data with null values
  - X_train: Dataset except data features with non null values
  - X_test: Dataset except data features with null values

We did not want to delete observations as that would mean less data and also would misrepresent the total number of COVID cases. We also did not want to delete the variables as we felt age, sex, and race are important variables for understanding the spread of COVID. For age and sex, we decided to impute the missing values with the mode, as both variables had very low numbers of missing values (1% and 3% respectively). Race, however, had about 42% of missing data. Imputing the data with the mode would not be effective here as a few states had no race data at all. However, we felt that even though there were many missing values for race, the lack of data has something to show for itself. There is strong analysis that can be made on why that data is missing and exposes the weaknesses in data collection on behalf of the CDC and state governments, demonstrating how disjointed states were in their response to COVID and data collection, and on such a crucial factor such as race. That being said, the missing values still had to be accounted for in order for the data to be run through a machine learning model. Therefore, the total number of missing values for each state were put into its own column.

## Machine Learning

### Model Choice
The model we chose to use is a **supervised random forest regression model.** We chose supervised machine learning because we have labeled data (our features in tabular form) and outputs. The input data, or our features, has a paired outcome which is plugged in to train the model to predict outcomes. Supervised machine learning models have target variables, or dependent variables, about which we want to gain a deeper understanding. In our case our target variable is how much effect COVID had on a state's population by looking at the total number of COVID cases divided by the total state population.

We chose a random forest algorithm because it can handle many input variables of which we have many. The algorithm can run efficiently on large datasets, and most importantly, random forest models can be used to rank the importance of input variables. This fits the question we are trying to answer perfectly - **what are the top factors that influence the spread of COVID?** A random forest model will help us rank the most influential factors. Since we have a large dataset with many features, as well as both continuous and categorical non-linear variables, a random forest algorithm will be more efficient and more accurate than a simple linear regression. While a large number of trees in a random forest algorithm can be slow requiring a lot of computational power and resources, the advantages outweigh the disadvantages.

### Code for Random Forest Model
To create the random forest model, we first initialize the dependencies, notably the 'from sklearn.ensemble import RandomForestRegressor'.

```
import pandas as pd
import numpy as np
from path import Path
from sklearn.ensemble import RandomForestRegressor
from sklearn.preprocessing import StandardScaler
from sklearn.model_selection import train_test_split
from sklearn import metrics
```

After loading in the data, we use one hot encoding to account for null values and convert categorical variables to integer data.

```
file_path = ("COVID_MARCH2020_DEC2020_TOTALS_PROJECT4.csv")
covid_df = pd.read_csv(file_path)

covid_cat = covid_df.dtypes[covid_df.dtypes == "object"].index.tolist()

from sklearn.preprocessing import OneHotEncoder
enc = OneHotEncoder(sparse=False)
encode_df = pd.DataFrame(enc.fit_transform(covid_df[covid_cat]))

encode_df.columns = enc.get_feature_names(covid_cat)
encode_df.head()
```

We then merge the one hot encoded features to the main dataframe and drop the originals.

```
covid_df = covid_df.merge(encode_df, left_index=True, right_index=True)
covid_df = covid_df.drop(covid_cat,1)
covid_df
```

We split our preprocessed data into our features and target variables.

```
y = covid_df["case_pop"].ravel()
X = covid_df.copy()
X = X.drop("case_pop", axis=1)
```

We then split the data into training and testing sets and scale the data. We set random_state to a number in the testing phase so that we can consistently see the same results when the test model is run (this could possibly be removed for the final model).

```
X_train, X_test, y_train, y_test = train_test_split(X, y, random_state=1)

scaler = StandardScaler()

X_scaler = scaler.fit(X_train)

X_train_scaled = X_scaler.transform(X_train)
X_test_scaled = X_scaler.transform(X_test)
```

We initialize the random forest classifier and fit the model. We set n_estimators to 128 because best practice is to use between 64 and 128 forests. Generally, the higher the number, the stronger and more stable the predictions are. Given that this is a test model, it is reasonable to assume the model might be able to handle 128 forests.

```
rf_model = RandomForestRegressor(n_estimators=128, random_state=1) 

rf_model = rf_model.fit(X_train_scaled, y_train)
```

We make predictions and then evaluate performance using the Mean Absolute Error, Mean Squared Error, and the Root Mean Squared Error.

```
y_pred = rf_model.predict(X_test_scaled)

print('Mean Absolute Error:', metrics.mean_absolute_error(y_test, y_pred))
print('Mean Squared Error:', metrics.mean_squared_error(y_test, y_pred))
print('Root Mean Squared Error:', np.sqrt(metrics.mean_squared_error(y_test, y_pred)))
```

We finally rank the importance of the features and see which have the most impact on the output.

```
importances = rf_model.feature_importances_
importances

sorted(zip(rf_model.feature_importances_, X.columns), reverse=True)
```

## Dashboard

### [Tableau Dashboard Demo](https://public.tableau.com/views/ALLSTATESDATAMARCHtoDEC2020/Dashboard4?:language=en-US&:display_count=n&:origin=viz_share_link)

### Blueprint and Interactive Elements

One of the interactive elements we are using is the filter action. Filter actions send information between worksheets. Typically, a filter action sends information from a selected mark to another sheet showing related information. Behind the scenes, filter actions send data values from the relevant source fields as filters to the target sheet and dashboards.

For example, in a view showing the states, when a user selects a particular state name, a filter action can show all state values for all the displayed variables. 
User can select marks to see information about a specific data filed. One can also select an individual mark or multiple ones by holding down the Ctrl key (for Windows) or the Command key (macOS).

When you select marks in the view, all other marks are dimmed to draw attention to the selection. The selection is saved with the workbook. Quick data view can also be done by one of the run-on options; hovering your mouse on the charts/marks. 

We have also created a simple HTML file to show the dashboard in a dedicated webpage with another interactive element where users can download the analysis into PDF file. 



#### OBSERVATIONS
s


----------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Project Delivery 4

We are at a crossroad right now.  All the work of the past 3 weeks seems to be erasing and I have questions

From the good work we had in Delivery 3, questions were asked
My reaction is that it is good to have questions and interest, so we are on track.
Michael had conversations on improving the machine language, and changed all the tables, cancelling SQL, ERD and all other tables, to get a targeted answer.  Michael and David created a fabricated / synthetic table, that will change our analysis.  I had questions for further conversations:

----------------

Michael Leggett  10:45 AM
@Dinah Bondzie, here is the covid data if you would like to start putting this into SQL. These files just need to be joined on top of each other if that makes sense, so there should be only 5 columns (state, age, sex, race, has_covid) and millions of rows. David and I are working on the data for the people who don't have covid and we will send that to you as soon as its ready.
4 files 
data_part1.zip
6 MB Zip6 MB — Click to download


data_part2.zip
3 MB Zip3 MB — Click to download


data_part3.zip
5 MB Zip5 MB — Click to download


data_part4.zip
5 MB Zip5 MB — Click to download



David Watson  11:51 AM
Only think I ask is that if we make new SQL documentation like the txt file. Can we save it under a new name like Part 2? I want to keep most of what we did for the Part 1 Analysis because it explains all the exploration that went into the project

Dinah Bondzie  3:04 PM
Could someone please explain the changes we are making?
3:04
Why do we have to discard the work we've done in the past 3 weeks?
3:05
What do I do with the zipped files
3:05
The new analysis seems to be a bit beyond my knowledge from the bootcamp (or may be not)

David Watson  3:21 PM
@Dinah Bondzie This part is going to make our analysis better and more clear. We want to be able to answer our crux question which is do we need to rewrite the playbook. As the analysis stands right now, we can't identify anything because we looked at data from states rather than generating data that represented states. Michael and I have been working on this and building out millions or rows of data. Think of this as our second attempt to make our project stronger. I'm keeping everything in the README as is but with this second pass, we should be able to get a more solid conclusion and visualizations as I understand it. Feel free to add if I missed @Michael Leggett
3:22
I think the TA's and Nick will appreciate the thought we put into this. But where this stands now, this part is like the conclusion/lessons learned part. But we're actually giving it a good and seeing what happens

Dinah Bondzie  3:24 PM
David, apart from you and Michael, who else understands and agrees with the change
3:25
I just prefer when we have the facts clear

Michael Leggett  3:57 PM
The facts are simply this:
Our aggregated table does not have a lot of predictive power. What a machine learning does is split data into testing and predictive so it will take 75% of our data and try to predict the other 25%. That means that it will take 35 states, learn from those states, and then use that to predict the affect of covid for the other 15. That is not good analysis. These states are individual observations. To have the model take CA and NY and predict for Nebraska would be bad.
With data aggregated by state, we simply cannot find the factors for each state and compare with the big table, even if running our big table through the ML model had any sort of sound analysis. That was what triggered the conversation with Zeb in the first place.
This leaves us with faulty analysis and a bad ML model. So what's the alternative?
The alternative is we try something else, mainly because we don't have much of a choice. This doesn't mean what we did was worthless. It's still an excellent tool for Tableau and data visualizations, plus everything that David laid out in his earlier message, and it was a big help in what I'm about to explain next.
Our only alternative is to go back to what we originally wanted to do in the first place - be able to predict whether or not someone has covid based on a bunch of factors with the target variable being whether or not a person has covid. That was the original idea. Where it snagged was that we only had data for who has covid and no data for who does not have covid. David and I have been working on a way to use feature engineering (Zeb said it was incorrect to say synthetic data) to create new values for those people who do not have covid. We used the big table Dinah created in SQL to help us do this. It's already almost done. Once I send those tables to you Dinah, we could have a ML model for this as soon as tomorrow. We'll be able to run ML models for this big new table and ML models for each state and compare. That's the current plan which we laid out in our post Zeb meeting which I thought we were mostly on board for.
There is not much being done outside the scope of this bootcamp. The creating the "synthetic data" kind of is but again, it's already almost done, and even then, we have done feature engineering in this bootcamp, it's not necessarily new.
Please continue to post questions or concerns in here, as it's important that we're all on the same page.

Dinah Bondzie  5:49 PM
@Michael Leggett do you mean put all files into the same table?  No joins, just import.  The ERD will be the one table.  Also, no summarizing
5:50
Maybe join to the noCOVID file when you send it

Dinah Bondzie  5:59 PM
@David Watson It'll be the same as the cdc_data file in the past ERDs
:ok_hand:
1


Michael Leggett  6:49 PM
@Dinah Bondzie Yes, I think you have it right! My saying 'join' probably wasn't the right word. The four data files look exactly the same - they have the same column headings. They're essentially one big table just split into four different csv files and they need to be put back together into one giant file in SQL. As you said, just imports will probably do! The table in SQL should maintain those 5 column headings and have millions of rows. Hope this helps.

Dinah Bondzie  9:15 PM
@Michael Leggett combining the 4 zipped files into one csv file is too big for my processor.  Can you run your ML code on the csv files you sent me?  It doesn't change ... or shouldn't
9:16
You did the work already :blush:
9:18
No new ERD either, it is not relating to any other database / table
9:21
Don't we loose some points without SQL joins?  Have we covered that

Michael Leggett  1:34 PM
No worries Dinah! I was able to combine the data. It is very large so uploading to amazon s3 now. Hoping I'm able to run this through a ML model before class today and hopefully we can really use class time to discuss how to move forward and see if this is something that is worth pursuing or if we should try to figure out something further with our aggregated data. Maybe putting our table into ratios and using an unsupervised model would be enough to be able to keep using our aggregated data? Any other thoughts? Hoping Nic will join in our breakout room at some point and maybe he can help guide us.
1:38
Mainly the issue is that we just don't have enough observations. We have county data, maybe we can aggregate by county instead?

Dinah Bondzie  1:39 PM
Ok

Michael Leggett  1:42 PM
Or maybe we bite the bullet and say, hey, this is what we got. Here a bunch of next step options. I don't think Nic would necessarily be upset with that but I guess we can see.

Dinah Bondzie  1:43 PM
Michael, I know you mean well for our group
1:43
Let's just get questions answered

David Watson  1:51 PM
I think the ship has sailed on pursuing county data. We committed to this route on Sat. and I think that's fine as long as we explain what happened and it's really ok if there are limitations from the data. After all, I think the joins would've been way more challenging by county. Would've needed a lot of manual data segmentation
New

Michael Leggett  1:54 PM
Yeah I agree David, good points. Would be a good thing to mention in a next step section or something similar though

David Watson  1:54 PM
Did we get our deliverable 3 graade?

Michael Leggett  1:54 PM
I do not see a grade yet




----------------
