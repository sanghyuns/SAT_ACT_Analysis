# College Entrance Exam Participation: Analysis of 2017 SAT and ACT Datasets

## Background

SAT and ACT exams remain the standard for college applications, however, most colleges don't require one over the other.  Both exams have similar registration costs and seek to test student aptitude. The ACT is composed of four subjects: math, science, english, and reading, while the SAT is composed of two: math and evidence-based reading and writing [1, 2]. The two tests have different scoring scales, which are summarized below (Figure 1).

<img src="./images/sat.png" width="50%" height="50%">

It is also important to note that the SAT test format was changed in March, 2016, making it more similar to the ACT [3].

## Dataset

I was provided with a dataset from each test organization, with state mean scores and participation rates [4, 5]. I merged, cleaned, and corrected errors in the datasets. I also calculated normalized total scores from each test and added them to my dataframe for future comparison. 

## Discussion 

SAT participation lagged behind the ACT in 2017. From Figure 3, it can be seen that the midwest region has the lowest SAT participation. North Dakota, Mississippi, and Iowa had the lowest rates at 2% each. If the College Board were to focus their promotional SAT campaigns, they would be wise to target the midwest.

<img src="./images/map.png" width="50%" height="50%">

A hypothesis test confirmed that the ACT has a higher mean participation rate than the SAT. Confidence intervals were constructed for 95% confidence of the national participation rate for each test: SAT (30%, 49%) and ACT (56%, 74%). From Figure 4, it becomes obvious that students are favoring one test over the other, which is why we see clusters at either end of this negative correlation.

<img src="./images/participation.png" width="50%" height="50%">

High achieving students are disproportionately represented in low participation state mean exam scores. As shown in Figure 5, there are obvious clusters of scores at high participation - low score and high score - low participation.

<img src="./images/rate.png" width="50%" height="50%">

The comparison shows that with a 100% participation rate, the total scores are the lowest. This is because we are capturing the total distribution (i.e. the whole eligible population). The lower participation rates might have higher mean scores since motivated students, students who are going to do well on the test, are being disproportionately represented. It is for this reason that we can't confirm which test is more difficult with the given data. Since we don't have individual student scores, only state mean scores, we don't know if the same students are taking both exams.

Total scores are strongly correlated to subject scores, with higher scores in non-technical subjects. As shown in the Figures 6 and 7 below, there is a strong positive linear correlation for both exams where a high total score is associated with high subject scores. This makes sense since the subject scores contribute to the total score. When we graph all the subjects on the same plot, we see that states typically have higher mean reading scores than the other subjects on the SAT and higher reading score for the ACT.

<img src="./images/sat_sub.png" width="50%" height="50%">
<img src="./images/act_sub.png" width="50%" height="50%">

To summarize, given the limited data we can conclude that the ACT had a higher mean participation rate (65%) than then SAT (45%) in 2017. Midwestern states had the lowest SAT participation, making them targets for promotional campaigns. High achieving students are disproportionately represented in states with low participation. Subject scores are strongly correlated to total scores. 

## Next Steps

Additional data is needed in order to make recommendations to improve SAT participation. Individual student test scores, as opposed to state mean scores, would help answers questions regarding the difficulty of one exam over the other. Contextual information per state or county, such as per capita income, would give insight to  potential factors influencing decisions to take one test over the other. Prior years results would allow for the identification and comparison of trends, such as the effect of changing the test format and its impact on participation. Lastly, it would be helpful to understand how the College Board and American College Test are defining eligible participants, in order to confirm that both tests are capturing the same populations.

## References: 

[1] https://collegereadiness.collegeboard.org/sat

[2] https://www.princetonreview.com/college/sat-act

[3] http://college.usatoday.com/2016/01/04/sat-changes-2016/

[4] https://reports.collegeboard.org/pdf/2017-maryland-sat-suite-assessments-annual-report.pdf

[5] https://www.act.org/content/dam/act/unsecured/documents/cccr2017/ACT_2017-Average_Scores_by_State.pdf
