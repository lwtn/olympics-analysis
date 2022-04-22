# Summer Olympic Games Analysis
![olympic](https://user-images.githubusercontent.com/97715547/161469419-e152356b-0fb6-46bf-93e0-edc16a5d41a5.jpg)

## About
This Mini-Project for SC1015 looks into the Olympic Games from the [120 Years of Olympic History](https://www.kaggle.com/datasets/mysarahmadbhat/120-years-of-olympic-history) dataset. Together with [World GDP](https://data.worldbank.org/indicator/NY.GDP.MKTP.CD) and [World Population](https://data.worldbank.org/indicator/SP.POP.TOTL) datasets from The World Bank, we merged these datasets together to generate useful insights. The following is a brief preview of the project:
1. Data Exploration
>- Scoping the project, separating data by gender, relationship between variables
2. Data Cleaning and Merging
>- Filling in NULL values, merging dataset with GDP and Population
3. Medal Analysis and Visualization
>- Compare medal count of countries, relationship between medal count and GDP
4. SMOTE and Random Forest Classifier
>- Dealing with class imbalance, predict medals based on chosen factors
>- Quick Note: Do not be mistaken by the variable names within the files. Notations such as "female_swim" or "male_swim" are not to be erroneously associated with the sport of swimming. Rather 'swim' is shorthand for 'sports with indicated medals'  


## Contributors
- @lwtn - Data Extraction, Data Visualization
- @sien551011 - SMOTE, Random Forest
- @wenyang1608 - Data Cleaning, Data Merging

## Problem Definition
- Are there any major factors that contribute towards the chances of winning an Olympic medal?
- Can we predict whether an athlete will win a medal based on these factors?
- Which medal will they win?

## Conclusion
### Objective 1: Is there a way to predict what medal a certain athlete would get in a particular sport before he/she even plays? 
The models that have been derived from the train data set are successful when tested with both the “pseudo-test” and Test data sets.

### Objective 2: For every sport, is there a particular quality of an athlete that makes him/her more likely to win? 
As can be seen from the classification tree models, and what was discussed earlier, many of these sports have GDP as a key predictor (often with higher GDP linked to higher chance of winning). 
Poorer countries can either avoid those sports, or channel only suitable athletes into these sports to maximising winning


Example: For Swimming (Male), it is unfortunately harder for less affluent countries to win a gold medal as from 2000 to 2016, 1832/2156 (~85%) of gold medals were won by countries with GDP Per Capita > 14970.
  Yet, what poorer countries can do to maximise their chances of getting a gold medal is to send athletes that are: 
  - Taller than 185cm
  - Weigh less than 76.957 kg
  - Younger than 24 years old
  This can be derived from analysing the branching points of the model.


