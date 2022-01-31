# Module_04_Challenge
Module 04 Challenge - PyCity Schools Analysis

## Overview of Project
Module 4 Challenge. This project involves using Jupyter Notebooks, pandas, and NumPy to import, clean, manipulate, and analyze data related to student perfomance at 15 high school campuses within a School District.

### Purpose
The purpose of this challenge is to take CSV files containing student-level and campus-level data, clean the data as necessary, and then use pandas and NumPy to calculate relevant statistics related to student performance in several key areas, and to then aggregate that data on a grade-level basis, a campus-wide basis, and a district-wide basis, while also attempting to show the impact that per-student funding levels, school size, and a school's status as a Charter school or a traditional District-operated school have on student performance.

As a result of potential irregulatrities in the data associated with 9th Grade students at Thomas High School, two different sets of analysis were performed - one utilizing the potentially irregular data as it was received, and a second analysis which excluded the test scores associated with 9th Grade students at Thomas High School

## Results
The results of our Analysis of the data is as follows:

### Impact of THS Data on Overall District Summary:

  - As demonstrated by the following images of the District Summary, the exclusion of data for 9th Grade Students at Thomas High School had a negligible effect on the Overall District Summary.  The exclusion of data related to THS 9th Grade Students resulted in overal Average Math Scores for the distrcit declining by 0.1%, but had no impact on the Average Reading Score; the percentage of District students Passing Math declined by %0.2, and the percentage of District Students Passing Reading declined by 0.1%.  Excluding THS 9th Grade Students from the analysis resulted in a decline in the Overall Passing rate by 0.3%.

    - Original Data Set, Containing Perfomance Data for THS 9th Grade Students:
    
    ![District Summary Including THS 9th Graders](/Images/District_Summary_Inc_THS_9th_Grade_Scores.png)
    
    - Revised Data Set, Excluding Performance Data for THS 9th Grade Students: 

    ![District Summary Excluding THS 9th Graders](/Images/District_Summary_Ex_THS_9th_Grade_Scores.png)

### Impact on the Exclusion of 9th Grade Student Data on Overall Results of Thomas High School:

  - Likewise, as demonstrated by the following images of the summary data for Thomas High School, the exclusion of data for 9th Grade Students had a negligible effect on the Overall Performance of the Campus.  The exclusion of data related to 9th Grade Students had no impact on Average Math Scores for the Campus, and resulted in an increase of 0.1% in the Average Reading Score; the percentage of Thomas High School students Passing Math, Passing Reading, and the Overall Passing rate were not impacted by the exclusion of the 9th Grade data 

    - Thomas High School Summary, Containing Perfomance Data for 9th Grade Students:
    
    ![School Summary Including THS 9th Graders](/Images/THS_Summary_Including_9th_Grade_Scores.png)
    
    - Thomas High School Summary, Excluding Perfomance Data for 9th Grade Students: 

    ![School Summary Excluding THS 9th Graders](/Images/THS_Summary_Excluding_9th_Grade_Scores.png)

## Election Audit Summary

There are multiple ways in which the Python script utilized for this project could be utilized for other elections - either with or without additional modification.

1. There is nothing specific to this script that would limit its use to this particular race or this specific Congressional District - the lists of Counties and Candidates are based on values contained within the election_results.csv file that is provided, allowing for this same script to be utilized in other races without requiring any modification of the script.


2. With minimal modification, this script could be utilized in instances where there are multiple races associated with a single ballot - for example, a ballot could contain votes in races for President, Senate, and House of Representatives.  One approach to facilitating this functionality would be to include an additional column in the election_results.csv file that denotes the specific Race that a choice is associated with - for example, adding "Race" to the existing fields of "Ballot ID", "County" and "Candidate", resulting in a single "Ballot ID" being associated with multiple records - one for each Race in which a selection was made.  The script could then be modified to create a Dictionary containing a list of each of the races being contested, much as is currently done to create a Dictionary containing each of the Candidate Names and County Names.  Using a "For/Each" approach for each of the "Races" contained in the new "Races" dictionary, with the existing code nested within it and with only minor modifications, it would then be possible to tabulate votes for multiple races through the use of a single election_results.csv file and single Python script, yielding output for each race being contested.      

## Limitations

There were no issues encountered in this project.  However, in an effort to ensure that both the output that is displayed within the terminal and the output that is contained within the text file that is created each were identical to the examples provided, a slightly less-efficient approach to the creation of the output strings was taken to account for the slight differences in "\n" new line characters between the terminal output and the text file output in the examples provided in the instructions for this challenge.

![Terminal Output](/Resources/terminal_output.png)

![Text File Output](/Resources/text_file_output.png)
