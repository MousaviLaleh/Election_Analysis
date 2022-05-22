## Election Analysis

### Overview of Election Audit
A Colorado Board of Elections employee has given us the following tasks to complete the election audit of a recent local congressional election. Since we are asked to automate the whole audit process in order to use for senatorial and local elections, we will use [Python](https://www.python.org/doc/essays/blurb/) for this project.<br/>

### Purpose
We are tasked with reporting the : 
- The voter turnout for each county
- The percentage of votes from each county out of the total count
- The county with the highest turnout
- The total number of votes cast
- The total number of votes for each candidate
- The percentage of votes for each candidate
- The winner of the election
<br/>

#### Resources
:card_file_box: Data Resources : [election_results.csv](/resources/election_results.csv)<br/>
:card_file_box: Output File : [election_analysis.txt](/analysis/election_analysis.txt)<br/>
:card_file_box: Software : [Python 3.6.1](https://www.python.org/downloads/windows/),  [Visual Studio Code 1.38.1](https://code.visualstudio.com/download)
- Note : use 'Windows x86-64 executable installer' for Python, and 'System Installer' version of VS-code 
<br/>

### Election Audit Results
The analysis of the election show that:
- There were 369,711 votes cast in the election.
- The counties were: 
    - Jefferson :  with 38,855 number of votes and 10.5% of the vote.
    - Denver :  with 306,055 number of votes and 10.5% of the vote.
    - Arapahoe :  with 24,801 number of votes and 6.7% of the vote.

- The candidates were:
    - Charles Casper Stockham :  with 85,213 number number of votes and 23.0% of the vote.
    - Diana DeGette :  with 272,892 number number of votes and 73.8% of the vote.
    - Raymon Anthony Doane :  with 11,606 number of votes and 3.1% of the vote.

- **Denver** county had the largest number of votes.

and <br/>
- **The winner** of the election was:
    - Candidate **Diana DeGette**, who received **73.8%** of the vote and **272,892** number of votes.
<br/>

### Election Audit Summary
There is a statement to the election commission that explores how this script can be used for any election, with two examples for modifying the script.  (4 pt)

Using a programming language like Python, and writing scripts in Python has many advantages like automating processes, fast execution of the code, and reusing the code for similar projects. This code quickly returns numerous data for a U.S. Congressional Precinct in Colorado, but can be easily used but for other elections as well. This code will automatically:
- find candidates names,
- find counties,
- count votes for each candidate and calculate vote percentage,
- count turnout per county and calculate their percentage,
- declare a candidate winner base on the highest vote count and percentage,
- declare a county with the highest turnout.<br/>
This code can be used on similar projects such as other congressional district elections, senatorial districts, local elections, and more.<br/>
- This code reads csv files but can be easily converted to read other files such as json, by importing other dependencies for example import json.
- By changing your source file-name and/or address, you can easily handle any amount of data in .csv file with the same structure of election_result.csv file.<br/>
![01.png](/resources/images/01.png) <br/>
- This code reads candidate name on 2nd index and county on 1st index, but in case of a different structure of the data set this lines of codes can be easily converted. <br/>
![02.png](/resources/images/02.png) <br/>

<br/>
