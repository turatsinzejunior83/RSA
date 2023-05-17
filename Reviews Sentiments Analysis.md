Reviews' Sentiments of Mobile Banking Applications in Rwanda Before & After 2020
Introduction
The last two years have caused a huge increase in cashless transactions. Many banks are commending their internet banking and mobile banking applications because not only they can save customers time but also they can help in coping with Coronavirus spread. I did the sentiment analysis of the users reviews of 10 different Android and iOS mobile banking applications from 10 different banks in Rwanda left on both Google Play Store and Apple Store before 2020 and after 2020 to see whether customers are leaving Negative or Positive reviews. The process involved getting reviews using the applications' IDs on Google Play and Apple Store respectively, processing the reviews (tokenization, correcting contractions and correcting spelling, lemmatization and removing non alphabetical characters, ...), checking the sentiment of the reviews using a combination of Textblob and Vader (the former uses the polarity and the subjectivity of the text while the later uses the emotion intensities associated with each lexical feature) and visualizing the results.

Ratings Over Time
Even though the first review date back in late 2012 most of the applications got their first reviews in 2016 or later. I decided to consider only reviews from January 1, 2017 to November 30, 2021. This analysis only shows the ratings given followed by a review note.

![image](https://github.com/turatsinzejunior83/RSA/assets/45234656/74cbce24-5708-4660-a14d-d364c6d81aed)
SENTIMENT ANALYSIS
There are several methods to know whether a comment/review is positive, neutral or negative. In python two of some popular libraries that help help in sentiment analysis are Textblob and Vader. The former uses the polarity and the subjectivity of the text while the later uses the emotion intensities associated with each lexical feature. Textblob is generalized while Vader is attuned to social media sentiments and can work with NLTK to provide sentiments on longer & tricky sentences that confuse other sentiment analysis tools.

Samples
![image](https://github.com/turatsinzejunior83/RSA/assets/45234656/015be632-2198-4ba7-b7b2-327d2e702a26)
Overall Distribution
![image](https://github.com/turatsinzejunior83/RSA/assets/45234656/27c75187-8742-46e9-8d49-b3e128fa1a4b)
Overall, slightly more than a half of reviews are positive while 13% are classfied as Neutral.

Sentiments by rating
![image](https://github.com/turatsinzejunior83/RSA/assets/45234656/cce3e21a-8e5a-43b7-98ca-d25e610a38ab)
Ratings of 3 or below are mostly dominated with negative reviews

Sentiments Before 2020
![image](https://github.com/turatsinzejunior83/RSA/assets/45234656/97bba877-bff4-4d14-ad19-1e108bdf8c61)
Before 2020, 62% of reviews were positive and only 24% were negative.

Sentiments After 2020
![image](https://github.com/turatsinzejunior83/RSA/assets/45234656/2141ad2b-18b9-435c-afb3-b5ef943fdafc)

After 2020, positive reviews goes down to 46% while negative reviews increased to 41%.

Conclusion & Future Work
Negative reviews increased from 24% before 2020 to 41% after 2020. Most negative reviews are associated with the rate of 3 or below.

The next step would be to check the upvotes of different sentiment, looking at reply/feedback rate to see whether the developers acknowledged negative feedbacks or provided help, and trying to classify/cluster the sentiment by topics. For example to see whether negative sentiments are associated with devices/os incompatibility, or some applications' features.
![image](https://github.com/turatsinzejunior83/RSA/assets/45234656/e1ae70ee-e4d6-4483-b3af-3099154bbc15)
![image](https://github.com/turatsinzejunior83/RSA/assets/45234656/7fafca5e-827c-421b-84de-3a88ec6f902d)

References


1.https://github.com/JoMingyu/google-play-scraper

2.http://blog.manbolo.com/2012/09/10/useful-itunes-web-services

3.https://www.nltk.org/howto/sentiment.html

4.https://textblob.readthedocs.io/en/dev/
