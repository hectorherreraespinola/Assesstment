Exploratory Data Analysis of Chronic Illness Costs
Project Overview
This project aims to analyze the costs associated with chronic illnesses using a dataset of outpatient claims and beneficiary summary files. The analysis includes data cleaning, visualization, and identifying patterns in healthcare costs.  
Data Sources
DE1_0_2009_Beneficiary_Summary_File_Sample_20.csv: Contains beneficiary summary information.
DE1_0_2008_to_2010_Outpatient_Claims_Sample_20.csv: Contains outpatient claims data.
Steps in the Analysis
1. Getting the Data
The data is loaded from CSV files into Pandas DataFrames. Detailed information about the data can be found here.  
2. Data Cleaning
Chronic conditions are converted to boolean values.
A new column Chronic_Conditions is created to represent combinations of chronic conditions.
3. Basic Summary
What is the distribution of races?
What is the most common chronic illness combination?
Which chronic illness combination has the total highest cost?
Which chronic illness combination has the highest cost per member?
4. Benchmarking
For each provider (use AT_PHYSN_NPI) & chronic illness, calculate the cost per member.
For each chronic illness combination, represent the distribution of costs per provider.
How does this change if we filter out cases where a given Chronic Illness & Provider NPI combination only has 1 member?
Which providers are consistently expensive across chronic illnesses they treat?