---
title: 'Part I: Why I feel bad for Max Scherzer (on the game-level randomness in sports)'
author: ''
date: '2018-08-22'
header:
  caption: ''
  image: ''
slug: part-i-randomness-of-games
tags:
- paired comparisons
- state space
- NBA
- NFL
- NHL
- MLB
categories: []
---

The best team in baseball during the 2013 season was the Detroit Tigers. 

Detroit's rotation featured the eventual Cy Young award winner (Max Scherzer), alongside both the 2011 and 2016 Cy winners (Justin Verlander and Rick Porcello, respectively). The Tigers line-up was spearheaded by Prince Fielder and Miguel Cabrera, the latter of whom would win his second consecutive MVP. Indeed, betting market rankings had the Tigers atop the sport from [April through October](https://statsbylopez.github.io/NESSIS2017_files/NESSIS_2017.html#section-2). 

But on October 19th of that year, the best team in baseball was fighting to save its season. The Tigers trailed the Boston Red Sox three games to two in Game 6 the American League Championship series, with each of Detroit's losses coming by one run. Needing a win to force a game 7, Scherzer gave the Tigers a bit of hope, in the form of a 2-1 lead as the teams went to the bottom of the 7th inning. 

It's at that point in the game that the best team in baseball was also its unluckiest. 

It started with a runner on second, one out, and Xander Bogaerts at the plate. With a full count, Scherzer threw a pitch that umpires almost always call a strike 3.

![](/post/2018-08-22-part-i-randomness-of-regular-season-competition_files/xander.gif)

But instead of strike 3, home plate umpire Dan Iassogna called the pitch ball 4 (for the record, umps call pitches in that location a strike about six out of every seven times). And so instead of a runner on 2nd and two outs, the Red Sox now had two runners on and out out. Iassogna's call dropped the Tigers' win expectency by about 12\%. 

Next, Detroit reliever Drew Smily induced a chopper up the middle off the bat of Jacoby Ellsbury, hit in the direction of shortstop Jose Iglesias. It's the type of play Iglesias often starts a double play on. Worst, one would think, he'd record only one out.

![](/post/2018-08-22-part-i-randomness-of-regular-season-competition_files/jose.gif)

But Iglesias bumbled the ball, recording no outs and leaving the bases loaded. Allowing for one out on the play, the error was worth about a 20\% drop in win expectency for Detroit.

Scherzer and the Tigers, without a doubt, should've been out of the inning but for a few bad breaks. But they weren't, which allowed Shane Victorino to step to the plate with the bases loaded. Victorino's at-bat involved a little less luck; he hit a grand slam, and the Tigers season was effectively over. 

The Tigers' final game was heartbreaking, and indicative of one of the most humbling aspects of being a sports fan: the better team doesn't always win, even when it may deserve to. It happened for the Tigers in 2013, but it happens for all teams in all seasons and in almost all sports. Sometimes it's just luck -- a referee call, a bad bounce, poor conditions, or, like the Tigers, a missed strike three. Or sometimes the better team just plays poorly -- missing open three-pointers, field goals, saves, or, like the Tigers, easy ground balls up the middle. Or sometimes the "better" team might simply be so close in terms of talent to the "worse" team, that any number of plays, shots, or referee decisions could play into the game's outcome, actions that, by and large, are largely noise and not indicative of any particular skill or talent.

When Greg, Ben and I set out to compare North American sports, our principal goal was to consider how often, in each sport, the better team ended up winning. Here's our main take-home, which summarizes the game-level randomness of each league.

![](/post/2018-08-22-part-i-randomness-of-regular-season-competition_files/parity2.png)

On the far left, the NHL and MLB games cluster closer to coin flips; that is, if we were to randomly take a game between two randomly drawn teams, it's less likely that the best team will win. As referenced above, part of this is luck -- one can surmise that given the low amounts of scoring involved in baseball and hockey, more breaks are needed to win -- but a related part of it is also because the best teams in the MLB and in the NHL can still lose to the worse teams and fans wouldn't be *that* surprised. The gaps in talent in those leagues are, at least relatively, not as wide. 

Alternatively, the NFL and NBA roughly live in a world halfway between coin-flips and pre-determined outcomes. 

Our findings are somewhat unique. There's a whole literature on competitive balance that's out there, with which we are only in partial agreement. For example, though tempting, answering a question like ours [can't be done using win percentages](https://www.vox.com/videos/2017/6/5/15740632/luck-skill-sports), because win percentages are effected by things like schedule strength and number of games. 

And our findings highlight the immense power of betting market data which, when combined with a statistical modeling framework the can account for changes to team strength, allows us to capture league-level and team-level traits that have, to-date, mostly been unknown. 

Scherzer's bad break is but one anecdote behind several ways in which our work can inform decision makers. 

Indeed, here's a list of several questions that, when armed with betting market information and an understanding of probability, one can answer. 

1. Looking at the standings to determine team strength? Stop -- you can do better. Our betting market metrics of how good each team is are better predictors of future won-loss percentage than current won-loss percentage is. In other words, if you look at the standings, and I look at betting market data, I'll have more accurate predictions of the rest of the season that you will (and I don't even have to know win percentage to make that claim). 

1a. Afraid of our modeling? Use Mike Beuey's ratings at [Inpredictable](http://www.inpredictable.com/). Bookmark his site. Market ratings like this are more on point than just about any public metric out there, and certainly better than standings or most power rankings. The data's that good. If you want to know how good a team is, check to see when it's a favorite or when it's an underdog. 

2. The traditional mechanism by which we evaluate teams — wins and losses - can belie characteristics vital to understanding team strength. Here's some specific ways that decision makers can use betting market information. 

- Is your team going to make the playoffs? Start with betting market data, estimate probabilities for each game and each team, simulate the rest of the season, and find out.

- Should you trade for a certain player? Compare how betting odds for this player compare when he is and isn't in the line-up. It's an easy, back-of-the-envelope estimate of how valuable a player is.

- Should you fire a coach? It's tempting to use winning percentage here. But if your team wasn't that good, or if it played a challenging schedule with several road games, you may want to check how betting markets have viewed how good your team actually has been. 

- What are your chances of winning a title if you do make the playoffs? Simulate the postseason (hint: I'll do that in my next post)

3. On a league level, understanding how gaps in team strength have widened or narrowed can be used to better explore topics like parity, attendence, and fan interest. As examples, does increased or decreased game uncertainty leads to more interest?  How much higher are TV ratings when games are closer?

Altogether, at critical moments in a team’s evolution, we recommend that teams look past wins and losses to better understand team strength in the context of their own league. And for fans, perhaps the knowledge that NHL and MLB games are so close to coin flips can both (i) provide a modicum of comfort when your favorite team falls or (ii) a glimmer of hope when a game is about to start and your team is an underdog. 


