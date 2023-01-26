# Real Estate Scraper

This application uses the BeautifulSoup library and pandas library to scrape information from a real estate listing on the website "sahibinden.com". The information is then stored in a dictionary and converted into a dataframe using pandas. The dataframe is then written to an excel file using pandas' ExcelWriter class.

## Usage

The script requires BeautifulSoup, pandas, requests and numpy library.

The main function ```get_sahibinden_record(html)``` takes the HTML content of a listing page as an input and returns a dataframe containing information about the property such as the title, price, square meter price, location, and other details.

The function ```ConvertStringToList(string)``` takes a string as an input and returns a list of words in the string.


The function ```get_sahibinden_link(html)``` takes the HTML content of a listing page as an input and returns the link to the listing page.

The code also checks if the scraped data corresponds to a "Araç" or "Arazi" and writes the dataframe to the respective sheet in the excel file.

### Note

It is important to note that this code is only an example and might not work properly without proper modification, as the website's structure might have changed or the listing is removed.
