# Mots-Pour-Les-Mauts-Environmentale
Supplementary Information for Project "Not God, Not Even Science?! Towards Peace in the Twitter War for 'Climate Change'

# General outline of the v1a pipeline, for further detail see Causalityv1.py: 

0. First, query by keyword and classify pro-and-contra climate change tweets. Then, query for the authors of pro- and contra- climate change tweets, and filter for authors with number of tweets >30,000 tweets and account age >5 years.  Do this until a quota of prolific pro and contra climate change twitter users is found.
1. Do some manual selection, to verify classificaiton and make sure authors are indivuals
2. Collect tweets of the selected authors.
3. Generate semantic networks using collected tweets.
4. Analyze the semantic networks using concepts from psychoanalysis and cognitive science.

# Files: https://drive.google.com/drive/folders/1UXxWsZTSJbTWZBoyiLAcFHX0l0bqiA2h?usp=drive_link 

Main Code:
Causalityv1.py - Code used to gather the data. Its analysis portion was not used, instead relying on the semantic network code of https://nocodefunctions.com/

Transformer model Classifier:
BertClassifierCode_v1a.ipynb - The code used to train a 4-label (pro/contra/news/other) climate-change tweet classifier model.
twitter_sentiment_data.csv - The labeled tweets to train the classifier
cleaned_twitter_sentiment_data - The same as twitter_sentiment_data.csv but with stopwords removed from the tweets
TrainedBertTweetModel - The trained classifier model.

The aggregated data for analysis, resulting from main code:
contra_first*.csv & pro_first*.csv - The aggregated tweets used to produce the 8 semantic networks (using NoCode Functions) which I showed in class 

Saved Environment from Main Code, containing until just after the last use of Twitter API:
EnvironmentWithCompleteMainDict.spydata - The saved environment with collected data/variables of up to step 4 of Causalityv1.py. 
EnvironmentWithCompleteMainDict_*.npy - The saved arrays from the same environment, which for some reason saved as a different file.

