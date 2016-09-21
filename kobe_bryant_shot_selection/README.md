# [Kobe Bryant Shot Selection](http:////www.kaggle.com/c/kobe-bryant-shot-selection)

*If your name is Kobe Bryant, you take the toughest shots. It's what you do.*  
~~*If you want to save 15% or more on car insurance, you switch to GEICO. It's what you do.*~~

##Which shots did Kobe sink?

Kobe Bryant marked his retirement from the NBA by scoring 60 points in his final game as a Los Angeles Laker on Wednesday, April 12, 2016. Drafted into the NBA at the age of 17, Kobe earned the sport’s highest accolades throughout his [long career](http://www.npr.org/sections/thetwo-way/2016/04/13/474107238/kobe-bryants-life-and-career-by-the-numbers).

Using 20 years of data on Kobe's swishes and misses, can you predict which shots will find the bottom of the net? This competition is well suited for practicing classification basics, feature engineering, and time series analysis. Practice got Kobe an eight-figure contract and 5 championship rings. What will it get you?

##Acknowledgements

Kaggle is hosting this competition for the data science community to use for fun and education. For more data on Kobe and other NBA greats, visit stats.nba.com.


##Data

This data contains the location and circumstances of every field goal attempted by Kobe Bryant took during his 20-year career. Your task is to predict whether the basket went in (shot_made_flag).

We have removed 5000 of the shot_made_flags (represented as missing values in the csv file). These are the test set shots for which you must submit a prediction. You are provided a sample submission file with the correct shot_ids needed for a valid prediction.

**To avoid [leakage](https://www.kaggle.com/wiki/Leakage), your method should only train on events that occurred prior to the shot for which you are predicting!** Since this is a playground competition with public answers, it's up to you to abide by this rule.

The field names are self explanatory and contain the following attributes:

- action_type
- combined_shot_type
- game_event_id
- game_id
- lat
- loc_x
- loc_y
- lon
- minutes_remaining
- period
- playoffs
- season 
- seconds_remaining
- shot_distance
- shot_made_flag (this is what you are predicting)
- shot_type
- shot_zone_area
- shot_zone_basic
- shot_zone_range
- team_id
- team_name
- game_date
- matchup
- opponent
- shot_id
