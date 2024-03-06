# Wep-Scraping
#Date_created

Project Overview

This Python project leverages web scraping and browser automation techniques to extract comprehensive product details for watches listed on the official Raymond Weil website ((https://ikepod.com/en/).

Core Functionality

Dynamic Loading: Employs Selenium to open the website, handle cookie consent interactions, and scroll the pages, triggering the loading of all product listings.
Initial Scraping: Parses the initial HTML source with BeautifulSoup to gather basic product information (title, product link).
Detailed Extraction: Utilizes requests to fetch individual product pages and BeautifulSoup to scrape in-depth specifications, descriptions, and other attributes.
CSV Export: Organizes collected data into a well-structured CSV file ("Ikepod1.csv").
Dependencies

requests
BeautifulSoup4
selenium
webdriver_manager (or a compatible WebDriver for your chosen browser)
csv
Instructions

Install Dependencies: pip install requests beautifulsoup4 selenium webdriver_manager csv

Download WebDriver: Ensure you have a WebDriver (e.g., ChromeDriver) installed and placed in your PATH or accessible to the script.

Run the Script:

python scraping_web.py

Data Structure (Ikepod1.csv)

The CSV file includes columns such as:

Reference Number
Product URL
Brand
Type
Year Introduced
Collection (Parent Model)
Specific Model
Nickname
Marketing Name
Style
Price
Image URL
Case Shape, Case Material, Bezel, Water Resistance, ...
Full Description
... (and more)
Potential Enhancements

Error Handling: Add more robust error handling (try-except blocks) to gracefully handle website changes or unexpected issues.
Efficiency: Explore if Raymond Weil provides an API that might offer a more direct way to get product data.
Data Analysis: Create separate scripts or notebooks to analyze the collected data (price trends, popular features, etc.)
Disclaimer

Please respect the Raymond Weil website's terms of service and avoid excessively frequent requests.
