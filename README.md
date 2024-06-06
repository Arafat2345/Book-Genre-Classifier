# Book-Genre-Classifier
A text classification model from data collection, model training, and deployment.
The model can classify 141 different types of book genres
The keys of deployment\genre_types_encoded.json shows the book genres

# Data Collection
Data was collected from a Goodreads Website Listing: https://www.goodreads.com/list/show/264.Books_That_Everyone_Should_Read_At_Least_Once
The data collection process is divided into 2 steps:

1. Book URL Scraping: The book urls were scraped with scraper\book_url_scraper.py and the urls are stored along with book title in scraper\book_urls.csv
2. Book Details Scraping: Using the urls, book description and genres are scraped with scraper\book_details_scraper.py and they are stored in data\book_detils.csv
In total, I scraped 6,313 book details.

# Data Preprocessing
Initially there were 640 different genres in the dataset. After some analysis, I found out 499 of them are rare (probably custom genres by users). So, I removed those genres and then I have 141 genres. After that, I removed the description without any genres resulting in 6,104 samples.

# Model Training
Finetuned a distilrobera-base model from HuggingFace Transformers using Fastai and Blurr. The model training notebook can be viewed here

