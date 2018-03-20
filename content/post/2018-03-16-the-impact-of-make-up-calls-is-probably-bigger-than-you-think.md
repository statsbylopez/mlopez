---
title: The impact of make-up calls is probably bigger than you think
author: ''
date: '2018-03-16'
slug: the-impact-of-make-up-calls-is-probably-bigger-than-you-think
categories: []
tags:
  - NHL
  - make-up calls
  - GAM
header:
  caption: ''
  image: ''
---


One of the more reliable indicators of which NHL team is likely to get the next power play has little to do with score or style of play. Instead, it's been shown repeatedly ([Ex 1](https://fivethirtyeight.com/features/hockey-refs-are-out-to-get-you-if-they-already-got-the-other-guy/), [Ex 2](http://people.stat.sfu.ca/~tim/papers/penalty.pdf)) that referees call a substantially higher number of make-up penalties than would otherwise be expected in order to maintain an overall even number of violations on each team. Call it a [*biased impartiality*](https://creativematter.skidmore.edu/cgi/viewcontent.cgi?article=1004&context=math_fac_schol) -- in order to appear impartial by game's end, ref's let previous decisions drive future ones. 

A common line of reasoning behind call reversals is that referees would prefer to $not$ be part of the final narrative as to why a particular team won or lost. If each team has a relatively similar number of power plays, media and fans clamoring that one team was favored would have less support. Turns out, however, that by evening up penalty calls, hockey ref's are impacting the same game narratives that they are trying to avoid being a part of. In this post, I'll both confirm the existance of make-up calls and extend a similar analysis to look at the impact of make-up calls on game outcomes.

## The make-up call

Claiming that a call in any sport is due to anything besides an unbiased referee assessment is a non-trivial task. Fortunately, hockey boasts several settings that make looking for make-up calls somewhat feasible. Game's are often tied, and looking at penalties in tied-game states can avoid results being impacted by changes in style of play due to the score. Second, with an average of about eight minors a game, there's a large enough sample size within each game on which to evaluate ref choices. And finally, as the overwhelming majority of hockey infractions are at the referee's discretion, subtle cues -- such as previous penalty decisions -- can impact most calls.  

Here's an initial chart showing how future penalty calls are linked to current penalty differential.[^1] The x-axis uses the home team's estimated pre-game win probability, as implied by betting markets (you can get that data [here](https://github.com/bigfour/competitiveness)). The y-axis shows the penalty differential for the home teaem after the first period (positive means more penalties), and the shade of the chart corresponds to the average penalty differential in periods 2 and 3. Only games that were tied at the end of the first period are included in this chart (the data goes from the 05-06 to 15-16 regular seasons).

![](/img/makeupF1.png)

When home teams have two more infractions than their oppononent at the end of the first period, they can expect, on average, about 0.8 fewer infractions the rest of the game. Alternatively, when home teams have two fewer penalties at the end of the first period, they average about 0.5 more violations in periods 2 and 3. The difference between having more and fewer penalties in tied games is quite significant. Of course, if you had read a few of the links above, you probably would have guessed that there would be an impact. But the effect size (about 1.25 penalties), as well as the shading of the chart above, seemed noteworthy.

## The impact of the make-up call

Make-up calls are all well and good until somebody loses a game because of it. 

One game that I remember all-too-well came during the 2011 Cup finals between Vancouver and Boston. In Game 5, the home Canucks were called 

To check how future games are impacted by make-up calls, I replicated the same chart. In this one, however, the shade reflects the percent of games eventually won by the home team.[^2]

![](/img/makeupF2.png)

In this version, the shading is reversed -- more first period penalties are linked to an increased win rate, just as fewer penalties are linked to a decreased win rate. Altogether, when the game is a relative toss-up, the difference between having two more first period penalties and two fewer first period penalties is about 7 or 8 percentage points in terms of the home team's chances. 

While this may seem like a relatively minor change, the fact that there's $any$ change in win percentage based on prior penalties is interesting. 
Additionally, we may be underestimating the impact of make-up calls -- if a team has first period penalties, it's also more likely to start the second period on the penalty kill, a quirk that I did not account for above that could lower that team's win rate. Further, this isn't a peculiar set of games  -- about a third of NHL games end the first period tied. Finally, although it'd require further assumptions with respect to playing style, it's also likely that make-up calls have an impact on games that aren't tied. 

One limitation of this and most of sports analytics is that, in using observational data, we can never be assured that something else isn't responsible for our finding. One alternative theory here is that teams who have taken penalties suddenly feel a need to be more aggressive, which then leads to the call reversals. However, in using tied games, I can't imagine that the revenge factor looms too large. Further, in [previous work](https://creativematter.skidmore.edu/cgi/viewcontent.cgi?article=1004&context=math_fac_schol), if anything, penalty reversals were higher in the postseason, where there is almost no expectation of revense. 

[^1]: I used a generalized additive model (GAM) of penalty differential as a factor of both home team win probability and first period penalty differential. In this and the example below, first period penalty differential was a significant predictor. GAMs make sense in this and other examples, as the true model fit with penalty outcomes is unknown.

[^2]: Same model as above, now with a binary outcome. 

