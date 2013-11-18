Data Analysis Assignment 1 README


Raw Data - Accessed on 11/13/2013 6:04 PM

URL: https://spark-public.s3.amazonaws.com/dataanalysis/loansData.rda

ntroduction:

Lending Club provides loans to individuals with investor members providing the funds for the loans. The company determines the interest rate of a loan by weighing credit risk and market conditions in addition to its base rate. Of all the variables considered by Lending Club, three are more strongly associated with the final interest rate, after an individual’s FICO score is considered. The Loan Amount, Amount Funded by Investors and Length of the Loan seem to be positively correlated with the interest rate, where higher values of these variables correlate with higher interest rates and lower values correlating with lower interest rates.

Methods

Data Collection

For the data analysis, I used 2500 rows of lending data that was provided by Lending Club. The data was downloaded on 11/10/2013 from Amazon’s S3 servers (via a link in the Assignment 1 Instruction page).

Exploratory Analysis

Exploratory analysis was performed by examining tables and plots of the observed data. I identified transformations to perform on the raw data on the basis of plots. Exploratory analysis was used to identify missing values and cleanup the data; identify the relationships of the different variables to the Interest Rate; and to see how each of the variables is distributed.

Statistical Modeling

In identifying associations between each of the variables in Lending Club’s data and the final interest rate, I chose to apply the correlation function in R to Interest Rate and each of the rest of the variables in the data. I created four subsets of the data by dividing them into four quartiles, according to the midpoint of the FICO score range. That is, I added a new column into my data frame which is the midpoint of the FICO score range and created subsets using quartiles of the new column.

