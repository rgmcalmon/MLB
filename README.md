# Examining Potential Umpire Bias in Major League Baseball

We started with review of research done by Christopher A. Parsons, Johan Sulaeman, Michael C. Yates, and Daniel S. Hamermesh on potential racial bias exhibited by umpires in Major League Baseball in 2004-2006. In short, their research stated that when the race of the umpire matched the race of the starting pitcher, the umpire was more likely to call a strike. Additionally, this particular effect was only seen in stadiums where there was no electronic review of the calls made by umpires. In 2004-2006, approximately 35% of games had electronic monitoring of calls.

## Our Data

We pulled game data for 2013-2015 from https://www.baseball-reference.com

We identified the urls for each game id
*Loop through each game to pull
*The home plate umpire name
*The pitch sequence
*The pitch count of balls and strike
*The pitcher name
*The batter name
*Boolean of whether or not the pitcher is the ‘home’ pitcher
*The inning
*The run difference

We pulled 2014 player (pitcher) racial data from https://www.besttickets.com/blog/mlb-players-census/

We identified any other pitchers from 2013, 2014, & 2015 who were not in 2014 census data and manually identified their race (based on google image search). For pitchers whose race was unclear to the initial evaluator, another group member was asked to evaluate.
*Races used: asian, black, hispanic, white

We Identified home plate umpires race from 2013, 2014, & 2015 manually using google image search. For umpires whose race was unclear to the initial evaluator, another group member was asked to evaluate.

## Our Hypothesis

There will be a difference in the number strikes called when the race of the home plate umpire matches the race of he pitcher.

Null: There will be not be any difference in the number of strikes called when the race of the home plate umpire matches the race of the pitch.

## Our Analysis

Logistic Regression was performed to evaluate the potential effects of umpire and pitcher race on the whether or not there were called 'balls' or 'strikes'.

## Results

Overall, we were unable to reject the null hypothesis, meaning that we cannot say that called strikes made by umpires is impacted by the race of the umpire or the pitcher.

However, when using fixed effects when the umpire was black there was a p value of .049, suggesting....

Furthermore, when using fixed effects where the umpire was 'non-white' (black or hispanic) there was a p value of .088. And when using fixed effects where the pitcher was 'non-white' (asian, black, or hispanic) there was a p value of .063. While this does not fall under the more desirable 95% confidence it does fall under 90% confidence and is an interesting finding.

## Conclusions