Scraping info from Walkscore around Pittsburgh.

get\_walkscores.py: script to scrape all the walkscores in Pittsburgh.
Using a grid of .005 degrees lat/lon. (they only compute points on a grid and
they say their grid is about 500ft square, but it's imprecise and hard to tell
where their grid actually is.)
The default boundaries are .01 degrees square around the center of Pittsburgh.
These boundaries and granularity give about 1600 results, which can be scraped
in a day. (rate limit is about 5000.)

Also might be scraping info about all the schools in Pittsburgh.

zipcodes.csv: list of all zip codes in Pittsburgh. Obtained from http://www.zip-codes.com/city/PA-PITTSBURGH.asp plus a Kimono instant-scrape. Then fed through `cut -c 11-15 < kimonoData.csv | tail -n +3 > zipcodes.csv`.

