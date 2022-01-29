# Module_04_Challenge
Module 04 Challenge - PyCity Schools Analysis

# Module_03_Challenge
Module 03 Challenge - Election Analysis

## Overview of Project
Module 3 Challenge. This project involves using Python to tabulate the results of a recent election for U.S. Representative for a Congressional District in Colorado.

### Purpose
The purpose of this challenge is to take a CSV file containing data related to each of the ballots cast in the election, and provide results including the total number of votes cast, the number of votes cast by County and the percentage of the total vote associated with each County, the number of votes cast for each candidate and each candidate's percentage of the total number of votes cast, and an ascertainment of the candidate receiving the greatest number of votes.   

## Election Audit Results
The results of our Election Audit are as follows:

- Total Number of Votes Cast: 369,711

- Total Votes by County, and Percentage of Total Votes Cast:
  - Jefferson County: 68,855 (10.5%)
  - Denver County: 306,055 (82.8%)
  - Arapaho County: 24,801 (6.7%)

- Denver County had the greatest number of votes cast, with 306,055 votes cast, accounting for 82.8% of the total number of votes cast,

- Total Votes for Each Candidate, and Percentage of Total Votes Cast:
  - Charles Casper Stockham: 85,213 (23.0%)
  - Diana DeGette: 272,892 (73.8%)
  - Raymon Anthony Doane: 11,606 (3.1%)

- Diana DeGette won the election, with a total of 272,892 votes out of the 369,711 total votes cast - 73.8% of the total number of ballots tabulated.

## Election Audit Summary

There are multiple ways in which the Python script utilized for this project could be utilized for other elections - either with or without additional modification.

1. There is nothing specific to this script that would limit its use to this particular race or this specific Congressional District - the lists of Counties and Candidates are based on values contained within the election_results.csv file that is provided, allowing for this same script to be utilized in other races without requiring any modification of the script.


2. With minimal modification, this script could be utilized in instances where there are multiple races associated with a single ballot - for example, a ballot could contain votes in races for President, Senate, and House of Representatives.  One approach to facilitating this functionality would be to include an additional column in the election_results.csv file that denotes the specific Race that a choice is associated with - for example, adding "Race" to the existing fields of "Ballot ID", "County" and "Candidate", resulting in a single "Ballot ID" being associated with multiple records - one for each Race in which a selection was made.  The script could then be modified to create a Dictionary containing a list of each of the races being contested, much as is currently done to create a Dictionary containing each of the Candidate Names and County Names.  Using a "For/Each" approach for each of the "Races" contained in the new "Races" dictionary, with the existing code nested within it and with only minor modifications, it would then be possible to tabulate votes for multiple races through the use of a single election_results.csv file and single Python script, yielding output for each race being contested.      

## Limitations

There were no issues encountered in this project.  However, in an effort to ensure that both the output that is displayed within the terminal and the output that is contained within the text file that is created each were identical to the examples provided, a slightly less-efficient approach to the creation of the output strings was taken to account for the slight differences in "\n" new line characters between the terminal output and the text file output in the examples provided in the instructions for this challenge.

![Terminal Output](/Resources/terminal_output.png)

![Text File Output](/Resources/text_file_output.png)
