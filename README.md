# Reviews' Sentiments of Mobile Banking Applications in Rwanda Before & After 2020

## Introduction

The last two years have caused a huge increase in cashless transactions. Many banks are commending their internet banking and mobile banking applications because not only they can save customers time but also they can help in coping with Coronavirus spread. I did the sentiment analysis of the users reviews of 10 different Android and iOS mobile banking applications from 10 different banks in Rwanda left on both Google Play Store and Apple Store before 2020 and after 2020 to see whether customers are leaving Negative or Positive reviews. The process involved getting reviews using the applications' IDs on Google Play and Apple Store respectively, processing the reviews (tokenization, correcting contractions and correcting spelling, lemmatization and removing non alphabetical characters, ...), checking the sentiment of the reviews using a combination of Textblob and Vader (the former uses the polarity and the subjectivity of the text while the later uses the emotion intensities associated with each lexical feature) and visualizing the results. 

## Ratings Over Time

Even though the first review date back in late 2012 most of the applications got their first reviews in 2016 or later. I decided to consider only reviews from January 1, 2017 to November 30, 2021. This analysis only shows the ratings given followed by a review note.

![monthly_average_rate](monthly_average_rate.png)

## SENTIMENT ANALYSIS

There are several methods to know whether a comment/review is positive, neutral or negative. In python two of some popular libraries that help help in sentiment analysis are [**Textblob**](https://textblob.readthedocs.io/en/dev/) and [**Vader**](https://github.com/cjhutto/vaderSentiment). The former uses the polarity and the subjectivity of the text while the later uses the emotion intensities associated with each lexical feature. Textblob is generalized while Vader is attuned to social media sentiments and can work with [**NLTK**](https://github.com/cjhutto/vaderSentiment) to provide sentiments on longer & tricky sentences that confuse other sentiment analysis tools.

### Samples

![positive_sample](positive_sample.PNG)

![negative_sample](negative_sample.PNG)

### Overall Distribution

![overall_sentiments](overall_sentiments.png)

> Overall, slightly more than a half of reviews are positive while 13% are classfied as Neutral.

### Sentiments by rating

![Sentiments_by_rating](sentiments_by_rate.png)

> Ratings of 3 or below are mostly dominated with negative reviews

### Sentiments Before 2020

![sentiments_before](sentiments_before.png)

> Before 2020, 62% of reviews were positive and only 24% were negative.

### Sentiments After 2020

![sentiments_after](sentiments_after.png)

> After 2020, positive reviews goes down to 46% while negative reviews increased to 41%.

## Conclusion & Future Work

Negative reviews increased from 24% before 2020 to 41% after 2020. Most negative reviews are associated with the rate of 3 or below.

The next step would be to check the upvotes of different sentiment, looking at reply/feedback rate to see whether the developers acknowledged negative feedbacks or provided help, and trying to classify/cluster the sentiment by topics. For example to see whether negative sentiments are associated with devices/os incompatibility, or some applications' features.

![summary](summary.png)

## References

https://github.com/JoMingyu/google-play-scraper

http://blog.manbolo.com/2012/09/10/useful-itunes-web-services

---
https://www.nltk.org/howto/sentiment.html

https://textblob.readthedocs.io/en/dev/
