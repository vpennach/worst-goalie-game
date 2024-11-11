# worst-goalie-game

This small project was inspired by watching a hockey game and witnessing one of the worst goalie performances ever so I asked the question what is the worst goalie performance ever.
You can be interpreted in many ways but I personally believe using the stat of xGoals (expected goals) from MoneyPuck.com is the best way to determine this.
Using MoneyPuck.com's data I wanted to find out who had the lowest GSAx in a single game. 

GSAx works by taking into account the quality of shots by the other team and assigning each shot on goal a percentage of the likelyhood of it going in. This is a much better indicator of goalie performance as opposed to just counting the shots on goal and looking at the goalies save percentage. 

This little coding project basically just sorts through the game data of every hockey game (since 2009) and finds the opposing teams xGoals and how many goals were allowed by a team. This will be able to give me a list of games sorted by whichever team had the worst GSAx (xGoals - Goals allowed). However this will not be able to tell the entire story of a game since MoneyPuck.com data does not take into account if a goalie was substituted out during the game, which is very likely to happen in all of these bad games. So I will have to search through the worst games on my own to find the individual goalies GSAx and not what it his for both goalies. Finally, I will also have to take into account if any empty net goals were scored during the game because that would also not go towards the goalies stats.
