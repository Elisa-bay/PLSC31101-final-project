# PLSC31101-final-project

## Short Description

This code creates a dataset of @RealDonaldTrump's most recent 1000 tweets, taking into account whether Twitter has flagged the tweet as mis- or dis-information or not. It then conducts a time series analysis by day and by week, a popularity analysis with favorites and retweets, and a word frequency analysis to compare flagged tweets and unflagged tweets.

## Dependencies

1. R, 4.0.2
2. Package - tidyverse
3. Package - rtweet
4. Package - lubridate
5. Package - ggplot2
6. Package - tm
7. Package - wordcloud

## Files

1. Narrative.Rmd: Provides a 3-5 page narrative of the project, main challenges, solutions, and results.
2. Narrative.pdf: A knitted pdf of Narrative.Rmd.
3. Bayoumi_Lightnight_Talk.pptx: Slides for my lightning talk.

#### /

1. Narrative.Rmd: Provides a 3-5 page narrative of the project, main challenges, solutions, and results.
2. Narrative.pdf: A knitted pdf of 00_Narrative.Rmd. 
3. Bayoumi_Lightnight_Talk: Your lightning talk slides, in whatever format you prefer.

#### Code/
1. 01_collect-nyt.R: Collects data from New York Times API and exports data to the file nyt.csv
2. 02_merge-data.R: Loads, cleans, and merges the raw Polity and NYT datasets into the Analysis Dataset.
3. 03_analysis.R: Conducts descriptive analysis of the data, producing the tables and visualizations found in the Results directory.

#### Data/

1. Trump_Tweets_flagged_unflagged: The created dataset after evaluating the first 997 tweets from @RealDonaldTrump on November 9th to December 10th for flagged content.

#### Results/

1. time_series_day.pdf: Graph of unflagged vs. flagged tweets over the collected time by day
2. time_series_week.pdf: Graph of unflagged vs. flagged tweets over the collected time by week
3. Retweets_faves_flagged_v_unflagged.pdf: Graph of favorites (upper two lines) and retweets (lower two lines) of collected flagged vs. unflagged @RealDonaldTrump tweets
4. Wordcloud_frequent_in_flagged_tweets.pdf: Word cloud of most frequently used words in flagged @realdonaldtrump tweets and not non-flagged tweets
5. Wordcloud_frequent_in_untagged_tweets.pdf: Word cloud of most frequently used words in non-flagged @realdonaldtrump tweets and not flagged tweets

## More Information

Results are spesific to how many tweets you get. Tweets selected were from November 9th, 2020 to December 10th, 2020. 

A bug in RTweet may require rerunning the get_timeline() code several times until enough tweets are collected for analysis.

Contact: ebayoumi[at]uchicago.edu

Thank you for visiting!
