**SEC Annual Report Links (2005–2025)**
This repository contains a comprehensive collection of URLs linking to SEC annual reports (such as 10-K and 20-F filings) for publicly traded companies in the United States, covering the years 2005 through 2025. The links provide direct access to the official filings hosted by the SEC.

**Overview**
A large collection of annual report URLs for most U.S. publicly traded companies over the last two decades.

Includes links to various forms commonly used for annual reporting, including 10-K and 20-F.

Useful for researchers, analysts, or developers who want to download or reference original SEC filings directly.

Compiled using web scraping methods via sec edgar full text search

**Contents**
annual_links_2005_2025.json — JSON mapping of company tickers to lists of annual report URLs.

Optional helper scripts for accessing and working with these links.

**Usage Example**
Here is a simple Python snippet demonstrating how to load and use the links:

import json

with open('annual_links_2005_2025.json') as f:
    annual_links = json.load(f)

ticker = 'MSFT'
if ticker in annual_links:
    for url in annual_links[ticker]:
        print(url)
        
**Notes**
This collection focuses on providing access to original SEC filings via direct links.

While it covers most companies, some filings may be missing due to changes in SEC archives or filing availability.

The links point to official SEC resources but users should verify accessibility and download files responsibly.

**License**
This project is licensed under the MIT License. You’re free to use and share with attribution.
