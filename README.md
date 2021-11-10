# Predicting Loan Defaults

## I. Introduction

The code contained in this notebook predicts loan defaults, sourced from 12 years of data from Lending Club (dataset found on Kaggle):

https://www.kaggle.com/wordsforthewise/lending-club?select=accepted_2007_to_2018Q4.csv.gz

This data was supplemented with macroeconomic indicators, pulled from the Federal Reserve Economic Dataset (FRED). Data from FRED was sourced via the quandl API in python. 

The final dataset encompasses over a million loans from Jan 2007 - Dec 2018.

## II. Modeling

In this project, 2 types of models were used - logistic regression and naive bayes. Each model predicts whether a given loan, based on applicant data and over-arching macro indicators, will be paid in full and default. 

Three unique datasets were passed through each model, with a combination of independent variables to asses the following 3 ranges:

1. All data, regardless of multicollinearity, as a baseline
2. Payment related variables removed from dataset
3. Payment and loan variables removed

Dataset 3 looks to explore only applicant and macro indicator data. The goal was to look at the direct effect of applicant data separated from information of payments during the length of the loan
