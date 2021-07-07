# Hackathon_anmol
Summer Analytics Capstone Project by C&amp;A Club, IIT Guwahati

Problem Statement
 

Let's take a case where an advertiser on the platform (DeltaX) would like to estimate the performance of their campaign in the future.

Imagine it is the first day of March and you are given the past performance data of ads between 1st August to 28th Feb. You are now tasked to predict an ad's future performance (revenue) between March 1st and March 15th. Well, it is now time for you to put on your problem-solving hats and start playing with the data provided under the "data" section.

Who is an advertiser?
An advertiser is a person or company that pays for their product/event to be advertised online or offline. 




About the data
The sample data dump shared below is the ad performance for the dates between 1st August 2020 and 28th Feb 2021.

Here is a brief hierarchy for relationships in adtech systems:

 


One Campaign can have one or more Ad Groups. One Ad group can have one or more ads. In the given dataset - we have only 1 campaign; 4 Ad Groups and multiple ads.


 

 

 

Data Description

 
 
 

date: the date on which the ad was made live

campaign: campaign number

adgroup: adgroup number

ad: ad number

impressions - Number of time the ad was shown

clicks - Number of time the ad clicked shown

cost - Amount spent to show ad

conversions - Number of transactions received

revenue: revenue generated from the ad

 
 
 
 

Below is some context about the dataset:

 
 
 
 

Raw metrics:

Impressions - Number of time the ad was shown

Clicks - Number of time the ad clicked shown

Cost - Amount spent to show ad

Conversions - Number of transactions received (higher the better)

Revenue - Total value of transactions received (higher the better)

 

Efficiency metrics (optional - can be used for creating new features/feature engineering): 

The below features can be newly created/calculated and used while building the models. These are based on raw metrics. 

CTR - Clicks / Impression (higher the better - used to evaluate if the users find the ad relevant)

CPC - Cost / Click (lower the better - used to evaluate if the cost for getting a click)

CPA - Cost / Conversion (lower the better - used to evaluate if the cost for getting a conversion)

ROI - Revenue/Cost (higher the better - used to evaluate the effectiveness of the advertising budget spent

 

 How to download and read the dataset?
 

In the 'Data' section of the challenge page check the 'Resources' subsection. For reference, see the screenshot below (the red box):


 

Click on the dataset that you want to download.

After you have downloaded the dataset, you can read the dataset in your jupyter notebook using the read_csv() function. Provide the appropriate path of the data located on your machine. For example, if the data is located in the same location where you are executing your jupyter notebook, you can read the dataset as:
train_data = pd.read_csv('Train data.csv')

 
Saving Prediction File & Sample Submission
 

You can find more details on how to save a prediction file here: https://discuss.dphi.tech/t/how-to-submit-predictions/548

 

Sample submission: You should submit a CSV file with a header row and the sample submission can be found below:

 

revenue
25
0
0
0
0
0
42.77
0
143.5
0
836.34
.

.

.

Etc.

Note that the header name should be ‘revenue’ else it will throw an evaluation error.

 

 

Acknowledgement
 

We would like to thank DeltaX for providing us this dataset.



