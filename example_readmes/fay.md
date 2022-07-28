# <span style="font-variant:small-caps;">Access as a Metric of Enrollment:</span>
#### <span style="font-variant:small-caps;">ACT/SAT Participation and Going-To-College Rates</span>
---
### <span style="font-variant:small-caps;">Problem Statement</span> 
*The State of California Department of Education (CDOE) would like to improve the rate at which its high school graduates enroll in a postsecondary, degree-granting institution within one year of graduation. The CDOE would like a report on whether the implementation of mandatory, in-school administration of either the ACT or SAT might have an effect on these going-to-college rates.*

### <span style="font-variant:small-caps;">Data Dictionary</span>

|DataFrame|Description|
|---|---|
|**ntwd_set**|2017-19 ACT and SAT US participation rates by state|
|**cali**|Dataset for California covering going-to-college rates, ACT and SAT participation rates, and median income by county, 2017-18|
|**cnty**|2014-18 Connecticut going-to-college rates and median incomes by county|
|**city**|2014-18 Connecticut going-to-college rates and median incomes by city|

|Feature|Type|Description|
|---|---|---|
|**a_part17**|*float64*|2017 ACT participation rate|
|**a_part18**|*float64*|2018 ACT participation rate|
|**s_part17**|*float64*|2017 SAT participation rate|
|**s_part18**|*float64*|2018 SAT participation rate|
|**pct_grad18**|*float64*|2018 graduation rate|
|**gc_rate17**|*float64*|2017 going-to-college rate|
|**grads17**|*blah*|Number of 2017 high school graduates|
|**in_comm17**|*blah*|Number of 2017 high school graduates who went to in-state community college within a year|
|**out_two17**|*blah*|Number of 2017 high school graduates who went to an out-of-state two-year institution within a year|
|**gc_rate18**|*blah*|2018 going-to-college rate|
|**grads18**|*blah*|Number of 2018 high school graduates|
|**in_comm18**|*blah*|Number of 2018 high school graduates who went to in-state community college within a year|
|**out_two18**|*blah*|Number of 2018 high school graduates who went to an out-of-state two-year institution within a year|
|**enrolled19**|*float64*|Number of students enrolled in 2019 at time of testing|
|**a_tested19**|*float64*|Number of students who took the ACT in 2019|
|**a_participation**|*float64*|2019 ACT participation rate|
|**s_tested19**|*float64*|Number of students who took the SAT in 2019|
|**s_participation19**|*float64*|2019 SAT participation rate|
|**med_inc18**|*int64*|Median income over the period of 2014-18|
|**gc_rate**|*float64*|College-Going Rates of High School Graduates - Directly from High School (2016)|
|**ent14**|*float64*|Percent of students who entered a post-secondary institution within a year of graduating in 2014|
|**ent15**|*float64*|Percent of students who entered a post-secondary institution within a year of graduating in 2015|
|**ent16**|*float64*|Percent of students who entered a post-secondary institution within a year of graduating in 2016|
|**ent17**|*float64*|Percent of students who entered a post-secondary institution within a year of graduating in 2017|
|**ent18**|*float64*|Percent of students who entered a post-secondary institution within a year of graduating in 2018|
|**med_inc**|*float64*|Median income over the period of 2011-15|

![Nationwide Participation vs GCR](./presentation/ntwd_fig.png)

### <span style="font-variant:small-caps;">An Analysis Brief, or a Brief Analysis</span>
We begin this analysis by looking at standardized testing participation rates and GCRs nationwide in order to examine the relationship between the two, which only becomes apparent when we categorize states by whether or not they have a mandate for in-school testing. With this categorization, we find that those that do have a mandate in place do, overall, have higher GCRs.
</br>
After this macro-level analysis, we look at the data from California which we are immediately concerned with given the purpose of this report. We examine how participation rates map against GCRs by county in the school years ending in 2017 and 2018, and observe trends therein related to median income as well.
</br>
Finally, we look at data gathered from Connecticut—-one of the twelve states that mandate in-school testing that reports data to a similar extent as California—-in order to observe if income still retains any effect on GCR, and to provide a pole against which to compare California.

### <span style="font-variant:small-caps;">Conclusions and Recommendations</span>

Upon performing this analysis, we are able to come to certain conclusions:

1. Participation in standardized testing has a positive correlation to going-to-college rates (GCR)
    - This is seen at the national level, where all states that mandate in-school testing as part of their school day have higher GCRs on average
    - There is also a strongly positive correlation at the California state level: districts with higher participation rates had higher GCRs
2. California county median incomes strongly correlate to the above trend as well, with higher income counties having both higher GCRs and standardized testing participation rates
    - By comparing this case with that of Connecticut, which dedicates a school day for mandatory, free testing, we can see that except in extreme cases (Fairfield county) the effect of income on GCR is drastically reduced
    - This shows that providing a requirement for free, in-school standardized testing has a direct correlation to GCRs
3. There is a strongly negative correlation between California community college enrollment and standardized test participation rates

And from these conclusions, we can make certain recommendations:

1. The California State Deparment of Education should mandate free, in-school testing in all of its public schools
2. While this stipulation should be made, this does not indicate that California should use the ACT or SAT as a metric of aptitude or student success in its own education policy; this is strictly a recommendation for the improvement of its GCRs statewide
3. The CDOE should at the same time provide free access to preparatory materials and preparatory classes, possibly as optional in-school periods, to work toward mitigating the effects that income has on participation rates, testing success, and GCR
4. The CDOE should expand this report to examine the following characteristics as well:
    - Race : In order to identify systemic issues in the state apparatus that contribute to gaps in student success and GCR
    - Parental education levels : To examine how schools might disseminate information to parents in order to bolster participation rates and GCR
    - Teacher/pupil ratios : In order to define a new parameter of 'engaged access,' upon which we can determine how student engagement correlates to testing participation and GCR
    - Collecting data on not only degree-granting post-secondary institutions, but also technical schools, in order to determine realistic GCR goals
5. To comprehensively study these issues and efficiently implement effective solutions, the CDOE should perform this analysis on all states where data is available
6. The CDOE should include records of college persistence as they relate to enrollment across all of the above defined metrics to assist in the shaping of education policy