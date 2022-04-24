# election_analysis


## Overview of Election Audit:

I assisted a Colorado Board of Elections employee, Tom, in an election audit of the tabulated results for a US Congressional District in Colorado. I was tasked with reporting:
* The total number of votes cast
* The total number of votes and percentage of vote for each candidate
* The winner of the election based on popular vote

This task is usually done in Excel, but Tom's manager wanted to know if there is a way to automate the process using Python. If this audit is done successfully with Python, the code would be used to audit other districts and local elections. After the votes were counted it was my job to certify this US Congreessional race.

Below, a sample of the dataset in CSV file. This was the data format I ran the Python code through to audit the congressional election results.

<img width="250" alt="csv_election_results" src="https://user-images.githubusercontent.com/102890151/164986645-36ee56e9-ee5d-4d31-9008-c8ecfa95008c.png">




## Election-Audit Results


* ### How many votes cast in this congressional election

I used Visual Studio to write Python for the audit. After establishing read and write connections to the data and outfiles (election summarry and results) the first task was to count of the number of total votes. To count up all the votes, I needed to initialize a variable. For convenience, I initialized a variable called total_votes to zero. This variable which is called an accumulator, increments by 1 as it reads each row in the for loop as it calculates the total votes cast. **Total vote count for this US congressional election was 369,711.**

Initializing variable in code (Viewed below)

<img width="387" alt="total_vote" src="https://user-images.githubusercontent.com/102890151/164986772-4aeee55b-c9c1-4346-b374-35fa4d754050.png">


* ### Number of votes and percentage for each county and highest county voter turnout

As the audit was winding down the election commission requested some additional data to complete the audit which included the voter turnout for each county, 
the percentage of votes from each county out of the total count and finally, the county with the highest turnout.

Snapshot of the outfile I created summarizing the election results (Image 1 below) for the audit. **Jefferson had 10.5% of the votes at 38,855. Arapahoe had 6.7% of the toal vote or 24,801 votes. Denver county at 82.8% of the votes (largest percent) and 306,055 votes which was the largest number of votes of the three counties.**



Image 3 (beloww) election summary

<img width="375" alt="Screenshot (47)" src="https://user-images.githubusercontent.com/102890151/164957031-fbe5ac78-b22d-48b3-8093-7188413a0b8d.png">

Working from the original dataset (csv file) I used for loops and conditional statements with membership and logical operators to find the number of votes and percentage of total votes for each county (Seen in image below). Then I, print the results to the command line and saved them to the election_results.txt file (image 3 above)

<img width="377" alt="county_votes_code" src="https://user-images.githubusercontent.com/102890151/164983603-9651e510-20bc-4dfb-96b4-577635ae2b05.png">


Provide a breakdown of the number of votes and the percentage of the total votes each candidate received.

We can count the votes for each candidate while we are in the if statement. As we iterate through each row of the CSV file, we can increment the votes for each candidate by 1. However, we need to link those votes with a candidate. A convenient way to do this is to create a dictionary where the key is each candidate's name and the vote count for that candidate is the value for the key.

The structure of the dictionary may look similar to this:

Which candidate won the election, what was their vote count, and what was their percentage of the total votes?

##Election-Audit Summary: 

In a summary statement, provide a business proposal to the election commission on how this script can be used—with some modifications—for any election. Give at least two examples of how this script can be modified to be used for other elections.
