---
layout: post
title: Lee's Post
---

# GO! CUBS! GO!

_By Lee Solo_  
_2018-10-15_

The Cubs are out of the playoffs (_there is always next year :smiley:_) and I am  done with the METIS Bootcamp Project Luther. The past two weeks went by so quickly didn't not have the time to realize how much I have learned in these weeks. Web scraping, Linear Regression, Lasso Regression, Ridge Regression WOW!!!  

During these past two weeks I was introduced to the world of web scraping and boy was it interesting. At first understanding the inner workings is a bit complex but with a little bit of patience and perseverance it is quite rewarding once you figure it out. In addition to web scraping a heavy dose if Statistical concepts were introduced to us that is important in the world of Data Science. The good thing about these past two weeks I got to incorporate my new found knowledge in my project.  

Project 2 was trying to predict run differential (difference between Runs scored vs Runs scored against) for the Chicago Cubs. This was a very good starting point for me to understand how data can be collected from the internet and used to create models using various statistical techniques. To scrape my data I used Beautiful Soup, luckily most of my data was in a table so it was not that difficult to scrape. I used [Baseball Reference](https://www.baseball-reference.com/)[newtab] which has most of the baseball statistics one would need. Given the amount of time I tried to keep my project quite simple using certain baseball metrics as my features. The reason I chose to look at baseball data since my goal is to predict what are the chances of the Cubs winning a night game. This project was a very good exercise on how to go about answering my final question (i.e. can I predict the chances of Cubs winning a night game).  

Most of my time was spent in cleaning my data that was quite messy once I got after scraping. In the future if there is any kind of data manipulation work or data cleaning my preferred choice will be SQL (Structured Query Language). It is much easier and quicker for me to do it in SQL rather than manipulating or cleaning data in a data frame (a.k.a. PANDAS).  

I used eight years worth of data which resulted in 1,297 observations and 21 features. Most of my features that I used were not used in a strategic manner. I used averages for player data (by year), schedule data and pitching statistics thinking that these metrics would be good features in predicting run differential. Boy was I wrong :smiley:.

I ran my dataset through multiple regression models. Starting off with splitting my dataset into train/test and using Linear Regression to determine if my model was overfitting or underfitting. At the same time I was also doing cross validation to my model. I used the Root Mean Square Error (RMSE) since this is in the same units as my prediction variable (i.e. run differential).  My model was overfitting therefore I had to use either Lasso or Ridge regression to correct my coefficients/betas.

I did a grid search cross validation to find the best hyper parameter for the Lasso and Ridge Regression. All the regression models gave me a very similar RMSE but I went with the Ridge model since Lasso will sometime get the feature coefficients to zero. Even though I used Ridge the features in my model were not good predictors of run differential. But that is fine, I know that in the future what baseball metrics not to use and what baseball metrics to use.

Overall this project has been rewarding because I learned a lot a new concepts that will help me create a more robust model in the future. As mentioned earlier this is just the beginning on learning how to model. My final question is yet to be answered (i.e. can I predict what are the changes of the Cubs winning a night game).


My next steps will be to bring in other features like opponent statistics, weathers, batting averages, daily lineups to mention a few. So stay tuned.

_To be continued..._
