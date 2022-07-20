# Election_Analysis
Performing analysis on a local Colorado election utilizing Python to determine winning candidate

## Overview of Election Audit
### Purpose
The purpose of this project was to utilize Python to automate the task of reading election results saved in a CSV file and providing summarized results for the election commission.  For loops and conditional statements were implemented in order to run through the large dataset and quickly determine the election commission's requested data points:

* The voter turnout for each county 
* The percentage of votes for each county out of the total count
* The county with the highest turnout
* The vote count by candidate along with percentage of votes
* Winning candidate highlighted with respective bote count and percentage of votes

## Election Audit Results
The following is a breakdown of the votes by county and candidate as well as highlighting the county with largest turnout and winning candidate.

* **Total Votes Cast**: 369,711

* **Votes Per County**:
	|County|Vote Count|Vote Percentage|
	|------|----------|---------------|
	|Jefferson|38,855|10.5%|
	|Denver|306,055|82.8%|
	|Arapahoe|24,801|6.7%|

* **Largest County Turnout**: Denver with 306,055 votes

* **Votes Per Candidate**:
	|Candidate|Vote Count|Vote Percentage|
	|---------|----------|---------------|
	|Charles Casper Stockham|85,213|23.0%|
	|Diana DeGette|272,892|73.8%|
	|Raymon Anthony Doane|11,606|3.1%|

* **Winning Candidate**: Diana DeGette with 272,892 votes and 73.8% of the votes

All the data points above were calculated using Python code with a couple images provided below to illustrate how some of the calculations were derived and showing how results were also printed to the Terminal.

**Largest County Turnout Code Sample**:
![Largest_County_Turnout_Calc_Sample.png](https://github.com/dschul01/Election_Analysis/blob/main/Resources/Largest_County_Turnout_Calc_Sample.png)

**Winning Candidate Code Sample**:

![Winning_Candidate_Calc_Sample.png](https://github.com/dschul01/Election_Analysis/blob/main/Resources/Winning_Candidate_Calc_Sample.png)

Additionally the results were written to the text file, [election_results.txt](https://github.com/dschul01/Election_Analysis/blob/main/Analysis/election_results.txt) via the code so the election commission can reference them as they need.

## Election Audit Summary
This script can be utilized for any election as the code reads the output of election results which are in a CSV file.  The only necessity is that the object location within the CSV file remains consistent (e.g. ballots in first column, location in second column, etc.) The County column of the CSV file could be replaced with any region such as city or state.  I would suggest two changes to the code to prevent needing to customize the code for each election.
1. The code could be modified to change the value and output for the 1st Index, currently holding the county string, to be more generic such as region.  All value, lists and dictionary references to county within the code would be adjusted to this generic label.
2. The code could also be modified to identify if the objects in the CSV were in a different order than the original county data.  This would eliminate the dependency for the data files to be in the same object/column order as each region might submit their input files differently.  

