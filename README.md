# Module_04_Challenge
Module 04 Challenge - PyCity Schools Analysis

## Overview of Project
Module 4 Challenge. This project involves using Jupyter Notebooks, pandas, and NumPy to import, clean, manipulate, and analyze data related to student performance at 15 high school campuses within a School District.

### Purpose
The purpose of this challenge is to take CSV files containing student-level and campus-level data, clean the data as necessary, and then use pandas and NumPy to calculate relevant statistics related to student performance in several key areas, and to then aggregate that data on a grade-level basis, a campus-wide basis, and a district-wide basis, while also attempting to show the impact that per-student funding levels, school size, and a school's status as a Charter school or a traditional District-operated school have on student performance.

As a result of potential irregularities in the data associated with 9th Grade students at Thomas High School, two different sets of analysis were performed - one utilizing the potentially irregular data as it was received, and a second analysis which excluded the test scores associated with 9th Grade students at Thomas High School

## Results
The results of our Analysis of the data is as follows:

### Impact of THS Data on Overall District Summary:

  - As demonstrated by the following images of the District Summary, the exclusion of data for 9th Grade Students at Thomas High School had a negligible effect on the Overall District Summary.  The exclusion of data related to THS 9th Grade Students resulted in overall Average Math Scores for the district declining by 0.1%, but had no impact on the Average Reading Score; the percentage of District students Passing Math declined by 0.2%, and the percentage of District Students Passing Reading declined by 0.1%.  Excluding THS 9th Grade Students from the analysis resulted in a decline in the Overall Passing Percentage of 0.3%.

    - Original Data Set, Containing Performance Data for THS 9th Grade Students:
    
    ![District Summary Including THS 9th Graders](/Images/District_Summary_Inc_THS_9th_Grade_Scores.png)
    
    - Revised Data Set, Excluding Performance Data for THS 9th Grade Students: 

    ![District Summary Excluding THS 9th Graders](/Images/District_Summary_Ex_THS_9th_Grade_Scores.png)

### Impact on the Exclusion of 9th Grade Student Data on Overall Results of Thomas High School:

  - Likewise, as demonstrated by the following images of the summary data for Thomas High School, the exclusion of data for 9th Grade Students had a negligible effect on the Overall Performance of the Campus.  The exclusion of data related to 9th Grade Students had no impact on Average Math Scores for the Campus, and resulted in an increase of 0.1% in the Average Reading Score; the percentage of Thomas High School students Passing Math, Passing Reading, and the Overall Passing rate were not impacted by the exclusion of the 9th Grade data. 

    - Thomas High School Summary, Containing Performance Data for 9th Grade Students:
    
    ![School Summary Including THS 9th Graders](/Images/THS_Summary_Including_9th_Grade_Scores.png)
    
    - Thomas High School Summary, Excluding Performance Data for 9th Grade Students: 

    ![School Summary Excluding THS 9th Graders](/Images/THS_Summary_Excluding_9th_Grade_Scores.png)

### Performance of Thomas High School Relative to Other Schools:

  - With respect to the Performance of Thomas High School relative to other schools within the district, the exclusion of data for 9th Grade Students did not have a material effect on the stack rankings of schools, as based on Overall Passing Percentage; however, in the categories of Average Math Score, and the Percentage of Students Passing Reading, the performance of Griffin High School now exceeds that of Thomas High School, and the difference in Overall Passing Percentage narrowed significantly, from nearly 0.5% to only 0.05%. . 

    - Stack Rankings, According to Overall Passing Percentage, Containing Performance Data for THS 9th Grade Students:
    
    ![Stack Rankings Including THS 9th Graders](/Images/School_Stack_Rankings_Inc_THS_9th_Grade_Scores.png)
    
    - Stack Rankings, According to Overall Passing Percentage, Containing Performance Data for THS 9th Grade Students: 

    ![Stack Rankings Excluding THS 9th Graders](/Images/School_Stack_Rankings_Ex_THS_9th_Grade_Scores.png)      

### Impact on Other Categorizations:

The exclusion of performance data for 9th Grade Students at Thomas High School did not have a material impact on any of the other categories by which data was analyzed, including: 

  - Math Scores by Grade:
       - Including Thomas High School 9th Graders:
       
      ![Math Scores by Grade Including THS 9th Graders](/Images/Math_Scores_Inc_THS_9th_Grade_Scores.png)
    
       - Excluding Thomas High School 9th Graders:
       
      ![Math Scores by Grade Excluding THS 9th Graders](/Images/Math_Scores_Ex_THS_9th_Grade_Scores.png)
      
  - Reading Scores by Grade:
       - Including Thomas High School 9th Graders:
       
      ![Reading Scores by Grade Including THS 9th Graders](/Images/Reading_Scores_Inc_THS_9th_Grade_Scores.png)
    
       - Excluding Thomas High School 9th Graders:
       
      ![Reading Scores by Grade Including THS 9th Graders](/Images/Reading_Scores_Ex_THS_9th_Grade_Scores.png)
  
  - Scores by Per Student Spending Levels (Thomas High School is Within the ($630 - $644) Bin):
       - Including Thomas High School 9th Graders:
       
      ![Scores by Funding Level Including THS 9th Graders](/Images/Scores_Spending_Inc_THS_9th_Grade_Scores.png)
    
       - Excluding Thomas High School 9th Graders:
       
      ![Scores by Funding Level Excluding THS 9th Graders](/Images/Scores_Spending_Ex_THS_9th_Grade_Scores.png)
      
  - Scores by School Type (Thomas High School being a Charter School):
       - Including Thomas High School 9th Graders:
       
      ![Scores by School Type Including THS 9th Graders](/Images/Scores_School_Type_Inc_THS_9th_Grade_Scores.png)
    
       - Excluding Thomas High School 9th Graders:
       
      ![Scores by School Type Excluding THS 9th Graders](/Images/Scores_School_Type_Ex_THS_9th_Grade_Scores.png)
      
   - Scores by School Size (Thomas High School being Classified as "Medium"):
       - Including Thomas High School 9th Graders:
       
      ![Scores by School Size Including THS 9th Graders](/Images/Scores_School_Size_Inc_THS_9th_Grade_Scores.png)
    
       - Excluding Thomas High School 9th Graders:
       
      ![Scores by School Size Excluding THS 9th Graders](/Images/Scores_School_Size_Ex_THS_9th_Grade_Scores.png)
    
## Summary

The exclusion of Performance Data for 9th Grade Students at Thomas High School had a negligible impact on the performance of the District overall, and did not have a material impact of the performance of Thomas High School as a whole or in relation to the other schools within the district.  The exclusion of data related to THS 9th Grade Students resulted in overall Average Math Scores for the district declining by 0.1%, but had no impact on the Average Reading Score; the percentage of District students Passing Math declined by 0.2%, and the percentage of District Students Passing Reading declined by 0.1%.  Excluding THS 9th Grade Students from the analysis resulted in a decline in the Overall Passing Percentage of 0.3%.
