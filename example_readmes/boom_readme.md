# Project 1: SAT & ACT Analysis Overview

### Contents:
- [Problem Statement](#Problem-Statement)
- [Executive Summary](#Executive-Summary)
- [Data Dictionary](#Data-Dictionary)
- [Conclusions and Recommendations](#Conclusions-and-Recommendations)

### Problem Statement 

With the new SAT format released in March 2016, both students and state educational authorities have had to make some reconsiderations as to which test they prefer: the SAT vs. the ACT. CollegeBoard, the organization that administers the SAT, tracks state-wide participation and scores. Historically, SAT participation throughout the US has been lower than ACT participation on average. It would be helpful to them to find out what kind of strategy would help them best improve SAT participation rates going forward, particularly for states with low SAT participation rates.

### Executive Summary

This notebook begins by importing and cleaning the 2017 and 2018 participation & score data files for both the SAT and ACT. Unfortunately due to lack of completeness, we are missing section-specific scores for ACT in 2018. Once cleaned, we perform some exploratory data analysis to uncover trends in the participation rates and section scores for both the SAT and ACT in 2017-2018 on a state-wide basis across all 51 states, then identify states that saw the largest increase in participation rate over the year to carry out a deep dive on. Using external resources in conjunction with our data, we reach some conclusions.

### Data Dictionary

|Feature|Type|Dataset|Description|
|---|---|---|---|
|**state**|*object*|ACT/SAT|the US state under consideration| 
|**sat_2017_participation**|*int*|SAT|percentage of high school students (freshman through senior) in the state that took the SAT in 2017| 
|**sat_2017_reading_and_writing**|*int*|SAT|scaled score between 200-800 (inclusive) measuring verbal reasoning, averaged over all test takers in state in 2017| 
|**sat_2017_math**|*int*|SAT|scaled score between 200-800 (inclusive) measuring mathematical reasoning, averaged over all test takers in a state in 2017| 
|**sat_2017_total**|*int*|SAT|sum of verbal and reading score, averaged over all test takers in a state in 2017| 
|**act_2017_participation**|*int*|ACT|percentage of high school students (freshman through senior) in the state that took the ACT in 2017|
|**act_2017_english**|*float*|ACT|scaled score between 1-36 (inclusive) measuring command of grammar, averaged over all test takers in a state in 2017|
|**act_2017_math**|*float*|ACT|scaled score between 1-36 (inclusive) measuring mathematical reasoning, averaged over all test takers in a state in 2017|
|**act_2017_reading**|*float*|ACT|scaled score between 1-36 (inclusive) measuring reading comprehension, averaged over all test takers in a state in 2017|
|**act_2017_science**|*float*|ACT|scaled score between 1-36 (inclusive) measuring scientific reasoning, averaged over all test takers in a state in 2017|
|**act_2017_composite**|*float*|ACT|mean of English, Math, Reading, and Science scores, averaged over all test takers in state in 2017|
|**sat_2018_participation**|*int*|SAT|percentage of high school students (freshman through senior) in the state that took the SAT in 2018| 
|**sat_2018_reading_and_writing**|*int*|SAT|scaled score between 200-800 (inclusive) measuring verbal reasoning, averaged over all test takers in a state in 2018| 
|**sat_2018_math**|*int*|SAT|scaled score between 200-800 (inclusive) measuring mathematical reasoning, averaged over all test takers in a state in 2018| 
|**sat_2018_total**|*int*|SAT|sum of verbal and reading score, averaged over all test takers in a state in 2018| 
|**act_2018_participation**|*int*|ACT|percentage of high school students (freshman through senior) in the state that took the ACT in 2018|
|**act_2018_composite**|*float*|ACT|mean of English, Math, Reading, and Science scores, averaged over all test takers in a state in 2018|

### Conclusions and Recommendations

Because we only have broad state-level participation data, there is only so much we can glean from the data. Our choropleth map of SAT and ACT participation rates in both years showed us that certain regions such as the East Coast (particularly New England) are already in CollegeBoard's pocket. But the story for the rest of the states appears to be more idiosyncratic.

As a case study we looked into Illinois, which was the state that saw the largest increase in SAT participation rate from 9% in 2017 to 90% in 2018. This particular case was a result of the State of Illinois' desire for a less-time consuming test to prepare for than the PARCC exam (which previously supplanted the ACT) in addition to CollegeBoard's victory in a bid, which was surprisingly less than the ACT's, for the state to subsidize testing fees. While Rhode Island and Colorado (the next two states with the highest increase in SAT participation rates from 2017-2018 after Illinois) had similar stories, this is all based on qualitative research. It is therefore difficult to give targeted data-driven recommendations without some further work to confirm our insights.

For example, is preparation time truly a statistically significant factor that drives the participation rate for a test? We could tackle this question using regression analysis after controlling for whether or not the state subsidizes a test. With the same regression equation, we could also uncover latent factors using techniques such as Principal Component Analysis. If we wanted to be really math-savvy, we could also apply some contract theory optimization problem to figure out what is the lowest price CollegeBoard should bid that is higher than the ACT's bid that would make the sponsor see the cost differential as negligible over the life of the contract. 

This dataset aside though, we do have a couple of recommendations based on our research.
- Given the key benefits of taking the test multiple times and the shared desire between multiple states' board of education to prepare students for college, Collegeboard should consider offering the test to Sophomores instead of juniors for free. They'll be more likely to retake the exam multiple times as a Junior and then a Senior, increasing revenues for CollegeBoard.
- One state with a low participation rate that has not change year over year is Utah, which requires the ACT instead of the SAT. This is because the state emphasizes a science requirement, which the SAT does not cover. College Board could also consider offering a science section similar to the ACT.