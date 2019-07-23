# a2downvoting

cityscrape: summarize the vote totals in a recent ann arbor election.

usage: cityscrape mon year

where mon is a month -- usually may, aug, or nov -- and year is four-digit year

example: cityscrape aug 2013  # also this is the earliest date that works

cityscrape retrieves and caches web pages from the washtenaw county election site.  (the size of the cache for a given election is less than 2 MB.)  output is sorted by vote total.

running cityscrape might take a half minute or so the first time for a given election.  subsequent runs are instant-ish.

cityscrape reports:
	Registered Voters
	Total Ballots Cast
	Ballots cast for each city-wide race

cityscrape also reports if a race is partisan, and if it was unopposed (except for write-ins)

sometimes there are no city-wide races, e.g., nov 2015


wardscrape is a worker script that converts the html for a specific precinct + ward report into text.


###

TODO

###

combine results from primaries, whcih can be recognized as races starting with one of the following words

	DEM, REP, LIB, D, R, L

(followed by a space)

this will fix a bug in the counting of partisan primaries


it is possible to decode elections earlier than aug 2013 ... but maybe it's not worth it.
