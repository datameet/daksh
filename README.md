daksh
=====

Daksh Voter Perception Data [from Daksh India](dakshindia.org)



The way our data is organized
==============================

This is from [Daksh blog](http://blog.dakshindia.org/2014/03/the-way-our-data-is-organized.html)

This post is specifically for people who are looking at either the detailed survey data or at least the Constituency-level summaries of our data. So if you're not one of those serious data-monkeys, begone!

OK, now that only the true believers are here, let me first talk about the CSV. The CSV is a complete representation of all the data collected on a given survey form (you can see a template in English here). Here's a brief explanation:
The data begins with a set of demographics - location type, gender, etc.) and each row has the actual selection of the respondent, as seen on the form.
The data then goes on to show information about the voter's preferences in terms of whom s/he will vote for, why, etc.
Thereafter comes the most important part: the importance and performance relating to each issue, in in two sets of columns. For example, the first issue that someone could  respond to is "Agricultural loan availability". In the CSV, you will see a column marked "I: 24 1 Agricultural loan availability", followed by one marked "P: 24 1 Agricultural loan availability". The I: 24... columns carry the original selection of the respondent: Low, Medium or High. The P: 24... columns, again, are the original response and they carry values of Bad, Average or Good.
After the selection columns, there are some "control" columns, including a unique ID for each record.
After the control columns, to make calculations easier, we've added numerical translations of the selections: Low becomes 1, Medium - 2 and High - 3. So also, on the Performance side, Bad becomes 1, Average - 2 and Good - 3. There are such translation columns for every pair of issue-related Importance and Performance columns.
Following the calculation base columns, we have Scores for each Issue. The Score for an issue is calculated as Issue * Performance * 10 / 9, to get all numbers on a "base" of 10.
After the last Score (Traffic congestion), we have an Average Score, calculated using only non-zero values (therefore ignoring issues that the respondent has not responded to).
Finally, we have a WealthIndex, a numerical representation of the assets that the respondent owns (taken with points for cattle, TV, motorobike and car, all of which appear in the Demographics section of the record).
That's about the CSV. The other online chart that you can look at is the Constituency Summaries that you can find here. The chart has four tabs. The first three (surprisingly named Issues, Performance and Scores!) are summaries of the columns from the CSV, but separated into their own sheets for eay assessment. For example, if you want to see what the newspapers and TV channels have been carrying as numbers for each Constituency, you can look at the Performance tab. If you want to see what we at Daksh think is the way the MP has done, look at the Scores tab. And the Issues tab will tell you what the issues are in each Constituency (although you'll have to copy out the issues in the header and their scores and then sort them as you see fit). The last tab is a summary of the Issues, Performance and Scores at a National level, averaging each element. This tab therefore provides a National backdrop to compare local issues, performance and scores with.
Hope this helps. If you have questions, please feel free to comment below and we'll respond as quickly as we can.
