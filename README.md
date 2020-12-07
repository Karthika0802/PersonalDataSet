# Maine 2018 Ranked Choice 2nd District House Race Results

## Motivation

In the United States and indeed many other nations around the world, many feel they have a lack of choice due to being locked into a two party system. It is often asserted that the main culprit of the lack of additional parties in many of these nations is due to their voting system - which is usually plurality voting. However certain cities, states and nations use other voting methods instead, including but not limited to: Borda Count, Proportional Represenation and Single Transferable Vote.

Within the United States, states such as Maine and more recently Alaska have made the switch over to a form of Ranked Choice voting called Instant Runoff Voting. In this sytem, voters could rank all candidates on the ballot as multiple rounds of election take place, as the lowest candidate is eliminated and have their votes redistributed to the voters' next choice. I was motivated to look at the 2018 race for Maine's 2nd District for the House, specifically as it is a high profile case where a candidate won through Instant Runoff Voting when they would have lost in regular plurality voting. 

## Data Sources

Maine's Department of the Secretary of State's Bureau of Corporations, Elections & Commissions releases certified results publicly. Personally I downloaded the data from http://electionresources.org/us/data/ as it was more combined whereas the official Maine SoS Data was split into various spreadsheets.

## Processing Steps

The data required quite a bit of processing, as all which was provided was the data itself, which required manual tabulation on my part. To do this I created a seperate column of the 1st, 2nd and 3rd rounds of the vote. For each of these rounds, I would do the following

1. Copy the previous round's votes (or the 1st pref in the case of the 1st vote section)
2. Declare any Overvotes as invalid
3. Eliminate the lowest ranking remaining candidate
4. Redistribute their votes to the next valid candidate on their preferences. If there was none it would be counted as invalid

## Visualization

The following is a visualization of the round by round results

![1st round](https://github.com/Karthika0802/PersonalDataSet/blob/master/1st%20round%20vote.png)
![2nd round](https://github.com/Karthika0802/PersonalDataSet/blob/master/2nd%20round%20vote.png)
![3rd round](https://github.com/Karthika0802/PersonalDataSet/blob/master/3rd%20round%20vote.png)



