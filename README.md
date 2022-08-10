# Project 1: SAT & ACT Analysis


### Contents:
 - [Problem Statment](#Problem-Statement)
 - [Executive Summary](#Executive-Summary)
 - [Data Dictionary](#Data-Dictionary)
 - [Conclusions and Recommendations](#Conclusions-and-Recommendations)

### Problem Statement

Many states have seen drastic changes in participation rates for both the ACT and the SAT between 2017 and 2018, with the trend going over to the SAT. The SAT, in general, has been much lower in participation in the past. It would be interesting to see if the states that changed over to the SAT have seen any benefits in the short span of 1 year.

### Executive Summary

We will take a look at the scores of SAT and ACT tests throughout the US in 2017 and 2018. After finding that the ACT 2018 dataset only included the participation rate and the composite score, additional research was conducted online and a reliable source showed the rest of the scores in the same way of the 2017 score. Now as we are able to clean up the data comparatively between the years, all the data was cleaned, the columns renamed, and the datasets merged into one single final dataframe.

### Data Dictionary

|Feature|Type|Dataset|Description|
|---|---|---|---|
|state|string|final_df|State from which ACT/SAT was taken|
|act_2017_part|float64|act_2017|Participation rate divided by 100| 
|act_2017_english|float64|act_2017|Average english score|
|act_2017_math|float64|act_2017|Average math score|
|act_2017_reading|float64|act_2017|Average reading score|
|act_2017_science|float64|act_2017|Average science score|
|act_2017_composite|float64|act_2017|Average composite score|
|sat_2017_part|float64|sat_2017|Participation rate divided by 100|
|sat_2017_ebrw|int64|sat_2017|Average reading&writing score|
|sat_2017_math|int64|sat_2017|Average math score|
|sat_2017_total|int64|sat_2017|Average total score|
|act_2018_part|float64|act_2018|Participation rate divided by 100|
|act_2018_english|float64|act_2018|Average english score|
|act_2018_math|float64|act_2018|Average math schore|
|act_2018_reading|float64|act_2018|Average reading score|
|act_2018_science|float64|act_2018|Average science score|
|act_2018_composite|float64|act_2018|Average composite score|
|sat_2018_part|float64|sat_2018|Participation rate divided by 100|
|sat_2018_ebrw|int64|sat_2018|Average reading&writing score|
|sat_2018_math|int64|sat_2018|Average math score|
|sat_2018_total|int64|sat_2018|Average total score|

## Conclusions and Recommendations

From the data provided, we can conclude that there was an increase of average SAT particiation between the two years, resulting in an overall lower average score, as proven by the heatmap above. This decrease in performance may be due to the sudden change in test format and the lack of resources from the states that have made this drastic change. In order to solidify the findings of the analysis, it is recommended to observe the states that made the change for a couple more years before making any further changes. If the scores, relative to the ACT, increase in those states, it would be safe to conclude that the change was beneficial, and more states should make the change.
It is crucial to note that there is a continued push against standardized testing and its effectiveness. If each state wants to continue its tradition of standardized testing, it is important to to conduct additional research to support its effectiveness and present it in a way that ties in the SAT/ACT with its success. If they wish to pursue a different path, they should consider other forms of tests that cater to each students' unique characteristics such as assessing a portfolio that was organized throughout the students academic career.

## Additional Research

Additional research was conducted in order to double check the accuracy of the data given and to append existing data.

Comprehensive 2017/2018 SAT scores: https://nces.ed.gov/programs/digest/d19/tables/dt19_226.40.asp
Comprehensive 2018 ACT scores: https://nces.ed.gov/programs/digest/d18/tables/dt18_226.60.asp

According to these sources, which was published by the National Center for Education Statistics(NCES) there were some differences in their data when compared to the data provided.
