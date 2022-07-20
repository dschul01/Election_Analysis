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

* **County Votes**
	|County|Vote Count|Vote Percentage|
	|------|----------|---------------|
	|Jefferson|38,855|10.5%|
	|Denver|306,055|82.8%|
	|Arapahoe|24,801|6.7%|

* **Largest County Turnout**: Denver with 306,055 votes

* **Votes Per Candidate**
	|Candidate|Vote Count|Vote Percentage|
	|---------|----------|---------------|
	|Charles Casper Stockham|85,213|23.0%|
	|Diana DeGette|272,892|73.8%|
	|Raymon Anthony Doane|11,606|3.1%|

* **Winning Candidate**: Diana DeGette with 272,892 votes and 73.8% of the votes


There are two stocks, ENPH and RUN, over the period which are revealed as providing positive results YoY.  The code seen below makes it quite easy to visualize by highlighting the positive returns in green seen in the output.
![Formatting_Code.png](https://github.com/dschul01/stock-analysis/blob/main/Resources/Formatting_Code.png)
![Positive_Returns_YoY.png](https://github.com/dschul01/stock-analysis/blob/main/Resources/Positive_Returns_YoY.png)
### Refactoring Impacts
The initial code was enhanced using an index for all the ticker's performance measurement loops and resulted in significant time reductions to run the code as seen in the images below.  The time differential would be even greater if the volume of stocks to analyze increased.
![Refactored_Time_Impacts.png](https://github.com/dschul01/stock-analysis/blob/main/Refactored_Time_Impacts.png)
## Summary
### Advantages of Refactoring Code
There are several advantages of refactoring code.  It leads to better quality code making it more manageable and cleaner for the original programmer or others who might need to update it in the future.  The process of refactoring will also help in finding bugs which might not have originally occurred when running initial use cases.  It also often reduces run times as it leads to removing unnecessary code.  

The refactoring for this particular project resulted in all the advantages listed.  The original code had unnecessary lines of code which made the performance run over 6 times longer before refactoring.  The new code is cleaner and runs much quicker as seen in the Results above.
  
### Disadvantages of Refactoring Code
There are also disadvantages of refactoring code.  Refactoring takes time and money. A programmer must go back through the code deciphering what it's doing and then use resources to refactor.  There are possibilities refactoring does not improve timeliness and could break other applications which depend on the source code being adjusted.

The refactoring for this particular project resulted in the use of additional hours spent to create better quality code.  However, the resulting 6x time savings made it a worthwile endeavor.

