---
name: Final Project 3
tools: [Python, HTML, vega-lite]
image: assets/pngs/final_visualization.png
description: This is the final project part 3.1 from group 22
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---

# NBA Player Statistics Analysis 2021-2022

### Group 6

Zhizhou Xu, Yeting Qi, Jindi Zhang

In this study, we would like to analyze the points per game for each team in NBA 2021-2022 games. The data we referred to is from NBAstuffers.com and the data can be found through this link: https://www.nbastuffer.com/2021-2022-nba-player-stats/.

## Contextual Visualization Ⅰ

<vegachart schema-url="{{ site.baseurl }}/assets/json/PPG_position.json" style="width: 100%"></vegachart>
This visualization demonstrates the mean points per game categorized by each position. For people who are not familiar with the NBA games, one of the important things to understand is the positions in the game. Knowing the positions would help them understand the structure of the game. There are several positions in basketball: C(center), G(guard), F(forward). Forward positions are closer to the basket, then the Center, and then the Guard. In our study, some players have two positions, such as “F-G”. This means that this player’s primary position is forward, but he also plays in Guard positions. As our graph shows position “F-G” has 18 mean points per game which is leading among all positions. This is expected because the forward position is the closest to the goal and also it has more points due to rebounds (points awarded to a player who retrieves the ball after a missed field goal or free throw). The reason we think why F-G has more points per game than F position is because it is hard for a player to play F-G because it pretty much covers the whole court and it’s harder. If a player plays F-G position, the player is usually very good and is probably in the top tier in terms of his overall performance. For other positions, the mean points per game are about the same because their positions are not as ideal to gain a field goal then a forward position would.

## Contextual Visualization Ⅱ

<vegachart schema-url="{{ site.baseurl }}/assets/json/PPG_AGE.json" style="width: 100%"></vegachart>
This visualization demonstrates the mean points per game of each age. This would help us better understand a team’s performance. By comparing the points per game with player’s age, we could see at what age the players are generally at their peak capability. This would also give us an idea of how a player is expected to perform, and how a team is expected to perform based on the team’s overall age. In the line graph, we see that there are two peak time periods. The first one is from age 26 to 28, and the second one is from age 32 to 35. Our explanation to the first peak is that from age 26 to 28, the players are at their peak body capacity. They have better physical ability and better reaction compared to some older players. The second peak from age 32 to 35 is older than we think, however it does make sense after careful analysis. The players are still actively playing in NBA at this age usually indicates that they are already good players, which is why they have a longer career. In addition, they would have a more stable mindset and more experience in the game, which allows them to play “smarter” with better decisions. The low mean points per game from age 29 to 31 can be explain by their lowering of the physical capacity and less game experience. This is a period when the age advantage slowly fades, but the experience has not been enough to support them for more field goals. According to our study, we would expect a team to perform better if they have more players in the age range 26 to 28 and 32 to 35.

<vegachart schema-url="{{ site.baseurl }}/assets/json/Team_PPG.json" style="width: 100%"></vegachart>
We choose to create a dashboard with a heatmap on the left and a bar graph on the right. For a person who is not familiar with our dataset, we want them to understand how points per game is distributed between players and team. The heatmap on the left shows the points per game versus each team. The bin number we chose is every 5 points because we think this will accurately separate the player’s performance. The interactive feature is brush and selection. The user can brush and select any region on the heatmap, and correspondingly the bar graph on the right would show the points per game versus the number of players in that points interval. By looking at the dashboard, the audience who don’t have much experience with NBA would be able to roughly understand how much points do each player get in a season. By analyzing this visualization along with our two contextual visualizations, the audience could understand some factors that affect a team and a player’s overall points per game. Overall, we can conclude that points per game range 0 to 10 has the most player counts. A player peak performance is in the age range 26 to 28 and 32 to 35. The position that has the most mean points per game is position F-G.

<!-- these are written in a combo of html and liquid -->

<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/DaBaLxx/DaBaLxx.github.io/main/_data/NBA_Stats_202122_All_Player_Statistics_in_one_Page.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/DaBaLxx/DaBaLxx.github.io/blob/main/python_notebooks/group-6-final-project-3.ipynb" text="The Analysis" %}
</div>
