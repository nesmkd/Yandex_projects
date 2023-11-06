# Description of project - Revenue growth and AB testing
## Research Goals
Prioritize and test hypotheses for increasing revenue in the online store. Also, conduct an analysis of the results of the A/B test.

## Data Sources
Collaboratively with the marketing department, 9 hypotheses for increasing revenue were prepared. The hypotheses are presented in a file in CSV format - hypothesis.csv
AB testing results described in files - orders.csv and visitors.csv. All data has been cleaned.

Data Description:
File - hypothesis.csv

- Hypothesis — a brief description of the hypothesis
- Reach — user reach on a 10-point scale
- Impact — impact on users on a 10-point scale
- Confidence — confidence in the hypothesis on a 10-point scale
- Efforts — resource investment required to test the hypothesis on a 10-point scale. The higher the Efforts value, the more expensive it is to test the hypothesis.

File - orders.csv

- transactionId — order identifier
- visitorId — identifier of the user who placed the order
- date — date when the order was placed
- revenue — order revenue
- group — A/B test group to which the order belongs

File - visitors.csv

- date - date when visited
- group — A/B test group
- visitors — the number of users on the specified date in the specified A/B test group

## Libraries
Pandas, Numpy, Matplotlib, Math, Scipy

## Research Plan:
1. Prioritization of hypotheses
   - Prioritization based on the ICE system
   - Prioritization based on the RICE system
   - Analysis of the results of two types of prioritization
2. A/B test analysis
   - Building cumulative metric charts
   - Creating scatter plots, defining percentiles, and studying anomalies
   - Statistical significance testing
3. Conclusions and decision-making
