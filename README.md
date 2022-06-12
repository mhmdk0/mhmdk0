# okicrawler
Python based Data Mining / Crawler for Okinawa Food &amp; Living App

1. Running Instructions
* Python 3.8 or Higher Version Required
* Running The Crawler Will Install All The Required Modules.
* Chec

2. Upgraded
* business_list.csv is The File That Contains Businesses' Categories.
* The Crawler Reads The Categories From business_list.csv file.
* It'll Scrape Data Based On The Caregory Name, Adding Some Flags to business_list.csv, and Creates a New CSV File 'places_errors.csv' For Error Checking.
* At The Very Beginning, Category's Status  Will Be -1 Which Means That It Have Never Been Scraped.
* If The Category Have Been Scraped With No Errors, The Status Will Be 1000, Else The Status Will Depend On The Error Type, And The Number Of Pages Scraped.
* If The Category Have No Data To Scrape, Or Failed Then The Status Will Be -1000.

3. Usage:

    python okicrawler.py option1 option2 optionX

    --without-images Scrapes The Data Without Images URLs.(Default is With Images)

    --without-reviews Scrapes The Data Without Reviews Content.(Default is With Reviews)

    --images-number Followed By X digit(s), To Scrape X Number(s) Of Images' URLs.(Default is 10)

    --reviews-number Followed By X digit(s), To Scrape X Number(s) Of Reviews' Content.(Default is 10)

    --max-tries Followed By X digit(s), Number of Tries If The Category/Place Raises an Error.(Default is 2)

    --headless Starts The Driver in Headless Mode.(Default is non-headless)

    --no-sandbox Fixes Issues When Running On Linux

    --help Views This Help Message.

    "To Scrape With Images, With Reviews, in non-headless Mode, get 10 Reviews and Images URLs, and 2 Maximum Tries; Don't pass any arguments."
