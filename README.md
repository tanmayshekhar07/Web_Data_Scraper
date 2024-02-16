# Web_Data_Scraper
In this project I've build a web-scraper using beautiful soup and selenium in order to scrape data from uber-eats and create my own dataset for pizzas that are being ordered through Uber-eats.
# Project: Web Data Extractor using Python.

## Topic: UberEats page for Pizzas



Name: Tanmay Shekhar

Email: shekhar.t@northeastern.edu

### Project Overview:

The objective of this project is to scrape restaurant data more specifically Pizza places from UberEats and build a dataset out of it by storring it in a CSV (Comma-Separated Values) file. The data includes information about the restaurants, their ratings, total reviews, and estimated delivery times. Python is used along with libraries such as BeautifulSoup for web scraping and the csv module for handling CSV files.


This project aims to scrape all important data from the website and create a dataset by further getting into a selected topic and scrape all information pertaining to:
Name of the restaurant

Avg Rating of the restaurants

Number of reviews

Delivery-Time




### METHODOLOGY:

This project uses the following Python libraries:

Requests
: To send HTTP requests to the UberEats API
Selenium Webdrive
: To access website and navigate to topics
Beautiful Soup
: To parse the HTML responses from the GitHub API
Pandas
: To store and analyze the scraped data





### Tools:

So you can use either of the following Editors:

Jupyter notebook (What I have used)

Google Colab

Visual studio code

Atom

## Project Steps

### Selenium Setup:
Selenium is a powerful tool for browser automation that can interact with web pages just as a human would. It is particularly useful for scraping data from web pages that load content dynamically with JavaScript, which is not accessible with static requests made by libraries like requests.
The code imports necessary components from Selenium, such as webdriver for controlling the browser, Options for configuring browser options, and By for selecting elements.
Browser Configuration:

The Options class is used to create a browser configuration object, where various arguments are added to customize the browser behavior. These arguments include maximizing the window on start, disabling notifications, popup blocking, and more. This setup aims to optimize the browser for scraping tasks by reducing interruptions and mimicking a typical user environment.

### WebDriver Initialization:
A Chrome WebDriver is initialized with the specified options. This driver launches a Chrome browser instance, allowing Selenium to control it programmatically.
Page Retrieval and Rendering:

The WebDriver navigates to the specified url (the same UberEats search URL for pizza delivery in the Boston Common area as mentioned earlier).
The script then pauses execution for a specified TIMEOUT period to allow the web page to render fully. This delay is crucial for ensuring that dynamic content loaded by JavaScript is fully loaded before proceeding with data extraction.

### Data Collection:

A specific website is selected for web scraping. In this project, the website chosen is Uber Eats, and a search query for "Pizza" is used as an example.
Selenium is used to automate the process of opening a web page and retrieving its source code. Selenium allows us to interact with web pages programmatically.

### Web Page Rendering:

After navigating to the desired webpage, a timeout is added to allow the page to render fully.

This is essential to ensure that the web page content is loaded completely before scraping.

### HTML Parsing:

The page source code (HTML) is passed to BeautifulSoup, a Python library for parsing HTML and XML documents. BeautifulSoup makes it easier to navigate and extract data from HTML documents.

### Data Extraction:

To extract data, specific HTML elements are targeted. The example in the project focuses on extracting restaurant names, ratings, total reviews, and delivery times.
XPath or CSS selectors are used to locate the desired HTML elements. If certain elements have unique identifiers such as classes or tags, they are used to pinpoint the data.

### Data Validation and Handling:

To ensure data quality and consistency, the project includes validation and handling of missing or incomplete data. For example, if a restaurant name is missing, it is set to "N/A" to indicate that the data is not available.

### CSV File Creation:

A CSV file is created using Python's csv module. The csv.writer class is used to write the extracted data to the CSV file.
The data is organized into rows and columns in the CSV file.



## Project Conclusion:

The project concludes with a confirmation message indicating the successful creation of the CSV file.
The CSV file can be further analysed or used for various purposes, such as data analysis, reporting, or data visualisation


### References:

Professors Reference Notebook of Indeed: /Users/tanmayshekhar/Downloads/ADS_Matierial/M02/scrape_indeed_student.ipynb:
ChatGPT 3.5: for helping give boilerplate code for building the scraper and certain error solving
