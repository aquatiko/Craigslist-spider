# Craiglist-spider
A python spider to scrape jobs list and their details form craiglist.

## Usage

In Terminal or CMD, navigate to the main Scrapy project folder, and run the spider:

```scrapy crawl jobs -o output.csv```

### Settings
In settings.py change these parts to make spider site friendly-

```Set CONCURRENT REQUESTS= 2 (or 5),  to set maximum concurrent requests made by spider to domain. A high limit might be detected by domain.```

```ROBOTSTXT_OBEY= False   ,to be able to scrape parts of website that itn't allowed by domain. You can check those rulse by visiting www.site_name/robots.txt```

```DOWNLOAD_DELAY=2 (in seconds), to allow a gap in time period between concurrent requests. This will make your spider slow but also lessens the chance of detected by domain.```

You can also uncomment other settings in settings.py and set their values for a more customized spider.
