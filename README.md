# Salary Predection: Project Overview
- Created a tool that estimates the **Employees Salary** to help HR to calculate the salary.
- Data is prepared by me.
- Engineered Features from the data and handling the missing values and outliers.
- In this project I used Linear Regression because the target was a continuous data.
- Built a client facing API using Flask.
## Code and Reources Used
**Python Version:** 3.7  
**Packages:** pandas, numpy, sklearn, matplotlib, seaborn, flask, json, pickle  
**For Web Framework Requirments:** `pip install -r requirements.txt`
## Data Collection
Data consists of following columns.
- experience  
- test_score  
- interview_score  
- salary
## Data Cleaning
After the data is prepared, I need to clean the data so that it was usable for our model. I made the following changes:
- Finding the missing values in the experience column and replacing with the 0.
- I changes the values of experience from string to numeric.
## Model Building
First I split the data into X and y.  
Because of the target column is continious we know that we can use the **Linear Regression**
## Deployment 
The model is dumped by using the pickle file.
## Production
In this step I build a filsk API endpoint that hosted on a local webserver.  The API endpoint takes in a request with a list of values from the HR  and returns the estimated salary.  
Latter, I uploaded this project in [Heroku](https://salary-predection-api.herokuapp.com/)

