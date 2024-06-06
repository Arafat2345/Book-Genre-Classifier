# Book-Genre-Classifier
A text classification model from data collection, model training, and deployment.
The model can classify 141 different types of book genres
The keys of deployment\genre_types_encoded.json shows the book genres

# Data Collection
Data was collected from a Goodreads Website Listing: https://www.goodreads.com/list/show/264.Books_That_Everyone_Should_Read_At_Least_Once
The data collection process is divided into 2 steps:

1. Book URL Scraping: The book urls were scraped with scraper\book_url_scraper.py and the urls are stored along with book title in scraper\book_urls.csv
2. Book Details Scraping: Using the urls, book description and genres are scraped with scraper\book_details_scraper.py and they are stored in data\book_detils.csv

