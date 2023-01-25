# Can you predict a tennis player's career earnings based on their profile?

**Contributors:** Shariq Imran Hassan, Nelson Li, Sanidhya Singh, Logan Hale

**Project Goal:** Formulate a Predictive Question and answer it using a simple classfier and regression model

## Introduction
For our project we will analyze player stats for the Top 500 tennis players. Tennis is a racket sport played on courts everywhere. Some major tournaments include Wimbledon, US Open, Australian Open, and French Open. Our dataset contains a variety of information including the player’s age, handedness, name, height, seasons, etc.

In this project, we aim to answer the following question:

### Can you predict a tennis player's career earnings based on their profile?
<br>

We believe that this question is important for sports agents and tennis players so they have a greater ability to predict their future earnings. Sports agents are paid based on how much their clients (the athletes) make, so it would be very beneficial for them to have some ability to predict this amount. It will also be useful for players to be able to predict their future earnings and determine what factors have a large impact on their earnings. If they understand what factors have the biggest impact on their earnings they will be able to set goals for themselves and be set up for monetary success.

## Discussion/Analysis

We compared the total earnings of tennis player's with multiple parameters such as Age, Current Rank, Best Rank, and Seasons Played. We ran a KNN regression on each parameter and tested multiple K-values to reach the best and most accurate predictor of Career Earnings. As shown above, in both Seasons Played, Age and Career Earnings had a weak positive relationship. This was as expected since Seasons Played and Age are both related to each other as well. Current Rank and Best Rank both revealed an inverse relationship with Career Earnings. Once again, this was as expected since a higher rank can reasonably be associated with a prize money amount.

After trial and error, we concluded that the overall Best Rank was the most accurate and reasonable predictor of total career earnings. Using Best Rank, we were able to attain the smallest RMSPE of all parameters compared with K = 4. While Age and Seasons Played both displayed a weak relationship, Current Rank was another contender for the best predictor. However, the Current Rank led to a reasonably larger RMSPE value than the Best Rank as shown in Table 3.1.

Initially, we had expected that Best Rank would be the best predictor for the total Career Earnings as prize money is usually dependent on the number of sponsors a player can get as well as their popularity. It is reasonable to assume that players who rank higher are more popular and more commercially viable than players with lower ranks. We had also expected that Best Rank would be inversely related to Career Earnings. Both of our initial hypotheses were supported by our findings.

After analyzing each predictor variable, we concluded the best rank to be the optimum indicator for a player’s expectation of their total Career Earnings. Since this is the case, it should serve as motivation for athletes to achieve the highest rank possible as it seems to have the strongest relationship with prize money and thus be the most accurate (smallest expected error) predictor. We presume any athlete would want to know how to reach financial independence knowing how short their careers last and as well as knowing how a critical injury/occurrence can impact their career drastically, albeit impacting them financially as well. These findings bring valuable insight and a much clearer view for tennis athletes and their agents who have such mindsets where they can now understand how to extract the most out of the sport financially. They can set clear goals in their mind to achieve a top 100 or top 50 rank. Looking at the Best Rank Prediction Plot (bottom left of Figure 3.1) we can observe that prize money increases exponentially as your best rank decreases. Hence these findings can help tennis athletes to visualize and understand their future goals for their tennis career.

These findings give rise to other questions related to or building upon this study such as:

1. What other variables affect career earnings in tennis?

2. What combination of predictor variables will produce the smallest RMSPE?

3. Does a player's likability (in modern social media) affect career earnings?

4. Does the tennis prize money model work the same in men’s tennis and women’s tennis?

5. Can tournaments win be a better predictor for this model?

6. How does tennis’s prize money model compare with other sports' prize money models?

7. Can we correlate prize money (more specifically tournaments won) to sponsorship money, hence creating a model where we understand how tournaments won impact sponsorship money?
