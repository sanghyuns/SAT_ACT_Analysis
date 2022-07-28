# Hilary's Project 1 Submission

## Analyzing SAT and ACT scores by school district in California to determine greatest need

## Executive Summary

### Problem Statement

A freelance data scientist has been hired by the California Department of Education to help them determine which school districts across the state need the most funding in the upcoming 2021 fiscal budget. Using the SAT and ACT scores by school district for the state and the median income by school district for the state, the data scientist must determine which school districts have both low scores and low median income, and therefore, need more funding. They will present and defend their findings to the State Board of Education.

### Summary

Insofar as the SAT and ACT can measure a student's "scholastic aptitude", they can also measure a school's ability to adequately prepare its students - both for the test itself, and for a college education. Schools that are underfunded tend to not be able to provide the same level of preparation for their students, and schools in low-income districts tend to be underfunded. Hopefully, using the data from the SAT and ACT tests from California in 2019 combined with data from the US Census Bureau and the National Center for Education Statistics about the median incomes in different school districts in California can give an accurate picture about the level of preparation that students in low-income school districts receive - and therefore, show the California Department of Education which school districts in California have the greatest need for increased funding in the 2021 budget.

We will look specifically at the number of students in a given school district who are able to meet certain benchmarks defined by the College Board - for the ACT, that means getting a score of at least 21 on the test as a whole, and for the SAT, that means at least a 480 in Evidence-Based Reading and Writing and a 530 in Math for students in Grade 12, and a 460 and 510 in those respective categories for a student in Grade 11.

### Data Dictionary

|Feature|Type|Dataset|Description|
|---|---|---|---|
|district_name|object|using_sat|These are the names of the districts that have reported data for the 2019 SAT|
|total_number_grd_12|float|using_sat|This is the number of students from each district who met the benchmark for the SAT from grade 12|
|total_number_grd_11|float|using_sat|This is the number of students from each district who met the benchmark for the SAT from grade 11|
|district_name|object|using_act|These are the names of the districts that have reported data for the 2019 ACT|
|num_students_greaterequal_21|float|using_act|This is the number of students reported by each district who received a score of at least 21 on their ACT test in 2019|
|district_name|object|using_inc|These are the names of the districts that were collected by the US Census Bureau and The National Center for Education Statistics|
|median_income_by_district|float|using_inc|This is the median income for each school district in California as reported by the US Census Bureau and The National Center for Education Statistics|

### Main Points, Findings, and Results

As expected, it quickly became clear that the 20 highest-income districts in California were producing many more students who were able to meet the benchmarks than the 20 lowest-income districts.

This graph shows the marked difference between the number students from high income school districts who were able to meet the benchmarks, and the number of students from low income school districts who were able: 
![alt text][plot]

[plot]: tested_students.png "Students Tested"

Additionally, plotting the median income for each district against the districts that had reported students  from Grade 12 meeting the College Board's SAT benchmarks showed a positive correlation between increasing income and increasing scores:
![alt text][plot]

[plot]: income_sat_12.png "Scores vs. Income for Grade 12"

Finally, the same plot was made for students from Grade 11 who had met the benchmark for the SAT, which also showed a strong positive correlation:
![alt text][plot]

[plot]: income_sat_11.png "Scores vs. Income for Grade 11"

### Observations and Conclusions

It's clear from the findings that the school districts with greatest need of increased funding are those with lowest income. If SAT and ACT tests can measure a student's readiness for college, they can also measure a school's abilitiy to prepare its students, so districts without adequate funding will not contain schools that are meeting the needs of their students. The California Department of Education should direct increased funding to the lowest-income districts in the state, particularly those in the 20 lowest median income bracket.

### Next Steps

An important next step with this project would be to determine which other school districts among the twenty lowest-income districts contained schools that were preparing students for college and designating those as funding recipients as well. The SAT and ACT data from the DOE had some holes that might have left some districts out to dry, and just because a district does not report students passing a certain benchmark, does not mean that district is not deserving of increased funding to support its students.

### Bibliography

Author: California Department of Education
Title: Record Layout for SAT Test Results
Date of Publication: 2019
Electronic Location or Identifier: https://www.cde.ca.gov/ds/sp/ai/reclayoutsat19.asp

Author: California Department of Education
Title: Record Layout for ACT Test Results
Date of Publication: 2019
Electronic Location or Identifier: https://www.cde.ca.gov/ds/sp/ai/reclayoutact19.asp

Author: Adam McCann
Title: Most & Least Equitable School Districts in California
Date of Publication: 2020
Publisher and/or Distributor: WalletHub
Electronic Location or Identifier:https://wallethub.com/edu/e/most-least-equitable-school-districts-in-california/77056/

Author: College Board
Title: Benchmarks
Date of Publication: Unknown
Electronic Location or Identifier: https://collegereadiness.collegeboard.org/about/scores/benchmarks
