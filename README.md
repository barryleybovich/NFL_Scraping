scraping
========

this is a scraper of NFL data as a personal introduction to node.js and scraping. this uses cherrio.

==========================================================================================================

mpos1.js is a script that takes position, statistic, and year inputs (run as 'node receiver.js *{position}* *{test}* *{year}*')
where {position} can be qb for quarterbacks, or rec for receivers, for qbs, test can be yardsPerInt, attemptsForTD, or ratingToSacks and for receivers, test can be recPercentage, recYardsPerAttempt, or distanceDownfield. Year is optional, and can be any integer, although leaving it blank, or any year less than 2002 or greater than 2013 will revert to 2013.

example input/output

node mpos1.js qb attemptsForTD 2009
In 2009, Drew Brees passed for a touchdown once for every 15.12 times he threw the ball.

node mpos1.js qb yardsPerInt 2010
In 2010, Tom Brady gained about 975 yards for every interception he threw.

======================================================================================================================================================================================

receiver.js is the first stable file allowing multiple inputs (run as 'node receiver.js *{test}* *{year}*')
where test can be receiverPercentage, recYardsPerAttempt, or distanceDownfield. year can be any integer, although any year less than 2002 or greater than 2013 will revert to 2013.


example input/output:

node receiver.js receiverPercentage 2012
Of 400 recievers, the average reception percentage was 61.92%
Randall Cobb had the best recieving percentage (minimum 50 receptions) with 76.92% receiving on 104 targets

node receiver.js distanceDownfield 2004
David Givens catches furthest downfield (min  50 receptions)  with catches an average of 15.61 yards downfield

node receiver.js recYardsPerAttempt 2010
Mario Manningham had the most yards per targets (min 50 receptions)  with 10.26 yards per target


