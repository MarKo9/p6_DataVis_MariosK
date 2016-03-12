# P6 Data Visualizaiton: Koletsis Marios 

### Course Project for Udacity course 'Data Visualization and D3.js'

#### Summary

The data visualization is a bubble chart about the performance of Facebook Ads across 6 industries "Consumer Packaged Goods",  "Ecommerce" , "Automotive",  "Professional Services", "Retail" and "Technology" described by different colors. The comparison is based on 2 basic metrics; cost per click on the Y axis and relevance score* on the X axis. The performance is also compared against the average Daily budget displayed by the size of the bubble on the chart. 

They key takeaways are:

1.	First of all the clear negative correlation between the cost per click and the relevance score regardless of the industry of the advertiser. As suggested by Facebook the cost per click of an ad is decreasing proportionally as the relevance score of an ad is increasing and this suggestion can be confirmed.

2.	Another fact is the absent of any effect of daily budget on ad performance. Among the ads management professionals in many cases there is the conception that daily budget affects positively the overall performance while others believe that with smaller budget it is easier to get better results since the target audience is narrower and is expected to be more interested in an ad. 
Finding that there is no actual correlation I though that it is a good way to demonstrate that budget is not a variable that ad managers would be focusing for performance optimization and that it seems situation specific, I though it is an interesting fact to display. 

*Relevance score is calculated a metric provided by Facebook on the ads report and it is calculated based on the positive and negative feedback from its target audience on a an ad.

#### Design
The dataset includes performance metrics for CPM, Cost Per Click, Cost Per Link Click, Relevance Score, Industry, CTR and Daily Budget. After some EDA with R, I have decided that regardless of the industry, there is a clear negative correlation between cost and relevance score and. I have used Cost Per Click and Relevance Score for the x and y axis and color for the industries available.

Initially I was thinking to use a scatter plot (CTR_RS_plot_zoom.png) in order to show the trend among Cost Per Click and Relevance Score but as pointed out from one of my colleagues the trend was clear but the industry specific trends are difficult to follow so I have used instead a bubble chart with average values for all metrics and for each industry (feedback_1). 

Furthermore from another one of my colleagues, I have received the feedback that since Cost Per Click and Relevance Score are report metrics (show the performance of the campaigns after the ads have been lunched) I could have further added a setting metric (a metric that the advertisers decides prior to launching a campaign) in order to demonstrate its effect on performance, the daily budget (feedback_2). I did that by adding a third dimension for the daily budget displaying it by the size of the bubbles.


#### Feedback
Other that the two in person feedback, I have also addes a post on the forums (https://discussions.udacity.com/t/p6-data-visualization-feedback-request/158943) receiving feedback from 3 other persons. All of them have pointed out that it is difficult to understand want the size represents and its relationship on the other two metrics. For this reason I have added a title displaying this information and pointing the relationship between the Cost Per Click and Relevance Score and that the effect on the daily spend is up to the reader to discover. 
One of the comments mentioned also that the chart’s overall size was small making it difficult to read so I have resized and also used larger size on the labels and legends. 


#### Feedback memo:
The in person feedback has been collected from my colleagues and is recorded in audio file included on the github folder. Since I am working in Japan and for a Japanese company the feedback is in Japanese so I am giving a translation.
feedback_1: Matsuura_2016_02_29 15_02_17
“The correlation between the cost per clicks and the relevance score is clear but not the trend in each of the industries so I would suggest to use average values instead on absolute.”
feedback_2: Tsuruta_2016_03_02 13_29_42
“The trend showed among cost per clicks and the relevance score is clear but I would suggest to further add another, setting metric such as daily budget”


#### Resources
http://dimplejs.org/advanced_examples_index.html

