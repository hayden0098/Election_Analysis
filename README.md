# Election_Analysis

## Overview of Election Audit:
In the Colorado Board of Elections; Tom, a employee in an eleciton auidt of the tabulated results for U.S. Congressional precinct in Colrado has provided a CSV file that need to be working with to get the Total number of votes cast and a complete list  of candidates who reeived votes. In the list of candidates, total number and percentage of votes for each candidate and the winner from the election are the informations must be included. At last, regarding to the request from election commission the voter turnout, percentage of votes out of the total count from each county and the name of county with highest turnout are the additional data need to be completed on the final result analysis. The work will be done on automate the process by using Python.

## Election Audit Resaults:
- ###### How many votes were cast in this congressional election?
  From this congressional election, there were 369,711 votes in total.

- ###### Provide a breakdown of the number of votes and the percentage of total votes for each county in the precinct.
  !(County Votes)[]

  From the analysis of the data, the image have show us the number of votes and the percentage of total votes for each county in the precinct. Jefferson has the 10.51% of the     total vote which is 38,855 votes; Denver has the 82.78% of the total vote which is 306,055 votes; Arapahoe has the 6.71% of the total vote which is 24,801 votes.

- ###### Which county had the largest number of votes?
  Denver is the county who carry the largest number of votes, since the 82.78% of the total vote which is 306,055 votes is the highest number of count compare than the others.

- ###### Provide a breakdown of the number of votes and the percentage of the total votes each candidate received.
  !(Candidate Votes)[]

  From the analysis of the data, the image have show us the number of votes and the percentage of total votes for each candidate. Charles Casper Stockham received 85,213 votes     that are 23% of the total votes; Diana DeGette received 272,892 votes that are 73.8% of the total votes; Raymon Anthony Doane received 11,606 votes that are 3.1% of the total   votes.

- ###### Which candidate won the election, what was their vote count, and what was their percentage of the total votes?
  As the final reuslt of the data analysis for this congressional election in Colorado, the winner of the election is candidate Diana DeGette. She has the most vote count of       272,892 votes, and the most winning percentage of 73.8%.

## Election Audit Summary:
As a automatical process Python script, it's suitable to use in election commission to get the result for any election with some modifacations are needed. 

1. After the statement that open the loaded file, inside the loop that used to read every rows of the file. the number of column in CSV file that indicate candidate name and county name may not be the same in every election based on the file that generated, so this would be the small modification is require to be done. 

  for example: candidate_name = row[number] 
                county_name = row[number] where number = 0 ~ (column # - 1 )

2. While setting the variable that want to load or save the file from a path, in side the os.path.join() statement filename variable and direct path in this case is name "election_results.csv" that in the path that folder name "Resources". In other case, the file name that has beed provided may not be the same in each election. Also the direct path would be different which mean the data file may not be in the same folder as the last time. Therefore inspection and modifications the path will be neccessary for every time using this script, and make the change as needed.

  for example: os.path.join("folder name","file name"); ".." can be added infront of
