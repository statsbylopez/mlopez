---
title: 'Part II: Rethinking our playoff philosophy (on the role of chance in the postseason)'
author: ''
date: '2018-08-22'
header:
  caption: ''
  image: ''
slug: part-ii-randomness-of-series
tags:
- paired comparisons
- state space
- NBA
- NFL
- NHL
- MLB
categories: []
---

In the 2016-17 season, the Washington Capitals [dominated](https://www.washingtonpost.com/news/fancy-stats/wp/2017/02/09/this-is-the-most-dominating-washington-capitals-team-ever-so-whats-it-mean-for-the-cup/?noredirect=on&utm_term=.940cf4c44b8f) the NHL like few teams in recent history, winning the Presidents' Trophy with 118 points. 

The Caps entered a 2nd-round playoff series with Pittsburgh as decent-sized favorites (58 percent), and sure enough, Washington outplayed its rivals. In each of seven consecutive games, the Capitals outshot the Penguins, finishing with 70 total more shots on goal. 

Unfortunately for Washington, not enough shots turned into goals, and because hockey games are decided by goals, it was the Penguins that moved onto the Eastern Conference Finals. The Caps were sent home, with the early exit enough to drive NBC commentator Mike Milbury to the brink. 

"They have to rethink their whole philosophy," Milbury [suggested](https://twitter.com/StatsbyLopez/status/862503623565205504) after the game. 

I probably don't need to tell you what happened next. The Caps made a few changes to their roster -- call it a reconsidered philosophy -- enough so that by this year's 2nd-round, they were the [least likely](https://twitter.com/StatsbyLopez/status/990611488401510401) team among the eight remaining to raise a Stanley Cup. Despite those odds, Washington won its first title. 

"This Capitals team doesn’t have better talent than years past, but they have better focus and attitudes," Milbury argued. 

Washington's rise to the top of the NHL illustrates that, in hockey's postseason, surprising things can happen. In the rest of this post, I opine on what should and shouldn't be surprising in playoff competition, using the NHL, NBA, NFL, and MLB. 

## When does the better team win in the postseason? 

Let's start with some trivia.

**Two NBA playoff teams from the last decade are drawn at random and play one another in a "best-of-7" series -- what is the probability that the better team wins out?**

Turns out, it's about 80%. In other words, the best NBA team advances, on average, in roughly four of five series.

That's a pretty high number -- how does it compare to other sports? 

Given what we've learned in previous [posts](http://statsbylopez.netlify.com/post/part-i-randomness-of-games/), it's no shock to find out that both the NHL and MLB hover just above 60% in "best-of-7" formats, which is notably lower. However, let's switch that question just a bit:

**How long would postseason series need to be in NFL, MLB and NHL to match the NBA's "better team advances" rate of 80%?**

Here's what [Ben, Greg, and I found](https://arxiv.org/abs/1701.05976). 

- In the NFL, a "best-of-11" series is needed to match the NBA's better team advances rate.

- In the NHL, a "best-of-51" series is needed to match the NBA's better team advances rate.

- And in MLB, an astounding "best-of-75" series is needed to match the NBA's better team advances rate.

That is, if we wanted postseason formats to be equivalent across leagues, we'd need the NHL and MLB to do complete, and obviously ludicrous, overhauls.

## How can we compare one postseason format to another?

The NFL's never going to use a "best-of-7" format, nor is MLB going to use a "best-of-75" format. 

Instead, to better contrast each league, [Greg, Ben and I](https://arxiv.org/abs/1701.05976) derived a general metric that takes existing postseason formats (number of teams, rounds, games in each round, etc), mixed in our measurements of team strength, and identified how closely each league aligned with a completely deterministic model where the best team *always* advanced and won a title.  

Here's a plot that summarizes the equivalence of current postseason formats in each of the MLB, NFL, NHL, and NBA. Tournaments where the better team always advanced would score on the far right, while tournaments where every franchise had an equal chance in each round would show up on the far left. 

![](/post/2018-08-22-part-i-randomness-of-regular-season-competition_files/parity.png)

Unsurprisingly, the NBA stands out.* Better NBA teams more often advance, and the best NBA team more often wins out. 

Interestingly, the NHL, MLB, and NFL all somewhat overlap. In other words, each league's postseason structure roughly does a similar job of allowing better teams to advance.

## So what's this all mean?  

Well, here's where the list gets long.

1. The best team doesn't always win in the postseason in any sport. However, the best team is substantially more likely to win in the NBA than in any of the other three leagues.

2. Compared to our [regular season findings](http://statsbylopez.netlify.com/post/part-i-randomness-of-games/), the NFL is less aligned with the NBA in the figure above. However, there's an easy explanation -- the NFL's single elimination playoff format. Single elimination tournaments add noise -- it's why the NCAA hoops tournament is called March Madness, after all -- which decrease the chances that better teams advance. It's why the NFL frequently has champs that seem to come from nowhere, including the 2001 Patriots, 2007 Giants, and 2011 Ravens. In such instances, we shouldn't be surprised when NFL teams that seem like surprises win out. It's what happens in single elimination formats. 


3. Another subtle difference in the NFL: it's the only league where a team is generally not given home advantage in the title game/series. One of the best sports teams of all time -- the 2007 Patriots -- lost to the Giants on a neutral field in a one-game Super Bowl. Imagine the 2018 Warriors playing the Cavs for an NBA title in a one-game series in, say, Indianapolis? Yes, that'd be incredible theater. But it'd be incredible theater for the same reason that March Madness games are often incredible theater. The Warriors would be favored, but the Cavs' chances in such a set-up would increase by several orders of magnitude, relative to the current NBA format.

4. From a team's standpoint, understanding the inherent randomness of postseason outcomes is critical. Some examples:

- Last seed into the NHL, NFL, or MLB playoffs? You still have a chance. And that's worth playing hard for, because, in all likelihood, having the worst chance is still actually a reasonable chance. 

- Last seed in the NBA playoffs? Your work is cut out for you. 

-  Win a title? Congrats! Now check if you are one of the best teams. If you are, even better. But if you aren't the best team -- say, you are the 2013 Red Sox, which won after [getting every break in the book](https://statsbylopez.github.io/NESSIS2017_files/NESSIS_2017.html#how-often-does-the-best-team-win) against a more talented Tigers team -- don't simply bring back all of your players and think that lightning will strike twice. It usually doesn't -- the 2014 Red Sox, with largely the same pieces as in 2013, finished in last place in the American League East.

- Fail to win a title? Here's where an understanding postseason tournament formats is most critical. If you are one of the top teams, do your best to keep going. Convince folks internally how talented and skilled your team actually was. Don't be afraid to point out things like randomness and luck (or to show them this article). And don't do things like "rethink your whole philosophy." Though, in fairness, "don't do things that Mike Milbury says to do" shouldn't need so much math.

- Consider tweaks to current playoff formats. The NBA begins its playoffs with a "best-of-7" series between No. 1 and No. 8 seeds. Sweeps in these matchups are often more likely than *any* wins from the No. 8 seed. Meanwhile, MLB starts with a one-game play-in game and a "best-of-5" series between a No. 1 seed and roughly the equivalent of a No. 4 seed. In some years, however, MLB's No. 4 seed may be nearly as good as its No. 1 (that may happen this year with the Yankees). Altogether, MLB and NHL postseason formats don't do enough to reward good teams, while the NBA arguably does too much.**

- Stop the all-consuming allocation of credit and skill to teams that win titles and to teams that win titles alone. This is particularly biting in the MLB and NHL, where a third strike call or crossbar can make a difference between winning a ring and not winning one. 

- Conversely, labeling once-in-a-generation players as chokers isn't quite appropriate in sports where it's tougher to win in the postseason, as [Rolling Stone](https://www.rollingstone.com/culture/culture-lists/10-biggest-chokers-in-sports-history-108696/alexander-ovechkin-109184/) did in 2017 with Alex Ovechkin.

- Beware of snake oil when it comes to postseason predictions. If it seems to good to be true, it probably is. As a hypothetical example, if a company says it can predict MLB or NHL series outcomes with 85-percent accuracy, perhaps avoid hiring that company to be the official sponsor of your league's stats page.


## Summary

This post was long, but the varying formats and differing levels of league skill make postseason tournament outcomes in the MLB, NBA, NFL, and NHL complex to contrast. For team officials, coaches, players, and fans, an acknowledgement of the operating characteristics of each league can improve our overall understanding of how and when teams win in postseason play.  


*Footnotes*

*We likely underestimated the deterministic nature of the NBA in our article. To derive team strengths, we used regular season data. However, stars play a more dominant role in the NBA's postseason, which means it can be difficult to pick up on how teams like Golden State or Cleveland will improve from their regular season results.

**The NFL is perfect and that is an unbiased opinion.


*Note: This is Part II in a set of posts of how betting markets can inform sports fans. To return to the series homepage, click [here](http://statsbylopez.netlify.com/post/lessons-hidden-in-sports-betting-markets/).* 
