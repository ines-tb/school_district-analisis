# School District Analysis
Analysis of Schools in a District with Pandas

## Challenge

#### Overview
Among the 15 schools in the District, _Thomas High School_ has reported discrepancies in their _9th graders_ data. For this reason, it has been requested the results to be re-analyzed after setting the math and reading scores of those particular students to NaN and leaving the rest of the information intact.
The new report should include answers to the following:
* How the district and school summaries have been affected.
* How Thomas High School's performance have been affected relative to the other schools.
* How the "Math and Reading Scores by Grade", "Scores by School Spending", "Scores by School Size" and "Scores by School Type" results have been affected after the data change.


#### Resources
* Data Sources: _schools_complete.csv_ and _students_complete.csv_.
* Software: Python 3.7.6, Visual Studio Code 1.45.1, Anaconda 4.8.3, Jupyter Notebook 6.0.3.
  

#### Summary

###### District results
The district figures are barely impacted by the adjusted data. Only a -0.1 difference in Math Score which makes -1% in Math passing percentage and Overall percentage. So the **impact over the district is not appreciable**.

  * District Summary:
  ![DistrictSummary](./media/1.districtSummary.png?raw=true)
  * District Summary without 9th graders Thomas H.S. data:
  ![DistrictSummaryChallenge](./media/2.districtSummaryChallenge.png?raw=true)

###### School results

Checking the results for Thomas High School we can see that the average score for both Math and Reading very slightly differ respectively from the same summary including 9th graders. This means that the 9th graders had same average than the rest of the school. However, the **passing percentage drop** over 26% for Math, over 27% for reading and over 25% overall passing, which indicates that the passing percentages for the invalid data were extremely high and therefore raised the metrics around 25% and those results are not kept by the following grades.
  * School Summary:
  ![SchoolSummary](./media/3.schoolSummary.png?raw=true)
  * School Summary without 9th graders Thomas H.S. data:
  ![SchoolSummaryChallenge](./media/4.schoolSummaryChallenge.png?raw=true)

###### Top Performing Schools

Performance wise, the new data extremely affects the ranking negatively, leaving Thomas High School out of the top five based on overall passing percentage. More precisely, **descending from the second place to the eighth** due to the over 25% fall suffer after the data adjustment.
  * Performance Summary:
  ![TopSchools](./media/5.TopSchools.png?raw=true)
  * Performance Summary without 9th graders Thomas H.S. data:
  ![TopSchoolsChallenge](./media/6.TopSchoolsChallenge.png?raw=true)

###### Spending Budget, Size and Type of School

When comparing the data based on the budget per student, school size of type of school, any of the average scores for Math or reading are affected. However, in all cases the **passing percentages drop** significantly in all cases 
* Based on **budget per student**: Decrease of a 6% in math, 7% in reading and overall.
  - Spending Summary:
    ![SpendingSummary](./media/7.SpendingSummary.png?raw=true)
  - Spending Summary without 9th graders Thomas H.S. data:
    ![SpendingSummaryChallenge](./media/8.SpendingSummaryChallenge.png?raw=true)

* Based on **school size**: Decrease of a 6% in math, reading and overall.
  - Size Summary:
    ![SizeSummary](./media/9.sizeSummary.png?raw=true)
  - Size Summary without 9th graders Thomas H.S. data:
    ![SizeSummaryChallenge](./media/10.sizeSummaryChallenge.png?raw=true)

* Based on **school type**: Decrease of a 4% in math and reading and a 3% overall.
  - Type Summary:
    ![TypeSummary](./media/11.typeSummary.png?raw=true)
  - Type Summary without 9th graders Thomas H.S. data:
    ![TypeSummaryChallenge](./media/12.typeSummaryChallenge.png?raw=true)


**NOTE** : When analyzing the data based on the score by grade, there is no information to provide as for Thomas High School 9th graders, the data for both Math and Reading is NaN.
* Score by Grade Summary without 9th graders Thomas H.S. data:
![ScoreByGradeChallenge](./media/13.ScoreByGradeChallenge.png?raw=true)
