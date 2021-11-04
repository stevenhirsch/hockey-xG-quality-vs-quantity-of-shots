# Hockey xG Quality versus Quantity of Shots Analysis

A pertinent tactical question in territory sports is whether a higher amount of low-quality shots at goal versus a lower amount of high-quality shots at goal results in different probabilities of winning a match. The expected goals (xG) a team accumulates during a game (soccer, for example) reflect their weighted quality and quantity of shots. For example, suppose Team A and Team B accumulated the same xG of 2.0. Team A amassed this xG in 10 total shots (low quantity, high quality). In contrast, team B did so in 15 shots (high quantity, low quality). Is Team A more likely to win than Team B, or are their probabilities of winning identical since they've accumulated the same xG? We can begin to answer this question by assessing the expected points (xPTS) the two teams earned based on their distribution of xG.

It is already reported in soccer that teams with a lower amount of high-quality shots are more likely to win the match than teams with a higher amount of low-quality shots. An aphorism in ice hockey, another territory sport, is to "get pucks at the net" without much emphasis necessarily on the quality of the shot. It is often frowned upon to pass the puck excessively to create higher-quality shot opportunities, especially during a power play, if it comes at the expense of attempting more shots.

However, the points awarded for winning and losing are allocated differently in soccer versus hockey. Therefore, the results from soccer can't be extrapolated directly and raise a question regarding whether the same relationship exists in ice hockey. The purpose of this analysis was to assess whether a lower amount of high-quality shots results in higher xPTS relative to a higher amount of low-quality shots in hockey. I hypothesized that a lower amount of high-quality shots would accumulate more xPTS than a higher amount of low-quality shots due to the xPTS findings from soccer. Further supporting this hypothesis is the current trend in basketball to prioritize shooting three-point shots to improve the probability of winning.

In this analysis (located in the Colab notebook), Team A accumulated 33% fewer shots than Team B. I simulated 1,000 potential games, each with varying xG accumulation ranging from 1.0 to 7.0. I simulated each match 10,000 times for a total of 10 million simulations. A problem I ran into with point allocation was when a game was tied after regulation and went into overtime. I modelled the 3-on-3 overtime (and shootout) as a coin flip. I decided to model it this way because I didn't think it was fair to assume, based on the xG accumulated in regulation time, which team is more likely to win.

The findings supported my hypothesis since Team A accumulated significantly more xPTS than Team B. Therefore, there is a strong argument that teams are more likely to win an ice hockey match by generating a lower quantity of high-quality chances than their opposition, so long as their total xG isn't impaired. However, the effect isn't as apparent in ice hockey as it is in soccer. Regardless, this finding has exciting applications for team building, tactics, and general hockey strategy (e.g., perhaps we want to "overload" talent onto one line to prioritize high-quality chances). However, there are limitations to consider of this work when applying it to practice. For example, it might be easier to defend against teams that are explicitly waiting to generate high-quality chances and not take opportunities for lower-quality shots. I do think this project created more questions than answers. Answering these future questions requires communication with domain-specific experts and perhaps more "real world" data.
