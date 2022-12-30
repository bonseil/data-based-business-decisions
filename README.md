# data-based-business-decisions
A/B testing for an online store

## Project description

We are a big online store. The Covid pandemic has greatly increased the number of people that regularly make their purchases online, but it has also increased the already tough competition between online stores.<br>
In this situation the marketing and the IT department compiled a list of hypotheses that might help to boost the revenue and let us stay afloat of the competition.
<br>
As the company's data analyst, I have to prioritize these hypotheses, launch an A/B test, and analyze the results. 

## Project instructions
   - Open and look through the data file. Path to the file:datasets/users_behavior.csv Download dataset
   - Split the source data into a training set, a validation set, and a test set.
   - Investigate the quality of different models by changing hyperparameters. Briefly describe the findings of the study.
   - Check the quality of the model using the test set.
   - Additional task: sanity check the model. This data is more complex than what you’re used to working with, so it's not an easy task. We'll take a closer look at it later.

## Data description
### *hypotheses_us.csv*
<ul>
  <li><i>Hypotheses</i> — brief descriptions of the hypotheses </li>
  <li><i>Reach</i> — user reach, on a scale of one to ten</li>
  <li><i>Impact</i> — impact on users, on a scale of one to ten</li>
  <li><i>Confidence</i> — confidence in the hypothesis, on a scale of one to ten</li>
  <li><i>Effort</i> — the resources required to test a hypothesis, on a scale of one to ten. The higher the Effort value, the more resource-intensive the test.</li>
</ul>
### *orders_us.csv*
<ul>
  <li><i>transactionId</i> — order identifier </li>
  <li><i>visitorId</i> — identifier of the user who placed the order</li>
  <li><i>date</i> — of the order</li>
  <li><i>revenue</i> — from the order</li>
  <li><i>group</i> — the A/B test group that the user belongs to.</li>
</ul>
### *visits_us.csv*
<ul>
  <li><i>date</i> — date </li>
  <li><i>group</i> — A/B test group</li>
  <li><i>visits</i> — the number of visits on the date specified in the A/B test group specified</li>
</ul>

## Project instructions
### Part 1. Prioritizing Hypotheses
    * Apply the ICE framework to prioritize hypotheses. Sort them in descending order of priority.
    * Apply the RICE framework to prioritize hypotheses. Sort them in descending order of priority.
    * Show how the prioritization of hypotheses changes when you use RICE instead of ICE. Provide an explanation for the changes.

### Part 2. A/B Test Analysis
Analyze the A/B test:

    * Graph cumulative revenue by group. Make conclusions and conjectures.
    * Graph cumulative average order size by group. Make conclusions and conjectures.
    * Graph the relative difference in cumulative average order size for group B compared with group A. Make conclusions and conjectures.
    * Calculate each group's conversion rate as the ratio of orders to the number of visits for each day. Plot the daily conversion rates of the two groups and describe the difference. Draw conclusions and make conjectures.
    * Plot a scatter chart of the number of orders per user. Make conclusions and conjectures.
    * Calculate the 95th and 99th percentiles for the number of orders per user. Define the point at which a data point becomes an anomaly.
    * Plot a scatter chart of order prices. Make conclusions and conjectures.
    * Calculate the 95th and 99th percentiles of order prices. Define the point at which a data point becomes an anomaly.
    * Find the statistical significance of the difference in conversion between the groups using the raw data. Make conclusions and conjectures.
    * Find the statistical significance of the difference in average order size between the groups using the raw data. Make conclusions and conjectures.
    * Find the statistical significance of the difference in conversion between the groups using the filtered data. Make conclusions and conjectures.
    * Find the statistical significance of the difference in average order size between the groups using the filtered data. Make conclusions and conjectures.
    * Make a decision based on the test results. The possible decisions are: 1. Stop the test, consider one of the groups the leader. 2. Stop the test, conclude that there is no difference between the groups. 3. Continue the test.
