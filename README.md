# P6 Data Visualizaiton: Koletsis Marios 

### Course Project for Udacity course 'Data Visualization and D3.js'

#### Summary
This is a visualiztion of the baseball dataset - average hit rate is plotted against home run count, with each point representing a player - the points are coloured by handedness of each player. There is also a barplot of the average batting averages for each type of handedness. The scatterplot clearly shows that there is a correlation between average hit rate and home run count, but the relationship is not linear - players with a higher hit rate tend to get far more home runs than those with a low rate. More interestingly, the barplot shows that left-handed and both-handed batters tend to have better batting averages than right-handers.

#### Design
The dataset includes statistics on handedness, height, weight, batting average, and home run count. After some exploration of the data in Rstudio, I decided that height and weight didn't tell much of a story. I did find a relationship between hit rate and home runs, so plotted these on the x and y axes. As handedness is a factor with only three levels, it was easy to represent by colouring the points of a scatterplot accordingly.

Based on the initial feedback I received, I decided to use d3 to make the points smaller and slightly more transparent after drawing the chart. Initially, I could only get the transparency to work, but found a stackoverflow post with the same issue, which suggested using setTimeout() to get the radius change to work as well.

When I initially submitted the project, my evaluator suggested looking more closely at the impact of handedness on performance. I then spent more time exploring the data, and realised that left/both handed players tended to perform better than right handed ones. As this relationship is not clear from the scatterplot, I decided that the best way to show it would be a barplot with the average batting average for each type of handedness. I felt that it was worth keeping the scatterplot to show the wide variation in performances, but worth adding the barplot to make the main point of the story (performance difference for types of handedness) more obvious to the viewer.

After further feedback, I decided to change the colourscheme. Originally I had just used default colours, but I decided that the red and orange were too similar, so switched to more saturated versions of red, green and blue, which were much easier to differentiate between. I also used the same colours for the barchart, as I felt that the consistency would help the viewer see the connection between the two visualizations of the data.

#### Feedback
I posted a thread in the class forum (https://discussions.udacity.com/t/final-project-feedback-baseball-player-performance/33777) and received feedback from one person there. I also showed the visualization to two people in person, who didn't have any data science experience, but both raised the same issue about distinguishing between points.

I then submitted the project, and was told to go back and look again at the relationship between handedness and performance.

After making some changes, I submitted my second draft to the forum for more feedback (https://discussions.udacity.com/t/final-project-feedback-baseball-performance/37690). I received suggestions from two members, including making the colours more distictive (which I used and expanded on) and adding a text summary (which I did). They also suggested making the barchart smaller, however I disagreed, as I think that it shows the most interesting aspect of the dataset. One user suggested that I look at average home runs per game - I agree that this would be interesting, but unfortuantely the dataset doesn't include this information, or the number of games each player had played in order to calculate it.

#### Resources
dimple.js documentation
stackoverflow: http://stackoverflow.com/questions/22836594/dimple-js-change-radius-of-circles
