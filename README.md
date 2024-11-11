# worst-goalie-game

# Intro
This small project was inspired by watching a hockey game and witnessing one of the worst goalie performances ever so I asked the question what is the worst goalie performance ever.
You can be interpreted in many ways but I personally believe using the stat of xGoals (expected goals) from [MoneyPuck.com](https://moneypuck.com/index.html) is the best way to determine this.
Using MoneyPuck.com's data I wanted to find out who had the lowest GSAx in a single game.

GSAx works by taking into account the quality of shots by the other team and assigning each shot on goal a percentage of the likelyhood of it going in. This is a much better indicator of goalie performance as opposed to just counting the shots on goal and looking at the goalies save percentage.

This little project basically just sorts through the game data of every hockey game (since 2009) and finds the opposing teams xGoals and how many goals were allowed by a team. All I wanted to do was basically find a list of the worst GSAx in a single game, which is simply (xGoalsAgainst - goalsAllowed)

# Findings
In the data file you will see the raw data in all_teams.csv and then the filtered data which is just a list of the 50 worst games by GSAx. The intial finding was very interesting. out of literally 10s of thousands of games the single two worst every team performances according to GSAx occured within one month for the SAME TEAM. and they are.
**DET vs PIT on 03/27/2022 with -7.268 GSAx**
**DET vs TOR on 02/26/2022 with -7.15 GSAx**

This would be a much easier stat to find if teams did not pull their goalies during bad games. Because of this I had to go deeper into every single shot that each goalie in these games faced. Although Alex Nedeljkovic started both of these games all of those GSAx cannot be attributed to him. However, [MoneyPuck.Com](https://moneypuck.com/g.htm?id=2021021050) has an amazing feature where you can search individual games and see their advanced boxscores from those games.

After a quick search I found:
**Alex Nedeljkovic** on 03/27/2022 had a **-4.7 GSAx**
**Alex Nedeljkovic** on 02/26/2022 had a **-3.84 GSAx**

However, Alex was saved by his team pulling him since these two statlines are technically not the worst individual performance of a goalie. That award goes to **Kaapo Kahkonen** of the Minnisota Wild who gave up all 9 goals in his matchup against the St. Louis Blues where, on 04/09/2021 he recorded a record **-6.72 GSAx**.

This was good for the 4th worst game by GSAx, with the first two being mentioned above and the third was another game where the goalies split the GSAx.

# Conclusion
Basically all I did was manipulate some csv files to find a stat I was interested in, and again thanks to [MoneyPuck.com](https://moneypuck.com/index.html) for having such a good website to find this data. I am fairly confident this is the worst individual goalie performance since 2009 unless there is another instance where the backup goalie came in and performed extremely well in order to boost the teams GSAx enough to the point where it made up for the starting goalie.