## MinneMUDAC Data Science Competition

### Introduction

The challenge was to predict the voter turnout for Democrats, Republicans, and third-party candidates for each of Minnesota’s eight Congressional districts, as well as for both Senate seats and the race for Governor.

Read more about the problem statement [here](https://carlsonschool.umn.edu/news/msba-team-wins-2018-minnemudac-case-competition?utm_source=msba&utm_medium=linkedin_organic&utm_campaign=events_minnmudacwinners).

Have a look at our final [presentation](MinneAnalytics.pdf) for a quick summary of our results.

It was one of the most challengeing data science problems I have tackled as no data was provided, we had to go get our own data and secondly there is no right way to tackle partisan voter turn out so we had to come up with our own methodology after doing a lot of research.

### Key Takeaways

1. Good data - I feel that sometimes this is taken for granted, especially in data science competitions. It really forces you to think deeply about the problem you are trying to solve.
2. Research - We did a lot of research
3. Think out of the box - 


### The Challenge

The challenge was to investigate the factors/characteristics that influence the number of voters who would cast a ballot in the 2018 Minnesota elections, and predict the number of votes that will be cast for each party (Democrat, Republican & Independent) for the 8 Congressional Districts, the governor and the 2 senate seats of Minnesota. This amounts to a total of 33 predictions [(8 + 2 + 1) x 3].

### Datasets

Part of the challenge was to find our own data. We looked at a number of different variables, including education, race, and income and how those translated to party affiliation and likelihood to vote.


We started by researching factors that could affect voter turnout and party inclination. The golden source for any demographic data in any country is the census, wherein a team of hard working people count and write down characteristics of every individual in the country. This herculean task is only done once in every 10 years and within a span of 10 years the congress changes 5 times and demographics vary drastically. The United States Census Bureau also does an annual survey on a sample population, called the American Community Survey and uses this sample demographic data to estimate the demographic data across the country. Not the most accurate data for our problem but we decided to go ahead with this.

Once we obtained the past 10 years of demographic data for each of the 8 congressional districts in Minnesota from the American community survey, we discussed what other data points could affect voters. We added historical voting data, campaign financing, pre-polling surveys and twitter sentiment data of candidates.

One complication with the application of a turnout estimate to the survey sample is the fact that election polls tend to overrepresent politically engaged individuals. 

incumbency
The incumbent’s margin of victory in his or her previous election, 
Fundraising, based on the share of individual contributions for the incumbent and the challenger as of the most recent filing period
the political experience level of the challenger
districts are also “swingier” (or more elastic) than others

Next, we realized that we have over 100 features or columns and this data is only available for the past 10 years (rows) for each congressional district. This means we have more variables then observations and in such a case the predictive problem would not have a unique solution unless it is further constrained. That is, there may be multiple (perhaps infinitely many) solutions that fit the data equally well. Such a problem is called 'ill-posed' or 'underdetermined' and can lead to overfitting.

We looked at a number of different variables, including education, race, and income and how those translated to party affiliation and likelihood to vote. But there were also factors such as candidate fundraising, how popular they were, and whether or not they were an incumbent that we had to factor into our model.

 However, factors affecting turnout are not always easy to measure.

“It was difficult for teams to account for differences in turnout due to the current political climate,

sentiment analysis using python on election candidates’ twitter profiles to call close races

### Clustering

To solve this challenge, we leveraged the K – Means clustering algorithm to find 10 similar districts in the United States for each of the 8 congressional districts in Minnesota based on demographic and political profile, increasing the number of observations (rows) ten-fold. 

states are demographically similar.
It uses a k-nearest neighbors algorithm to identify similar congressional districts based on a variety of demographic,11 geographic12 and political13 factors. 


### Predictions

This might be the most straightforward part where we had to build a prediction model. The 2018 elections could see the highest turnout for a midterm since the mid-1960s

evaluate the teams on several factors, including data preparation, creativity, methods, communication of results, and team synergy. The accuracy of their model and predictions of turnout also were factored into their scoring. 

Have a look at our final [presentation](MinneAnalytics.pdf) for a quick summary of our results.

### MinneMUDAC 

MinneMUDAC, now in its third year, is a partnership between MinneAnalytics and the Midwest Undergraduate Data Analytics Competition (MUDAC). Read more about the competition [here](http://minneanalytics.org/students-use-data-to-predict-voter-turnout-at-minnemudac-2018/) and [here](


