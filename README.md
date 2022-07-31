# MilsurpAuctionScraper

Configurable Tool to help estimate median price of a certain surplus firearm based on data gathered from completed auctions from Rock Island Auction company.

I'm starting to collect WWII-era and earlier Military Surplus rifles.  One of the major problems with this is answering the question "what is a good price?".  As this surplus is not currently being manufactured, prices are perpetually changing.

## Scraper - Minimum Function List
- [ ] URL Request Get Auction base webpage
- [ ] Generate Filter - C&R, Caliber = 30 CARBINE
- [ ] URL Request Filtered Webpage
- [ ] Scrape Filtered Page using BeautifulSoup - get Lot Number / Individual Webpage
- [ ] Create json object for single item lot.
      - Model
      - Manufacturer
      - Bore Condition
      - Rating
      - Serial Number
      - NPRF
      - Estimated Price Range
      - Price Realized (obfuscated png, read using OCR and convert to number)
      - Hammer Price

## Scraper - Next Steps
Config file:
- [ ] Auction Number
- [ ] Caliber Search
- [ ] Model Name


## Price Estimator - Minimum Function List
- [ ] Input fields: Model, caliber, Condition, Manufacturer
- [ ] Find matching json items
- [ ] Grab each price realized and hammer price
- [ ] Find High, Low, Median realized price
- [ ] Find High, Low, Median hammer price
- [ ] Print data to console

## Price Estimator - Next Steps
- [ ] When no Condition selected, give general median, and medians of each condition
- [ ] Identify lots that sold under median per condition, under estimated price and provide link
- [ ] GUI