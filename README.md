# Modelling-and-simulation-for-one-day-cricket
Given that only a finite number of outcomes can occur on each ball that is bowled, a discrete generator on a finite set is developed where the outcome probabilities are estimated from historical data involving one-day international cricket matches. The probabilities depend on the batsman, the bowler, the number of wickets lost, the number of balls bowled and the innings. The proposed simulator appears to do a reasonable job at producing realistic results. 

"""# **Dataset:**

1188 ODI matches -> odi.csv

**Each dataset consists of the following columns:**

- mid -> Each match is given a unique number
- date -> When the match happened
- venue -> Stadium where match is being played
- bat_team -> Batting team name
- bowl_team -> Bowling team name
- batsman -> Batsman name who faced that ball
- bowler -> Bowler who bowled that ball
- runs -> Total runs scored by team at that instance
- wickets -> Total wickets fallen at that instance
- overs -> Total overs bowled at that instance
- runs_last_5 -> Total runs scored in last 5 overs
- wickets_last_5 -> Total wickets that fell in last 5 overs
- striker -> max(runs scored by striker, runs scored by non-striker)
- non-striker -> min(runs scored by striker, runs scored by non-striker)
- total -> Total runs scored by batting team after first innings


**Prediction Algorithm and Accuracy:**

Algorithm Used:

*Random Forest Regression*

**Features and Label Used:**

Features: [runs,wickets,overs,striker,non-striker]

Label: [total] *italicized text*

**Accuracy in terms of [R Square Value,Custom Accuracy]:**

*ODI matches -> [79,77]*

*Note: Custom Accuracy is defined on the basis of difference between the predicted score and actual score. If this difference falls below a particular thresold, we count it as a correct prediction.*


"""
