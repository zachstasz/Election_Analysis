# Election_Analysis

## Project Overview
A Colorado Board of Elections employee has given the following tasks to complete the election audit of a recent local election.

1. Calculate the total number of votes cast
2. Get a complete list of candidates who received votes.
3. Calculate the total number of votes each candidate received.
4. Calculate the percentage of votes each candidate won.
5. Determine the winner of the election based on popular vote.
6. The voter turnout for each county.
7. The percentage of votes from each county out of the total count.
8. The county with the highest turnout.

## Resources
- Data Source: election_results.csv
- Software: Python 3.6.1, Visual Studio Code, 1.38.1

## Election Audit Results
The analysis of the election show that:
- There were 369,711 votes cast in the election.
- The candidates were:
    - Charles Casper Stockham
    - Diana DeGette
    - Raymon Anthony Doane
- The candidate results were:
    - Charles Casper Stockham received 23.0% of the vote and 85,213 number of votes.
    - Diana DeGette received 73.8% of the vote and 272,892 number of votes.
    - Raymon Anthony Doane received 3.1% of the vote and 11,606 number of votes.
- The winner of the election was:
    - Diana DeGette, who received 73.8% of the vote and 272,892 number of votes.
- The county results were:
    - Jefferson's turnout was 10.5% of the vote and 38,855 number of votes
    - Denver's turnout was 82.8% of the vote and 306,055 number of votes
    - Arapahoe's turnout was 6.7% of the vote and 24,801 number of votes
- The county with the highest turnout was:
    - Denver, whose turnout was 82.8% of the vote and 306,055 number of votes

![Results](https://user-images.githubusercontent.com/103209236/166824215-371d6580-1f98-4d9b-a8af-9b4997be83d8.PNG)

## Election Audit Summary
Using this script, I was able to loop through all the data and analyze the votes by how many, county, and candidate. 

This script could be used with any election by modifying it to suite varies election's needs.

You would first need to modify the upload data. As seen below, just replace "election_results.csv" with another csv file. 

![Example1](https://user-images.githubusercontent.com/103209236/166825360-f877b2d4-4c05-4bfd-bf3e-7e04b8adc36a.PNG)

Provided the ID, county, and candidate are in the same columns, it will work with the new data. If not, then adjust accordingly. As seen below, since the county name is in the 2nd column, we were able to extract the data using row[1]. If the candidate name is in the 2nd column, than it would be candidate_name = row[1] instead.

![Example3](https://user-images.githubusercontent.com/103209236/166826091-83ce679a-8962-465d-9e26-f2a9cf4a6a78.PNG)

Another modification may be how the winner is decided. Instead of the winner being the one that got the most votes, perhaps the winner is weighed by county results. Or if the vote is close enough, there is no winner and a run-off election would need to take place. The winner in this script is the highest vote getter

![Example4](https://user-images.githubusercontent.com/103209236/166826874-9f16fe23-ab20-472c-9858-2a977d8b49d4.PNG)

However, you could say there is no winner if a candidate's votes are within a certain range of another candidates.


