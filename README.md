# Live_Twitter_Sentiment_Analysis

This project addresses the problem of sentiment analysis in twitter; that is classifying tweets according to the sentiment expressed in them: positive, negative, or neutral and find out anomalies.
For this topic is **"US Recession"**

_**Steps :**_
Project is created in three phases

**Phase I)**

1) Data Collection : Collected data with the help of twitter api keys.Use "Tweepy" for collecting data.
2) Data Preprocessing : It involves tasks such as removing stop words, punctuation, URLs, mentions, and hashtags. The data should also be converted to lowercase and tokenized.
3) Sentiment Analysis Model: Created sentiment analysis model  to classify tweets into positive, negative, or neutral based on polarity.
4) Evaluate Sentiment score : In this calculate sentiment socre of each post/tweet(Positive,negative and neutral) along with timestamp and stored in the database. For this Lexicon based analysis or hybrid approach is used.

**Phase II)**

For this , I collect 30 days of data(From 1-3-2023 to 30-3-2023) and take difference between present day and previous day and all generated into an heatmap.
For Calculating sentiment score following formulae used:

**diff_ss = (ss_old - ss_current)/TD**

where,
diff_ss = Differential Sentiment Socre
ss_old = Sentiment Score Of Previous Day
ss_current = Sentiment Score Of Current Day
TD = Time Difference

**Phase III)**

Anomalies were find by threshold_differnce.
Consider threshold_difference is 10
e.g If threshold_difference > diff_score then it is consider anomalie and if not then it will go on next date

_**Conclusion :**_

From this i got that  March 6-7,16-17,28-29 are anomalie days. On that days many incident happend like Bank of America shares,first republic bank stock down and Us Banks SVB and signature bank collapse and new rules are imposed. Also verify them on twitter app news also.

_**Inventive Step:**_
Use the differential of the sentiment score over a large period of time and analysis it to find the key events in past.

_**Purpose:**_
1) Understanding public opinion.
2) Detecting early warning signs of crises.
3) Improving customer service.
4) Marketing & Advertising.
5) Social media monitoring.
