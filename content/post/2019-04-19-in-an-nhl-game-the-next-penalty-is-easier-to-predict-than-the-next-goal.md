---
title: In an NHL game, the next penalty is easier to predict than the next goal
author: ''
date: '2019-04-19'
slug: next-nhl-event
categories: []
tags:
  - NHL
  - penalties
header:
  caption: ''
  image: ''
---

It's NHL playoff season, which means that, given the relative [league parity](https://arxiv.org/abs/1701.05976), every call and no-call will come under the microscope. In the third period of close games, for example, a penalty call alone could increase or decrease a team's chance of winning by [10 percentage points](http://moneypuck.com/g.htm?id=2018030174) or more. 

One characteristic of NHL games that a few prominent members of the media [have picked up on](https://twitter.com/domluszczyszyn/status/1116450841022488576) is that penalty calls tend to "even-up" -- that is, it is unlikely that either team ends the game with a substantially larger number of penalties than its opponent. [Kevin and I](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=2259798) (as well as a few others ([ex 1](http://people.stat.sfu.ca/~tim/papers/penalty.pdf), [ex 2](https://www.researchgate.net/publication/274325288_Reversal_of_Fortune_A_Statistical_Analysis_of_Penalty_Calls_in_the_National_Hockey_League))) have covered this in depth over the last few years. 

But a fun comparison I thought to make would be that, instead of the analyzing the impact of penalty differential alone, let's compare penalty likelihood to goal likelihood. That is, given goal and penalty information from earlier in the game, compare the chance that the next goal is scored by the home team to the chance that the next penalty is called on the home team.

Using all games from 2005-2016, here's the likelihood that the first penalty is called on the home team (left plot) and the first goal is scored by the home team (right plot) after the second period begins, given both the goal and penalty differentials in the first period. 


![](/img/nhlpens.png)

Two aspects stand out. 

First, the rates shown in the penalty plot are both more extreme and show more consistent of a pattern than in the goal plot. If you want to predict the first penalty of the second period, that's likely an easier task than predicting the first goal. Second, much of the differences in the goal plot are driven not by goal differential, but by penalty differential. Thinking more broadly, we've long known that score effects impact NHL team behavior -- I wonder if part of this is due to the fact that score effects are somewhat of a proxy for penalty differential.

Technical postscripts: 

1. I stopped after the 2016 only because I don't have a clean pbp data-set to match the nhlscrapR version I used before. If anyone wants to update, I'd be curious to see the results. A comparison of regular and postseason games could also be warranted. 

2. A smart observer would point out that one could improve a goal prediction model by including characteristics of each team. However, including team specific factors is unlikely to have as much of an impact on a penalty prediction model. Perhaps a future post.  



