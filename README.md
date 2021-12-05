# Election Audit

## Overview
Tom is a Colorado Board of Elections employee who needs help with an election audit for a US Congressional Preccint. The data comes in tabulated results and needs to be counted in order to report total number of votes as well as the amount of votes each candidate got. With such numbers in hand, percentages are calculated and the winner is certified. Such task is usually done in Excel, but the idea is to automate the process using Python. 

## Election Audit Analysis
After our Python script ran and analysed the ballots cast, we came to the final results:

* In total, 369,711 votes were cast comprising three counties: Arapahoe, Denver and Jefferson;

* The distribution of votes cast per county was as follows - being Denver the one with the largest turnout:
    * Arapahoe: 24,801 (6.7%)
    * Denver: 306,055 (82.8%)
    * Jefferson: 38,855 (10.5%)

* The breakdown of number of votes per candidate is as follows:
    * Charles Casper Stockham: 85,213 (23.0%)
    * Diana DeGette: 272,892 (73.8%)
    * Raymon Anthony Doane: 11,606 (3.1%)

* **Diana DeGette** was the winner candidate. She got **272,892 votes** out of 369,711 - totalling **73.8%** of the total votes - an impressive almost three-quarters of the cast votes!

The computed results were shown on the screen right after the script ran:
![terminal_results](/resources/terminal_results.png)

## Election Audit Summary
The audit was a success! Within a few seconds, all votes were counted and the winner was announced - with very little human intervention - given all we had to do was to run the script.

A similar process can be used to count votes for any election as long as the data is in the correct format and a few adjustments are made. We could point a few scenarios like:
* In a similar scenario as the proposed one, but for the entire state, meaning counting the votes for all congressional districts for the entire state in one single election. If the District information is not already in the data along with the ballots, we can create a Dictionary linking each County to its corresponding Congressional District. The script would have to deliver one more total (list): votes per District. This could be handled in a similar way as the totals for counties or candidates or could just be made up by summing up the totals for all counties in a given District after the main loop in the script. Another modification we anticipate is to have the key for the candidate dictionary as County-Candidate instead of just Candidate because there may be two candidates with the exact same name running for different districts and their votes should be counted accordingly - this might not be necessary if the state enforced different names before the election.
* In a scenario where votes for Governor are being counted, on the other hand, we would not necessarily need the County information - unless we want the breakdown of how many votes each candidate gets by County.

It is very important to state that this algorithm can be applied with minor changes in different scenarios as long as the winner is based on popular vote. If, for instance, an election calls for electoral vote, a more serious code review might take place to reflect the results properly.

