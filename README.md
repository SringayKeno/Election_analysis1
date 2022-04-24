# election_analysis


## Overview of Election Audit:

I assisted a Colorado Board of Elections employee, Tom, in an election audit of the tabulated results for a US Congressional District in Colorado. I was tasked with reporting:
* The total number of votes cast
* The total number of votes and percentage of vote for each candidate
* The winner of the election based on popular vote

This task is usually done in Excel, but Tom's manager wanted to know if there is a way to automate the process using Python. If this audit is done successfully with Python, the code would be used to audit other districts and local elections. After the votes were counted it was my job to certify this US Congreessional race.

Below, a sample of the dataset in CSV file. This was the data format I ran the Python code through to audit the congressional election results.

<img width="350" alt="election_results" src="https://user-images.githubusercontent.com/102890151/164954437-cef85d1b-0669-44bf-9587-028a03ed545f.png">


## Election-Audit Results: 

### How many votes cast in this congressional election

I used Visual Studio to write Python for the audit. After establishing read and write connections to the data and outfiles, the first task was to count of the number of total votes. To count up all the votes, I needed to initialize a variable. For convenience, I initialized a variable called total_votes to zero. This variable which is called an accumulator, increments by 1 as it reads each row in the for loop as it calculates the total votes cast. **Total vote count for this US congressional election was 369,711.**

Initializing variable in code (Viewed below)

<img width="400" alt="total vote counter" src="https://user-images.githubusercontent.com/102890151/164955859-349e1b14-6689-4514-9021-b76ea4d23268.png">











Which county had the largest number of votes?
Provide a breakdown of the number of votes and the percentage of the total votes each candidate received.
Which candidate won the election, what was their vote count, and what was their percentage of the total votes?

##Election-Audit Summary: 

In a summary statement, provide a business proposal to the election commission on how this script can be used—with some modifications—for any election. Give at least two examples of how this script can be modified to be used for other elections.
