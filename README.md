# How To Be A Better Chess Player

## Authors and Github Links
- Alden Chan (https://github.com/AldenCh)
- Nicholas Panait (https://github.com/NicholasPanait)
- Victor Ma (https://github.com/waachaa)
- Saffron Birch (https://github.com/SaffyTaffy)

## Introduction
The contents of this report cover our analysis of over 20,000 chess games played on [Lichess](https://lichess.org/) compiled into a dataset by [Mitchell Jolly](https://www.kaggle.com/datasnaek) on [Kaggle](https://www.kaggle.com/datasnaek/chess). Our analysis encompassed the pre-processing and cleaning of our data, allowing us to investigate the influence of 12 attributes on various aspects of the game. Some examples include move count, which side you’re playing, opening choice, and how the game ended. Finally, we summarized our findings in a conclusive report, defining expected outcomes based on certain attributes.

## Discussion
&nbsp;&nbsp;&nbsp;&nbsp; Throughout our data analysis, we discovered a few key factors that affect the overall outcome of the game.  The first analysis we did was on which side (white or black) was more likely to win a game of chess.  We found that white had a 4.26% higher chance of winning compared to black.  We also found that the average number of turns in a game (not including draws) was roughly 61.2. In the games where white won, the average number of turns was 60. In comparison games where black won had 62.5 average number of turns. Using this information, to have a higher chance of winning you would want to play as white, while utilizing a strategy that will take less than 61 turns.  On the other hand, if you are playing black, you can still have the upper hand if you use a strategy that takes longer than 61 turns.<br>

&nbsp;&nbsp;&nbsp;&nbsp; From our analysis of openings and their play rates, we found that the most popular openings typically had far fewer moves. A likely reason that this pattern occurs is that as an opening has more moves, there are more opportunities to disrupt it, meaning that part way through the opening the player may be forced to use a different variation/strategy. Another more evident reason why openings with more moves are played less frequently is that they may incorporate early sacrifices to gain an advantage later on.  These types of openings are typically only used by players who are very skilled at the game, allowing them to pull off more difficult and complex openings compared to the average chess player.  The final reason that openings with more moves are played less often could be because the opening is just a joke and has no advantage (like the Bongcloud Attack).<br>

&nbsp;&nbsp;&nbsp;&nbsp; When looking at the play rates of each opening we discovered that openings with more variations are played more often than those with fewer or none.  When an opening has many variations, it means that although the start will be the same, the opening can branch off with many different subsequent moves. An opening with more variations is more likely to be played since more variations mean more versatility. Openings with more options allow players to adapt to their opponent's moves more effectively, especially since most players will only learn to play about 3 openings.<br>

&nbsp;&nbsp;&nbsp;&nbsp; Using our analysis of the openings and their win rates, we discovered that common openings have an equal distribution of wins between white and black, whereas the less common openings tend to favor one or the other.  Although some openings may be more beneficial to one side compared to the other, the more likely cause of this finding is that the lesser-played openings don’t have enough data to determine their viability.<br>

&nbsp;&nbsp;&nbsp;&nbsp; When analyzing the risk factor of each opening, we found that the less common an opening is, the higher the risk it is.  The risk that was used for these openings was their viability for use on both white and black, meaning a higher-risk opening would be skewed to one side.  Using this knowledge, new players should try to learn common openings first, as they are just as viable on both black and white.  Finally, if you can learn multiple different openings, knowing which ones benefit which side can provide a significant advantage over your opponent.<br>

&nbsp;&nbsp;&nbsp;&nbsp; The winrates of each opening vary greatly depending on which side they are played from, these findings confirm the hypothesis that openings were designed for certain sides and created to build an advantage through a series of strategic moves at the beginning of the game.<br>

The top 3 highest win rate openings for white were:
- The Queen’s Gambit
- Philidor Defense #3
- Scandinavian defense.

The top 3 highest win rate openings for black were:
- Van’t Kruijs Opening
- Sicilian Defense
- Queen’s Pawn Game.


## Conclusion
&nbsp;&nbsp;&nbsp;&nbsp; In conclusion, we found many different factors that can affect the winrate of a chess game.  The first factor we identified was which side the player was on, with white being the preferred side as it had a higher win rate.  The second factor was the number of turns you should take, with games under 61 turns favoring white and games over 61 turns favoring black.  The last factor that we analyzed was the different openings and their variations.  We found that the more popular an opening is, the more even it will be in terms of win rate.  This means that a less common opening will be much more likely to either favor white or black, although there is a possibility this is due to there being less data compared to the popular openings.  Lastly, we found that openings with fewer variations and more moves were much less popular than ones with less moves and more variations.

&nbsp;&nbsp;&nbsp;&nbsp; While completing this assignment, we learned many things about chess such as what side and openings are the most advantageous.  We also learned interesting things such as what openings are better for white/black and how variations and complexity affect the popularity of an opening.  For the future, an improvement that we could make would be to add more to the questions to further refine the data gathered.


## Acknowledgements
&nbsp;&nbsp;&nbsp;&nbsp; This project was submitted as the final course project for CSCI 2000U “Scientific Data Analysis” during Fall 2021. The authors certify that the work in this repository is original and all appropriate resources are rightfully cited.”

## Steps to Run our Jupyter Notebook
1. Install [Docker](https://docs.docker.com/engine/install/ubuntu/) and [Docker Compose](https://docs.docker.com/compose/install/) on Ubuntu or [WSL](https://docs.microsoft.com/en-us/windows/wsl/install)<br>
2. Clone the necessary Docker files using git in your preferred directory:<br>
&nbsp;&nbsp;&nbsp;&nbsp; - Using HTTPS Authentication with PAT: **git clone https://github.com/maakemi/csci2000u-jupyter-notebook**<br>
&nbsp;&nbsp;&nbsp;&nbsp; - Using SSH Authentication: **git clone git@github.com:maakemi/csci2000u-jupyter-notebook**<br>
3. Change into the cloned directory<br>
4. Run the following two commands in your terminal<br>
&nbsp;&nbsp;&nbsp;&nbsp; - **sudo service docker status**, NOTE: If docker is already running then there is no need for the second command<br>
&nbsp;&nbsp;&nbsp;&nbsp; - **sudo docker service start**<br>
5. Open up a new Ubuntu or WSL terminal and run **sudo docker run hello-world** to make sure docker works<br>
6. Start the container with **sudo docker-compose up** to start the Jupyter environment and you will be given URLs that you can use in any browser to access the environment<br>
7. Upload our Jupyter Notebook to your Jupyter environment and click it to run the notebook in a new tab<br>
8. Click the two right-facing arrows that look like a fast-forward button in the toolbar at the top to run the entire notebook<br>
