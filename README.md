
# School District Analysis

## *A high-level snapshot of the district's key metrics*

### Project Overview: Analyze the school district data and relay findings on school performance based on the overall passing rate, budget per student, school size and type of school, and average math and reading scores received by students at each grade level at each school.
---
</br>
After our first fullscale analysis, the school board found evidence of academic dishonesty, specifically among reading and math grades for Thomas High School ninth graders.  Due to this finding, we were tasked with replacing the uncredible scores with NaNs in order to uphold state-testing standards, while keeping the rest of the data intact.  The first portion of our second round analysis was to remedy this situation, then to repeat the previous school district analysis and write the following report to explain how changes affected the overall analysis.
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
- After rounding, Thomas High's average reading score increased from 83.8 v. 83.9.
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

There were no changes between the original findings and the findings once the ninth graders scores at Thomas high has been removed for academic integrity for the scores by school spending, size and school type analyses.  Though we accounted for a change in school population when running the calculations for the new scores and percentages passing above, we left the "Total Students" population unaltered, so as not to report incorrectly the actual number of students in the Thomas High population or per student budget.
</br>
Most obviously, the ninth grade column changed to all NaNs for Thomas High School in the scores by grade analysis.  Our analyses of the district scores by spending, school size and school type were as follows: 
</br>

- Oddly, the highest performing schools fell into the lowest budget per student category.
  - There was a 90% overall passing rate at schools with a $585 or less per student budget
  - The overall passing percentage was 81%
- How does replacing the ninth-grade scores affect the following:
- Math and reading scores by grade
- Scores by school spending
- Scores by school size
- Scores by school type
</br>

## Resources
* Data Source: schools_complete.csv, students_complete.csv (located in "resource" file)<br/>
* Software: Python 3.7.6 64-bit, Visual Studio Code, Version: 1.61.0

## Summary
Summarize four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.
