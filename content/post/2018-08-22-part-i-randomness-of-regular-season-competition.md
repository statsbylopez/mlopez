---
title: 'Part I: Randomness of regular season competition'
author: ''
date: '2018-08-22'
slug: part-i-randomness-of-regular-season-competition
categories: []
tags:
  - paired comparisons
  - state space
  - NBA
  - NFL
  - NHL
  - MLB
header:
  caption: ''
  image: ''
---


One of the most humbling aspects of being a sports fan is that the better team doesn't always win. 

It could happen for a few reasons. The better team might get unlucky, whether it's a missed foul call or bad bounce. The better team might play poorly, missing open three-pointers, field goals, or easy saves. Or the "better"" team might simply be so close in terms of talent to the "worse" team that any number of plays, shots, or referee decisions could play into the game's outcome, actions that, by and large, are largely noise and not indicative of any particular skill or talent.

When Greg, Ben and I set out to compare North American sports, our principal goal was to consider how often, in each sport, the better team ended up winning. Though tempting, answering a question like this [can't be done using win percentages](https://www.vox.com/videos/2017/6/5/15740632/luck-skill-sports), because win percentages are effected by things like schedule strength and number of games. But it can be done with the help of a statistical modeling framework, in particular one that picks up on factors like the home advantage, relative team strength, and changes in team strength over time. And it can be done with betting market data, which when combined with our modeling framework, can provide unbiased, low-variance estimates of how good each team is at a particular point in time.

Here's our main take-home, which summarizes the game-level randomness of each league.


![](/img/parity2.png)

On the far left, the NHL and MLB cluster closer to coin flips; that is, if we were to randomly take a game between two randomly drawn teams, it's less likely that the best team will win. As referenced above, part of this is luck -- one can surmise that given the low amounts of scoring involved in baseball and hockey, more breaks are needed to win -- but a related part of it is also because the best teams in the MLB and in the NHL can still lose to the worse teams and fans wouldn't be *that* surprised. The gaps in talent in those leagues are, at least relatively, not as wide. 

Alternatively, the NFL and NBA roughly live in a world in between coin-flips and pre-determined outcomes. 

Here's what decision-makers in sports should be aware of: 

1. Betting market metrics of team strength are better predictors of future won-loss percentage than current won-loss percentage. Is your team going to make the playoffs? Should you trade for a certain player? Should you fire a coach? What are your chances of winning a title if you do make the playoffs? All questions where the use of betting market data -- in terms of how it can assess team strength -- is more appropriate than using traditional, public metrics. Meanwhile, the traditional mechanism by which we evaluate teams — wins and losses - can belie characteristics vital to understanding team strength. 

2. Similar metrics can also be used to better understand opponent strength. Worried about a team catching you for a playoff spot? Simulate the rest of the season, which is easy to do when you have estimates of team strength and variability. 

2. On a league level, understanding how gaps in team strength have widened or narrowed can be used to better explore topics like parity, attendence, and fan interest. As examples, does increased or decreased game uncertainty leads to more interest?  How much higher are TV ratings when games are closer?

Altogether, at critical moments in a team’s evolution, we recommend that teams look past wins and losses to better understand team strength in the context of their own league. And for fans, perhaps the knowledge that NHL and MLB games are so close to coin flips can both (i) provide a modicum of comfort when your favorite team falls or (ii) a glimmer of hope when a game is about to start and your team is an underdog. 


