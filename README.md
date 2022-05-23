## Election Analysis

### Overview of Election Audit
A Colorado Board of Elections employee has given us the following tasks to complete the election audit of a recent local congressional election. Since we are asked to automate the whole audit process in order to use for senatorial and local elections, we will use [Python](https://www.python.org/doc/essays/blurb/) for this project.<br/>

### Purpose
We are tasked with reporting : 
- The voter turnout for each county
- The percentage of votes from each county out of the total count
- The county with the highest turnout
- The total number of votes cast
- The total number of votes for each candidate
- The percentage of votes for each candidate
- The winner of the election


#### Resources
:card_file_box: Data Resources : [election_results.csv](/resources/election_results.csv)<br/>
:card_file_box: Output File : [election_analysis.txt](/analysis/election_analysis.txt)<br/>
:card_file_box: Software :  [Python 3.6.1](https://www.python.org/downloads/windows/) &#44;  [Visual Studio Code 1.38.1](https://code.visualstudio.com/download)
- Note : use 'Windows x86-64 executable installer' for Python, and 'System Installer' version of VS-Code 
<br/>

### Overview of the methods and code
#### :black_medium_square: Open, read & write the file
One of the most important steps in data analytics is opening, reading, and writing a file. Opening and reading a file is the first step that needs to be done in order to start data analysis.<br/>

**1. Import dependencies**
   <p align="center"><img src="https://github.com/MousaviLaleh/Election_Analysis/blob/main/images/06.png"></p>
  
  - ```import csv``` :  allows to easily pull data from external CSV files and perform operations on them. This dependency includes the following functions:
    - next() - skips the row (most commonly used to skip a header row).
    - reader() - reads each row from the csv file and return data as a list of strings.
   
  - ```import os``` : allows to interact with the operating system. This dependency includes the following functions:
    - path() - allows us to access files on different operating systems.
    - join() - joins file path components together when they are provided as separate strings; then, it returns a direct path with the appropriate operating system separator, forward slash for macOS or backward slash for Windows

**2. Declare a variable, and load a file from the path**
 <p align="center"><img src="https://github.com/MousaviLaleh/Election_Analysis/blob/main/images/07.png"></p>
    
   - ```file_to_load``` - declaring a variable for the file.
   - ```resources``` - directory of the file.
   - ```election_results.csv``` - name of the file.
    
    Note : Directory has to be provided exactly. Letter case matters.

**3. Open and read the file** 
<p align="center"><img src="https://github.com/MousaviLaleh/Election_Analysis/blob/main/images/08.png"></p>

   - ```with open()``` - opens the file and ensures the proper acquisition of data without having to close the file, so the data isn’t lost or corrupted.
   - ```as <variable_name>``` - assigning alias to a variable.
   - ```csv.reader()``` - a new variable that will be used in the for loop to access the elements via indexes.
   - ```election_data``` - passing an argument to a function, a file that we want function to read.


**4. Declare and and skip the header row**  <br/>
this function will skip first row of data which is the header.
<p align="center"><img src="https://github.com/MousaviLaleh/Election_Analysis/blob/main/images/09.png"></p>
<br/><br/>

<p align="center">
   the full code to open and read a file<br/>
   <img src="https://github.com/MousaviLaleh/Election_Analysis/blob/main/images/10.png">
</p>
<br/>
**5. Additional code for writing a file**  <br/>


#### :black_medium_square: Looping through dictionaries and the lists
#### :black_medium_square: The get() method
#### :black_medium_square: Finding the winner
#### :black_medium_square: 

### Election Audit Results
The [analysis](/resources/images/03.png) of the election show that:
- There were 369,711 votes cast in the election. 

- The counties were: 
    - Jefferson :  with 38,855 number of votes and 10.5% out of the total votes.
    - Denver    :  with 306,055 number of votes and 10.5% out of the total votes.
    - Arapahoe  :  with 24,801 number of votes and 6.7% out of the total votes.

- The candidates were:
    - Charles Casper Stockham :  with 85,213 number of votes and 23.0% of the vote.
    - Diana DeGette           :  with 272,892 number of votes and 73.8% of the vote.
    - Raymon Anthony Doane    :  with 11,606 number of votes and 3.1% of the vote.

- **Denver** county had the largest number of votes.

- **The winner** of the election was:
    - Candidate **Diana DeGette**, who received **73.8%** of the vote and **272,892** number of votes.
<br/>
<p align="center">
   <img src="https://github.com/MousaviLaleh/Election_Analysis/blob/main/images/02.png">  --
  <img src="https://github.com/MousaviLaleh/Election_Analysis/blob/main/images/01.png"><br/>
   code output in command line  vs   text file
</p>

### Election Audit Summary
Using a programming language like Python, and writing scripts in Python has many advantages like automating processes, fast execution of the code, and reusing the code for similar projects. <br/>
This code quickly returns numerous data for a U.S. Congressional Precinct in Colorado, but can be easily used but for other elections as well. This code will automatically :
- find candidates names,
- find counties,
- count votes for each candidate and calculate vote percentage,
- count turnout per county and calculate their percentage,
- declare a candidate winner base on the highest vote count and percentage,
- declare a county with the highest turnout.

This code can be used on similar projects such as other congressional district elections, senatorial districts, local elections, and more.<br/>

- Since Python script finds unique names of candidates and counties we can reuse this code on a much larger dataset with more candidates, more counties or other areas.
- This code reads csv files but can be easily converted to read other files such as json, by importing other dependencies to the code, for example *import json*.<br/><br/>
![03.png](/images/03.png) <br/><br/>
- This code accesses the dataset in a specific directory and writes a report to a specific file, but this specific lines of codes can be easily fixed by renaming a directory and file in the code itself.<br/><br/>
![04.png](/images/04.png) <br/><br/>
- This code reads candidate name on 2nd index and county on 1st index, but in case of a different structure of the data set this lines of codes can be easily converted. <br/><br/>
![05.png](/images/05.png)<br/>
<br/>
<hr/>
  
  
  finish
