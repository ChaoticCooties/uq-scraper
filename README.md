## UQ Course Scraper
Scrapes UQ course profiles for course specific information.
Implemented caching to reduce load on UQ's servers.

## Quick setup
```bash
pip install -r requirements.txt
```

Installs BeautifulSoup4, requests-cache and etc. Then import it usign
```python
import uqscraper
```

## Quick usage guide
A UQScraper object must first be initialized with the course code string for example:
```python
scraper = UQScraper("COMP3320")
```

Then you can use the provided get() functions to scrape what you need.
```python
title = scraper.get_title()
print(title)
```

Returns the title.
