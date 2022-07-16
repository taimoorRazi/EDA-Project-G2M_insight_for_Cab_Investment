# G2M insight for Cab Investment firm


## What is the business problem?

**The Client**:
XYZ is a private firm in US. Due to remarkable growth in the Cab Industry in last few years and multiple key players in the market, it is planning for an investment in Cab industry and as per their Go-to-Market(G2M) strategy they want to understand the market before taking final decision.

**Project delivery**:
You have been provided with multiple data sets that contains information on 2 cab companies. Each file (data set) provided represents different aspects of the customer profile. XYZ is interested in using your actionable insights to help them identify the right company to make their investment.

The outcome of your delivery will be a presentation to XYZ’s Executive team. This presentation will be judged based on the visuals provided, the quality of your analysis and the value of your recommendations and insights

**Data Set**:
You have been provided 4 individual data sets. Time period of data is from 31/01/2016 to 31/12/2018.
Below are the list of datasets which are provided for the analysis:

1. Cab_Data.csv – this file includes details of transaction for 2 cab companies

2. Customer_ID.csv – this is a mapping table that contains a unique identifier which links the customer’s demographic details

3. Transaction_ID.csv – this is a mapping table that contains transaction to customer mapping and payment mode3. 

4. City.csv – this file contains list of US cities, their population and number of cab users


## What are the properties of the data provided (data intake report)

Tabular data details:

File 1: Cab_Data.csv
Total number of observations	<359392>
Total number of files	<1>
Total number of features	<7 >
Base format of the file	<.csv>
Size of the data	<20.1 MB>

File2: Customer_ID.csv
Total number of observations	<440098>
Total number of files	<1>
Total number of features	<3 >
Base format of the file	<.csv>
Size of the data	<1.0 MB>

File3: Transaction_ID.csv
Total number of observations	<49171>
Total number of files	<1>
Total number of features	<4 >
Base format of the file	<.csv>
Size of the data	<8.58 MB>

File4: City.csv
Total number of observations	<20>
Total number of files	<1>
Total number of features	<3 >
Base format of the file	<.csv>
Size of the data	<4.0 KB>



## What steps were taken in order to create an applicable data set?

The datsets were merge together on common columns to avoid duplication of columns. Cab_Data was merged with Customer_ID on transaction ID.
The customer Data also contains the unique transaction ID as in Cab data. However, there are 80706 data entries(rows) more in df_customer than the df_cab dataframe. These rows were lost when we merge these dataframes as it would have so many missing values especially the cab company column. This combined data frame was further merged with Transaction_ID dataset on Customer ID column. This combined dataset was further merged with City dataset on City column.
After merging, feature engineering was done to clean the data and to create new features. The data types of the variables were corrected. 

## How did you prepare and perform your analysis?

Initially, brainstorming was done and different questions/hypothesis were made regarding the dataset. 

## What type of analysis did you perform?

Numerical and Categorical Analysis 
Demand analysis 
Profit Analysis
Customer Loyalty Analysis


## Why did you choose to use certain analytical techniques over others?

Since the aim of the EDA was to help XYZ make investment in the more successful company, Demand analysis and Profit analysis over the time period (Time series analysis) is useful to compare the success of the companies. 
The initial categorical and numerical analysis was performed to give an overall outlook on the market as it is easy and fast to perform.

## What were the results?

The result showed that the yellow cab dominated the market in terms of demand, profits, customer loyalty etc and hence is the right company to invest in.
