#[Facebook V: Predicting Check Ins](https://www.kaggle.com/c/facebook-v-predicting-check-ins/)

##Identify the correct place for check ins

[Ever wonder what it's like to work at Facebook?](https://www.kaggle.com/c/facebook-v-predicting-check-ins/details/work-at-facebook) Facebook and Kaggle are launching a machine learning engineering competition for 2016. Trail blaze your way to the top of the leaderboard to earn an opportunity at interviewing for one of the 10+ open roles as a software engineer, working on world class machine learning problems.
##Acknowledgements

![ScreenShot](FB5_banner.png)

The goal of this competition is to predict which place a person would like to check in to. For the purposes of this competition, Facebook created an artificial world consisting of more than 100,000 places located in a 10 km by 10 km square. For a given set of coordinates, your task is to return a ranked list of the most likely places. Data was fabricated to resemble location signals coming from mobile devices, giving you a flavor of what it takes to work with real data complicated by inaccurate and noisy values. Inconsistent and erroneous location data can disrupt experience for services like Facebook Check In.

We highly encourage competitors to be active on [Kaggle Scripts](https://www.kaggle.com/c/facebook-v-predicting-check-ins/kernels). Your work there will be thoughtfully included in the decision making process.

##Data

In this competition, you are going to predict which business a user is checking into based on their location, accuracy, and timestamp. 

![ScreenShot](kaggle_screenshot.png)

The train and test dataset are split based on time, and the public/private leaderboard in the test data are split randomly. There is no concept of a person in this dataset. All the row_id's are events, not people. 

**Note**: Some of the columns, such as time and accuracy, are intentionally left vague in their definitions. Please consider them as part of the challenge.

###**File descriptions**

- **train.csv, test.csv**
	- row_id: id of the check-in event
	- x y: coordinates
	- accuracy: location accuracy 
	- time: timestamp
- place_id: id of the business, **this is the target you are predicting**
- **sample_submission.csv** - a sample submission file in the correct format with random predictions


##Evaluation

Submissions are evaluated according to the [Mean Average Precision @3](https://www.kaggle.com/wiki/MeanAveragePrecision)  (MAP@3):
MAP@3=1|U|∑u=1|U|∑k=1min(3,n)P(k)
where |U| is the number of check in events, P(k) is the precision at cutoff k, n is the number of predicted businesses. 

##Submission File

For every user check in, you must predict a space-delimited list of the businesses they check into. **You may submit up to 3 predictions for each check in.** The file should contain a header and have the following format:
```
row_id,place_id
0,2083653582 1476539553 1000015801
1,6147316961 6147316961 8999137193
etc...
```