**API and Web Data Scraping Project**

**Cryptocurrency Data Collection Using CoinGecko API and Web Scraping**


**Project Overview**


This project demonstrates data collection using two approaches:

- Retrieving structured data from an API

- Scraping tabular data from a web page

For the API component, cryptocurrency market data was retrieved from the CoinGecko public API.

For the web scraping component, tabular data was extracted from Wikipedia.

The project showcases the full data acquisition workflow, including API communication, JSON handling, HTML parsing, data cleaning, and exporting results to CSV format.


**API Data Retrieval**


**Objective**

To retrieve real-time cryptocurrency market data and structure it for analysis.


**Approach**


- Defined the CoinGecko /coins/markets endpoint.

- Passed query parameters to retrieve the top 20 cryptocurrencies by market capitalization.

- Sent a GET request using the requests library.

- Verified successful communication using HTTP status code 200.

- Converted the JSON response into a Pandas DataFrame.

- Selected and renamed relevant financial columns.

- Exported the cleaned dataset to output/api_crypto_data.csv.


**Challenges**

Selecting an api to use.

Identifying relevant fields from a large API response.



**Web Scraping**


**Objective**

To extract structured cryptocurrency-related tabular data from a public website.


**Approach**


- Inspected the webpage structure to identify HTML tables.

- Retrieved page content using requests.

- Added a User-Agent header to resolve HTTP 403 (Forbidden) error.

- Used pandas.read_html() to extract tabular data.

- Selected the relevant table and exported it to output/scraped_crypto_table.csv.
  

**Challenges**


- Selecting a webiste to scrap
- limited options of websites to scrap
- Encountered an HTTP 403 error due to automated request blocking.

Resolved the issue by adding appropriate request headers.


**Technologies Used**


    Python

    Google Colab

    requests

    pandas

    JSON handling

    HTTP protocol


**Project Structure**


API-&-WebScraping-Project/

│

├── Notebooks/

│     └── api-&-webscraping-project.ipynb

│

├── Raw_Results_Data/

│     ├── API_DATA.csv

│     └── SCRAPED_DATA.csv

│

└── README.md
