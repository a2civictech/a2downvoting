# a2voting

cityscrape: summarize the vote totals is a recent ann arbor election.

usage: cityscrape mon year

where mon is u month -- usually may, aug, or nov -- and year is four-digit year

cityscrape retrieves and caches web pages from the county election site.  the size of the cache for a given election is less than 2 MB.

example: cityscrape nov 2018

wardscrape is a worker script that converts a specific precinct and ward html report into text.
