---
layout: post
title: A New Scoring System
---

A tremendous number of videogames, especially in the past, have used a “highscore” system to give feedback on how well a player did in the game. The idea is to always strive to score better than the current highscore, at which point your score becomes the new highscore for the game, which in turn you will try to surpass on future plays.

There are a few advantages that scoring systems have. Their wide range of outcomes gives good feedback to the player about which strategies are effective or ineffective, and they can also accommodate players of many skill levels, since the extremely good or bad players will be able to notice increases and decreases in score more than marginal winrate gains, like .5% to 1% winrate or 99.6% to 99.9% winrate.

People in my circles have spoken much about flaws with the highscore system, and with scoring systems as a whole. If you aren’t familiar with their criticisms, here’s a quick recap:

1. Because the only point is to score beat the current best score, as scores get higher and higher, only extremely risky, extremely high payoff strategies become viable. Once someone successfully executes a very risky strategy, the only way to outscore them is to adopt a higher payoff strategy, which is probably much riskier if the game in question has any sort of risk management at all.

2. In many cases, the longer a specific game lasts, the more points are scored. As a result, at the highest scoring levels, the game begins to last an exorbitantly long, completely wasting the player’s time.

3. Much of the time, trying for a high score involves replaying boring or trivial parts of the game over and over again waiting for things to line up during the difficult part.

4. After the highscore is beaten, for some reason the game doesn’t end, and the player is stuck playing without a goal. Should they try and score as high as possible? Should they try and beat the highscore by the lowest amount possible so that beating it the next time is as easy as they can make it? Who’s to say?

5. Finally, and maybe most universal, having a huge range of possible end states makes it almost impossible to have longer arcs that stop precisely when the game is finished, which contributes to more homogenous play. With well-defined events centered around the win state, the game can support diverse longer arcs.

So, in light of the problems with the traditional highscore systems, we’ve moved on to what I like to call the goal + ranking system. Each individual match has some sort of goal that’s supposed to be reasonably easy to achieve at the player’s skill level. Then, there’s a system of “ranking points” outside the matches that measures how often the player is winning and adjusts the difficulty of the matches to the best possible level.

While the goal + ranking system solves all of the problems with the highscore system, it gives worse feedback, since marginal winrate changes are harder to parse than changes in score. It simply gives less feedback on the whole compared to a scoring system, since “did I win: yes/no” is less precise than “how many points did I get?”.

That brings me to another system that I’ve contrived, which I believe has all the best aspects of the highscore system and the goal + ranking system. I call it the score + ranking system, and it entails a match-based structure in which the player scores points and then subsequently the game updates the player’s ranking based on the number of points scored. Each match is assigned difficulty based on the rank that the player had when they entered, just as it is in the goal + ranking system. This system has the advantage of finer grained feedback that the highscore system has, and also solves many of its problems:

1. The player is trying to maximize the score, not the probability of passing a certain score threshhold, so it's unlikely that extremely risky strategies would come to dominate like they do in traditional highscore systems.

2. Since there's no highscore in any meaningful sense, the designer can scale the points and set up a score "par" (or score needed to break even on ranking) that keeps match length in check, preventing it from spiraling out of control like it does in highscore systems.

3. Because of the match structure, the game can be designed to challenge the player throughout the match, rather than forcing the player to replay the already-beaten beginning of the game each time they want to play the later parts.

4. Due to the lack of highscore, there's no question of what to do after the highscore is beaten. Instead, the player can focus on maximizing the expected value of the number of points scored throughout the match, knowing that as long as the game is in progress what they're expected to do is clear.

### But what about arcs?

On the surface, it seems like the score + ranking system doesn’t solve the lack of structure that is present in the highscore system. While it’s true that there’s no easy way to tie match structure to win condition (since there is no win condition), there’s still one remaining way to confer structure onto each match: tying the arcs of the match to the loss condition instead.

I’d like to talk more about tying structure to loss conditions right now, but the fact is that thinking about loss conditions and designing around them is relatively unexplored, even in the specific game design community that I'm a part of. It’s common to use a “enemy hits u” system or a “u run out of time” system even in the best designed games I’ve encountered. Loss conditions are something that I think needs more attention, and that I plan to write about further on this blog once I have better ideas about them. Until then, it’s hard for me to prescribe techniques for structuring arcs around loss conditions.

Come to the [Dinofarm Discord](https://discord.gg/8PPwfDY) or [Dinofarm Forums](http://www.dinofarmgames.com/forum/index.php) to further the conversation about game design.
