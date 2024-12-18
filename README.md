# Data Project Repo
## Summary
### Defining the Question
#### The objective of this data analysis is to determine how age, gender, employment status, marital status, education and income relate to average number of books an individual reads per month.  This data source comes from [https://www.kaggle.com/datasets/vipulgote4/reading-habit-dataset/data](https://www.kaggle.com/datasets/vipulgote4/reading-habit-dataset/data).  This data might answer the objective because it contains data for almost 3000 individuals on their reading habits, personal income, employment status, age and other information.

### Data Cleaning
#### Corrections were made to column titles. Column titles were changed to increase readability. Corrections were made to the income ranges in the Income column. Columns of unneeded data were dropped from the data set. The rows that contained null values for income were dropped from the data set. It was determined that the Midpoint Income column is slightly right skewed therefore dropping the rows without an income was chosen versus filling the null values with the mean (since there is a skew, filling with the mean, would have further altered the integrity of the data set). Midpoint Income was reconverted to an int64 to eliminate the decimal place. Additionally, the null values in the Education column were replaced by Unknown. Data types for each column were checked to ensure they were properly assigned. 

### Engineered Features
#### A new column, Midpoint Income, was created that contained a single numerical value, from the original Income column. Instead of having a range of incomes, the midpoint of the range was calculated and entered into the Midpoint Income column for each row.  Additionally, a new feature was created by dividing the ages of the data set into three categories in the Age Group – child, adult and senior. 

### Findings
#### For this data set: women appear to read a higher average of books per month than men (there is a significant difference in the number of books read per month per gender). There is a significant difference in the number of books read per month based on educational level (those with more education appear to read more books). There is a significant difference in the average books read per month based on employment status, however the definition of “Other” in the Employment column was not defined so it’s not clear what “Other” stands for – given this is not defined, it’s not clear that this is a valid finding. There is a statistically significant different int  the average number of books ready per month based on age group, with seniors reading the most books per month, followed by children and then adults. 

#### The following do not appear to predict how many books an individual reads per month: income, marital status. There doesn’t seem to be a strong pattern of correlation between age, number of books read per month and income. It appears from the graph Age versus books ready by month by education that that Seniors with college/some college/technical training/professional training are reading more than adults with similar education. It also appears from the graph Gender versus Books read per Month by Education that females with college/some college/technical training/professional training are reading more books per months than males with same education. 

#### The main objective of this data analysis was to determine how age, gender, employment, marital status, education and income relate to average number of books an individual reads per month. For this data set, it has been determined that age, gender and education all impact the number of books read by an individual each month. 


### Summary
#### In conclusion, age, gender, and a higher level of education are associated wtih reading more books each month. Women tend to read more than men. Seniors read more than children who read mroe tahn adults. Income and marital status do not appear to impact average number of books read per month. 

### Recommendations
#### This is a small data set. In order to determine if these findings can be generalized to a larger population, a larger data set should be obtained. Additionally, these findings are limited given the geographical location of the individuals contributing to the data set is unknown. It is also unknown when and how this data was obtained. It is recommended that fu4rther analysis of this data could be completed with more advanced statistical methods. It is also recommended that to enlarge the data set, so that it could possibly be more valid to generalize to the larger population, that other data sets of simliar or related data be merged into this one to enlarge the data set. 
