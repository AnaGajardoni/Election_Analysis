# Election Audit
Election Analysis with Python

## Overview
Tom is a Colorado Board of Elections employee who needs help with an election audit for a US Congressional Preccint. The data comes in tabulated results and the needs to be counted in order to report total number of votes as well as the amount of votes each candidate got. With such numbers in hand, percentages are calculated and the winner is certified. Such task is usually done in Excel, but the idea is to automate the process using Python. 

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

* The winner of the election was Diana DeGette, who got 272,892 votes - totalling 73.8% of the total votes.

## Election Audit Summary
The audit was a success! Within a few seconds, all votes were counted and the winner was announced - with very little human intervention given all we had to do was to run the script.
This process can be used to count votes for any election - depending on the scenario, a few changes can be 