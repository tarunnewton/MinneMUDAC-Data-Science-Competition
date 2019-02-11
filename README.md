## MinneMUDAC Data Science Competition

### Introduction

The challenge was to predict the voter turnout for Democrats, Republicans, and third-party candidates for each of Minnesota’s eight Congressional districts, as well as for both Senate seats and the race for Governor.

Read more about the competition [here](https://carlsonschool.umn.edu/news/msba-team-wins-2018-minnemudac-case-competition?utm_source=msba&utm_medium=linkedin_organic&utm_campaign=events_minnmudacwinners).

Have a look at our final [presentation](MinneAnalytics.pdf) for a quick summary of our results.

It was one of the most challenging data science problems I have tackled for two main reseason, firstly as no data was provided, we had to research and get our own data and secondly there is no right way to tackle the problem of predicting voter turn out for each party so we had to come up with our own methodology which included a lot of trial and error.

### Key Takeaways

1. Good data - The old “garbage in, garbage out” adage is true here, it is impossible to solve a data science problem with bad data. I feel that sometimes this is taken for granted, especially in data science competitions. Collecting your own data really forces you to think deeply about the problem you are trying to solve. 
2. Research - We did a lot of research especially since for many of us it was our first experience of the election process in the US. I feel that successful research lies in iteration: we should return again and again to the key questions, methods, and data, which then leads to new ideas, revisions, and improvements.
3. Think out of the box - We should not get stuck on just collecting endless data or trying to improve the performance of the existing model by trying different algorithms and parameter settings but every once in a while really think about where and why the current approach is failing and what can be done to improve that. This kind of thinking was critical to the success of our project.
4. Communication - It’s not enough just to have the technical know-how to analyze data, create predictive models, and so on – communication skills are equally important. You must be able to explain effectively how you came to a specific conclusion and be able to rationally justify your approach. For us being able to convince our audience who were from very diverse backgrounds (college data science professors to business professionals) that our results make sense was key.

### The Challenge 

The challenge was to investigate the factors/characteristics that influence the number of voters who would cast a ballot in the 2018 Minnesota elections, and predict the number of votes that will be cast for each party (Democrat, Republican & Independent) for the 8 Congressional Districts, the governor and the 2 Senate seats of Minnesota. This amounts to a total of 33 predictions [(8 + 2 + 1) x 3]. Teams were evaluated on several factors, including data preparation, creativity, methods, communication of results, team synergy and the accuracy of their model and predictions of turnout. 

### The Data Challenge

Part of the challenge was to find our own data and this was probably the most difficult and time-consuming. We initially read a lot of research papers on what could be the driving factors and then looked at a number of different variables, including education, race, and income and how those translated to party affiliation and likelihood to vote.

The main source for any demographic data is the census, as is only done once in every 10 years, we decided to move to the American Community Survey where the United States Census Bureau does an annual survey on a sample population and uses this sample demographic data to estimate the demographic data across the country. It is the most accurate data but we decided to go ahead with this.

Once we obtained historical demographic data for each of the 8 congressional districts in Minnesota we looked at other possible factors. We added pre-polling surveys but one complication with the survey sample is the fact that election polls tend to overrepresent politically engaged individuals. Then we looked at fundraising, based on the share of individual contributions for the incumbent and the challenger as of the most recent filing period, the political experience level of the challenger, voter registration, incumbency, the incumbent’s margin of victory in his or her previous election.

We also did a sentiment analysis on election candidates which we felt was very useful in especially the Senate races because there were two seats up for election and with most other factors being the same this helped differentiate the candidates.

### Clustering

As elections happen very infrequently and we didn't want to use data that was very old we were restricted to the sample size we had to train our model. To solve this challenge, we used clustering to find similar districts in the United States for each of the 8 congressional districts in Minnesota based on their demographic and political profile, increasing the amount of data we had to train our models.

### Predictions

This might be the most straightforward part where we had to build a prediction model. We used a two model approach where we first directly predicted the voter turn out for each party by using a multi-output regression model and then combined those results with another set of models which first predicted the overall turn out  and then used a classification model on top of that to get the predicted votes cast for each party.

Have a look at our final [presentation](MinneAnalytics.pdf) for a quick summary of our results.

### About MinneMUDAC  

MinneMUDAC, now in its third year, is a partnership between MinneAnalytics and the Midwest Undergraduate Data Analytics Competition (MUDAC). Read more about the competition [here](http://minneanalytics.org/students-use-data-to-predict-voter-turnout-at-minnemudac-2018/).

