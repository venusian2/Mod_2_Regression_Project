# Mod_2_Regression_Project

DSC NYC Flatiron Module 2 Project:
By: **Jason Drummond**

## Goal

To create a linear regression model that will be used to predict Salaries of NYC Employees based upon a multitude of different variables.

## Use Case

As a new high school graduate you would like to find a career that will pay the most upon graduating college.

## DataSet

Our Dataset comes from the NYC Open Data website, (https://data.cityofnewyork.us/City-Government/Citywide-Payroll-Data-Fiscal-Year-/k397-673e)

There were over 3 million rows in our Dataset depicting the salaries for NYC Employees between the years of 2014-2019. It is our goal to see what factors contribute most to an Employees Salary.


## Data Cleaning

There were many things that needed to be cleaned up in our Dataset. First we dropped Fiscal Year 2014 from our dataset as it had very little data to use. We then created a new column to explore any relationhip between number of years worked for city and Salary. Upon investigating the Data for Teachers I found bi problem that needed to be fixed. Whenever a Teacher does extracurricular work they get paid per session and this shows up in an entirely different row from their yearly salary. I took all the money they made from this row and addded it in as OT in their respective yearly salary row. This one step got rid of a big chink of Data as teachers are one of the most common jobs in NYC. From here I fixed all of the Agency Names to reflect the overarching Agency that they belong to, as some were broken down into smaller components, mainly Community Board, Department of Eduaction, and District Attorney. The last step was getting rid of anyone that was not a full time workker as we only wanted to focus on this group.

## Statstical Tests

* Two Sample T-test on two most populous jobs based on salary
  * We Rejected the null hypothesis that these salaries were not statisticaly different from one another
* Annova/MultiComparison Test on work location 
  * We Rejected the null hypothesis that the salariies in each borough were not statistically different
* Annova/MultiComparison Test on Pay Basis
  * We Rejected the null hypothesis that the salaries in each pay Basis were not Statistically different


