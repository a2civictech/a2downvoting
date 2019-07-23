# a2voting

cityscrape: summarize the vote totals is a recent ann arbor election.

usage: cityscrape mon year

where mon is a month -- usually may, aug, or nov -- and year is four-digit year

example: cityscrape nov 2018

cityscrape retrieves and caches web pages from the washtenaw county election site.  the size of the cache for a given election is less than 2 MB.  output is sorted by vote total.

running cityscrape might take a half minute or so the first time for a given election.  subsequent runs are instant-ish.

cityscrape reports:
	Registered Voters
	Total Ballots Cast
	Ballots cast for each city-wide race

there may be no city-wide races, e.g., nov 2015


wardscrape is a worker script that converts a specific precinct and ward html report into text.
