# mf-nav-data
Historical NAV (price) data of mutual funds and popular benchmark indices in India 

## Context
### Real-life application of library
I built and operated a mutual fund investing platform as an AMFI licensed mutual fund distributor for a year. I used this data to analyse and visualise mutual funds.

### Open source in fintech?!
The finance industry wants exclusive access to data to be a barrier for entry of competition. I believe that, on the contrary, data should be universally accessible and differentiation in product or distribution could be the barriers. This is why I am open-sourcing all the data I collected.

## Data source
I have obtained this data by aggregating data from multiple sources, collected by crawling websites and having access to transaction portals as an AMFI licensed mutual fund distributor.

## Data stats
* ~45 MB of compressed data 
### `mf_nav`: Daily NAV data of mutual funds
* for 45 MF companies incl a few that have since then been closed down
* for all funds of each company
* for all schemes (growth/dividend/bonus, direct/regular etc) of each fund
* since start of each scheme
* till 2016 (Feb for some funds, Jun for others)

### `index_values`: Daily closing value of benchmark indices
* for 13 most popular stock indices like BSE Sensex, NSE Nifty etc and SBI FD
* since start of each index
* till Apr 2016

## Play with data
I used mongoDB to store all this time series data. My [other github repo](https://github.com/utkarshohm/mf-models) talks more about it.

## Related repos
* [Library to build a mutual fund transaction platform using the Bombay Stock Exchange StarMF platform and API](https://github.com/utkarshohm/mf-platform-bse)
* [Historical NAV/price/time-series data of mutual funds and popular benchmark indices in India](https://github.com/utkarshohm/mf-nav-data)

## Need help setting this up or want to contribute?
Feel free to raise an issue and I will get back asap
