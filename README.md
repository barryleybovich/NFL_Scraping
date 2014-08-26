scraping
========

this is a scraper of NFL data as a personal introduction to node.js and scraping. this uses cherrio.

receiver.js is the first stable file allowing multiple inputs (run as 'node receiver.js *{test}* *{year}*')
where test can be receiverPercentage, recYardsPerAttempt, or distanceDownfield. year can be any integer, although any year less than 2002 or greater than 2013 will revert to 2013.


example input/output:

node receiver.js receiverPercentage 2012
Of 400 recievers, the average reception percentage was 61.92%
Randall Cobb had the best recieving percentage (minimum 50 receptions) with 76.9
2% receiving on 104 targets

node receiver.js distanceDownfield 2004
David Givens catches furthest downfield (min  50 receptions)  with catches an av
erage of 15.61 yards downfield

node receiver.js recYardsPerAttempt 2010
Mario Manningham had the most yards per targets (min 50 receptions)  with 10.26
yards per target



qbtest is an expansion that will provide receiver or qb data depending on input
