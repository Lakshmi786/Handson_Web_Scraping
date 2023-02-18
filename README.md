# Handson_Web_Scraping
## Introduction 
The code in this notebook provides an example of how web scraping can be done using Python. It shows how a webpage can be scraped to extract tables using BeautifulSoup, how to extract relevant information from the tables, and how to clean and organize the data using pandas.

## Motivation
Web scraping is an essential tool that allows us to extract data from websites that are not readily available in a structured format. This data can be used for various purposes such as market research, trend analysis, and competitor analysis. In this notebook, we demonstrate how web scraping can be used to extract sex-ratio data from a webpage and clean it to retrieve ISO country codes from a GitHub repository.

## Requirements
The code requires the following Python libraries:

pandas
urllib3
bs4

## Usage
run the following functions:

## get_webpage_tables(url: str) -> List[BeautifulSoup]: 
This function takes the URL of the webpage to download and returns a list of BeautifulSoup objects, one for each table on the webpage.

## process_num(num: str): 
This function processes a string representing a number to a float.

## is_valid_cell(cells: List[BeautifulSoup]) -> bool: 
This function determines if a list of BeautifulSoup objects representing table cells is valid.

## make_str_valid(s: str) -> str: 
This function makes a string valid by removing any text in parentheses.

## extract_country_sex_ratio(tables: List[BeautifulSoup]) -> pd.DataFrame: 
This function extracts country sex ratios from a list of BeautifulSoup tables.

## get_country_codes(df) -> pd.DataFrame: 
This function retrieves ISO country codes from a GitHub repository and returns a cleaned DataFrame.

## Example
Here is an example of how the code can be used to extract sex-ratio data from a webpage:

This code will download the webpage from the given URL, extract all the tables using BeautifulSoup, extract the country sex ratios from the tables, and clean the data to retrieve ISO country codes from a GitHub repository. The resulting DataFrame will contain the extracted data.

## License
The code in this notebook is released under the MIT License. See the LICENSE file for details.
