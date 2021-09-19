# Election_Analysis

## Project Overview
A Colorado Board of Elections employee has given us the following tasks to complete the election audit of a local congressional election.

1. Calculate the total number of votes cast.
2. Get a complete list of candidate who received votes.
3. Calculate the total number of votes each candidate received.
4. Calculate the percentage of votes each candidate won.
5. Determine the winnder of the election based on the popular vote.
6. Get a complete list of the counties where votes were cast.
7. Calculate the total number of votes cast in each county.
8. Calculate the percentage of the total vote for each county.
9. Determine the county with the largest voter turnout.

## Resources
- Data Source: election_results.csv
- Software: Python 3.8.8, Visual Studio Code 1.60.0

## Election-Audit Results
The analysis of the election show that:
- There were 369,711 votes cast in the election.

<img width="191" alt="Election Results" src="https://user-images.githubusercontent.com/89098766/133939286-423b8f00-a686-4f39-a23c-d41347510787.png">

- The Candidates were:
  - Charles Casper Stockham
  - Diana DeGette
  - Raymon Anthony Doane
- The Candidate results were:
  - Charles Casper Stockham received 23% of the vote with 85,213 votes.
  - Diana DeGette received 73.8% of the vote with 272,892 votes.
  - Raymon Anthony Doane received 3.1% of the vote with 11,606 votes.
- The winner of the election was:
  - Diana DeGette with 73.8% of the vote and 272,892 votes.
 
 <img width="290" alt="Candidate votes" src="https://user-images.githubusercontent.com/89098766/133939301-0fe2a705-08d9-43c5-b717-602d67a9e7e7.png">

- The County results were:
  - Jefferson county accounted for 10.5% of the total vote with 38,855 votes.
  - Denver county accounted for 82.8% of the tota vote with 306,055 votes.
  - Arapapoe county accounted for 6.7% of the total vote with 24,801 votes.
 - The largest county turnout was:
  - Denver county with 82.8% of the vote with 306,055 votes.

<img width="245" alt="County Turnout" src="https://user-images.githubusercontent.com/89098766/133939306-34097f00-06d3-4fe0-b398-6e82691e2be6.png">

## Election-Audit Summary

The script used to perform this audit can be used for any election with some modifications. The data source was written directly into the code which could be changed to pull the same information for another election.  

<img width="495" alt="Data source" src="https://user-images.githubusercontent.com/89098766/133939520-8b94e2e3-df61-4649-bb25-9cc9dcce220f.png">

The new data source ideally would have the same structure in order to use the existing code to pull candidate names, counties and votes. If the data was formatted differently, our existing code could be modified to pull the corresponding data from new columns within the data source. See below, our code is pulling candidate name from column 3 and county name from column 2 in election_results.csv. This could easily be changed to match where the data is coming from in a new data source.

<img width="332" alt="Column sources" src="https://user-images.githubusercontent.com/89098766/133939700-b4a22b81-31c1-4b77-83e3-863e3bad4564.png">

The same repetiton and condition statements could be used for other elections as long as the code is modified to pull the correct data from the correct location within the new data source. These statements are set up to pull information from established data source based on variables. In our case the variables are set as candidate, county, votes, percetages, election winner, and largest county turnout, so the data source could change but would still produce the desired outcome (i.e. election winner, voter turnout per county).

The analysis we have done here to provides valuable information for the election board.The script could be modified further to find new insights in the data. For example we can add furhter decision statements to pull how many votes and the percentage of the vote each candidate got per county. If new election data sources provided part infomation, we could modify the code to produce turnout by party for both the entire election and per each county. Overall this script is capable of not only being used for future elections, but also can be modified to produce a variety of different results based on what the election board wants to analyze.
