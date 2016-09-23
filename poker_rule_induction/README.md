#[Poker Rule Induction](https://www.kaggle.com/c/poker-rule-induction)


##Determine the poker hand of five playing cards

Your friend bailed last minute on poker night? Before giving up on a much-needed evening of bad bluffs and quarter buy ins, light a cigar and get familiar with the rules of the game. Each record in this competition consists of five playing cards and an attribute representing the poker hand. You are asked to predict the best hand you can play based on the cards you've been dealt. 

![ScreenShot](dogs_playing_poker.jpg)

The order of cards is important, which means there are 480 possible Royal Flush hands instead of just four. Identify those, and the other 311,875,200 possible hands correctly, and you’re in the money!

*"Isn't this easy? I know two-of-a-kind when I see it"*, you might rightfully wonder.


##Data

In this competition, you are going to predict which business a user is checking into based on their location, accuracy, and timestamp. 

![ScreenShot](kaggle_screenshot.png)

The train and test dataset are split based on time, and the public/private leaderboard in the test data are split randomly. There is no concept of a person in this dataset. All the row_id's are events, not people. 

And you'd be right. **The intent of this challenge is automatic rules induction, i.e. to learn the rules using machine learning, without hand coding heuristics.** Pretend you are in a foreign land, have never played the game before, are given a history of thousands of games, and are asked to come up with the rules. It is potentially difficult to discover rules that can correctly classify poker hands, yet it is trivial for a human to validate the rules objectively. Remember, your algorithm will need to find rules that are general enough to be broadly useful, without being so broad that they end up being occasionally wrong. We suggest reading the [paper](http://www.wseas.us/e-library/conferences/crete2002/papers/444-494.pdf) by Cattral et al. for more background on the topic.

Playground competitions are an opportunity to build and stretch your machine learning muscles. Pull up a chair to the data science poker table and ante up.


##Acknowledgements

Kaggle is hosting this competition for the machine learning community to use for fun and practice. This dataset was created by Robert Cattral and Franz Oppacher. We also thank the UCI machine learning repository for hosting the dataset. If you use the problem in publication, please cite:

*Bache, K. & Lichman, M. (2013). [UCI Machine Learning Repository](http://archive.ics.uci.edu/ml/). Irvine, CA: University of California, School of Information and Computer Science*