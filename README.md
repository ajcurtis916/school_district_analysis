
# School District Analysis

## *A high-level snapshot of the district's key metrics*

### Project Overview: Analyze the school district data and relay findings on school performance based on the overall passing rate, budget per student, school size and type of school, and average math and reading scores received by students at each grade level at each school.
---
</br>
After our first fullscale analysis, the school board found evidence of academic dishonesty, specifically among reading and math grades for Thomas High School ninth graders.  Due to this finding, we were tasked with replacing the uncredible scores with NaNs in order to uphold state-testing standards, while keeping the rest of the data intact.  The first portion of our second round analysis was to remedy this situation, then to repeat the previous school district analysis and write the following report to explain how these changes may have affected the overall analysis.
</br>
</br>

## Results

Original District Summary     |  Credible Scores District Summary
:-------------------------:|:-------------------------:
<img src="https://github.com/ajcurtis916/school_district_analysis/blob/main/resources/zOG_dsum_top8.png" width="500" />|<img src="https://github.com/ajcurtis916/school_district_analysis/blob/main/resources/zcredible_scores_dsum_top8.png" width="500"/>
</br>

There were very insignificant changes between the original findings and the findings once the ninth graders scores at Thomas high has been removed for academic integrity.  The summaries above show the top eight (8) performing schools based on overall passing percentage (%).  The bottom seven (7) performing schools can be found in the resources file.  Both pictures together create a comprehensive district summary, 15 schools in total:
</br>

- Thomas High's positioning as second (2nd) highest in performance overall did not fluctuate.
- The remaining 14 high schools in the district summary were not affected by the second round analysis.  
- After rounding, Thomas High's average math scores were 83.4 after both analyses.
  - If the scores were not rounded, math scores decreased minimally during the second analysis.
- After rounding, Thomas High's average reading score increased from 83.8 to 83.9.
- After rounding, Thomas High's percentage passing math was 93% after both analyses. 
  - If the scores were not rounded, percentage passing math decreased minimally during the second analysis.
- After rounding, Thomas High's percentage passing reading was 97% after both analyses.
  - If the scores were not rounded, percentage passing reading decreased minimally during the second analysis.
- After rounding, percentage passing overall was 91% after both analyses.
  - If the scores were not rounded, percentage of students passing both tests decreased minimally during the second analysis.
</br>
</br>

Scores by Spending     |  Scores by Size    |    Scores by School Type 
:-------------------------:|:-------------------------:|:-------------------------:
<img src="https://github.com/ajcurtis916/school_district_analysis/blob/main/resources/zscores_by_spending.png" width="400" />|<img src="https://github.com/ajcurtis916/school_district_analysis/blob/main/resources/zscores_by_size.png" width="400"/>|<img src="https://github.com/ajcurtis916/school_district_analysis/blob/main/resources/zscores_by_type.png" width="400"/>
</br>

There were no changes to the scores by school spending, size, and school type after removing the ninth graders' scores at Thomas High.  We accounted for a change in school population when running the calculations for the new scores and passing percentages above, but left the "Total Students" population unaltered, so as not to incorrectly reprt the actual number of students in the Thomas High population or per student budget.
</br>
Most obviously, the ninth grade scores columns changed to all NaNs for Thomas High School.  Our analyses of the district scores by grade, spending, school size and school type were as follows: 
</br>

- Overall passing percentages by grade level were within a 1% margin at each school.
- The highest performing schools fell into the lowest budget per student category.   
  - There was a 90% overall passing rate at schools with a $585 or less per student budget.
  - The overall passing percentage was 81% at schools with a $586-629 per student budget.
  - The overall passing percentage was 63% at schools with a $630-644 per student budget.
  - The overall passing percentage was 54% at schools with a $645 or more per student budget.
- The performance of schools sized "small" (less than 1,000 students) and "medium" (1,000 to 2,000 students) performed best. 
  - Small and medium sized schools were within 1% of each other at 90% and 91% respectively.
  - The performance from large sized schools (2,000 to 5,000 students) was significantly lower at 58% of students passing overall.
- Charter schools outperformed the general district schools by a large margin.
  - The overall passing percentage was 90% at schools classified as "Charter".
  - The overall passing percentage was 54% at schools classified as "District". 
</br>

## Resources
* Data Sources: schools_complete.csv, students_complete.csv (located in "resource" file)
* Software: Jupyter Notebook 5.0

## Summary
Minimal changes were observed within the overall district metrics after replacing the reading and math scores for the ninth grade students at Thomas High School.  The largest observed change was the increase in Thomas High's average reading scores by .1%.  Additional changes were observed when comparing the average math scores, passing reading, passing math and overall passing percentages to the hundredths place or higher.
</br>
</br>
Type of school was found to have the greatest weight on increased test performance.  Based on overall passing percentages, students at Charter schools performed 36% better than students at District schools.  School size followed closely behind in regards to impact on performance.  Students at schools with 2,000 students or more had 32% less overall passing percentages than their smaller student body counterparts. Oddly, budget per student and school performance were negatively correlated.  The higher the budget per captia, the lower the overall passing percentages became.
</br>
</br>
Based on our findings, Charter schools and schools with student populations less than 2,000 are correlated to higher performance.  It may be worth taking a closer look at the reasons behind the counterintuitive negative correlation between high student budget and student test performance.
