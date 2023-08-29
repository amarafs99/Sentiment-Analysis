# Yelp Review Sentiment Analysis using BERT



[![Python Version](https://img.shields.io/badge/Python-3.x.x-blue)](https://www.python.org/downloads/)
[![Transformers Version](https://img.shields.io/badge/Transformers-4.11.3-brightgreen)](https://github.com/huggingface/transformers)
[![Torch Version](https://img.shields.io/badge/Torch-1.10.0-orange)](https://pytorch.org/get-started/locally/)
[![Requests Version](https://img.shields.io/badge/Requests-2.26.0-yellow)](https://pypi.org/project/requests/)
[![BeautifulSoup Version](https://img.shields.io/badge/BeautifulSoup-4.9.3-blueviolet)](https://pypi.org/project/beautifulsoup4/)
[![Pandas Version](https://img.shields.io/badge/Pandas-1.3.3-lightgrey)](https://pandas.pydata.org/getting_started.html)
[![Numpy Version](https://img.shields.io/badge/Numpy-1.21.5-red)](https://numpy.org/install/)
[![Matplotlib Version](https://img.shields.io/badge/Matplotlib-3.4.3-brightgreen)](https://matplotlib.org/stable/users/installing.html)

## Overview

This project demonstrates sentiment analysis on Yelp reviews using a pre-trained BERT-based model. It showcases the use of the Hugging Face Transformers library for natural language processing tasks.

## Getting Started

Follow these steps to run the sentiment analysis:

1. Install the required dependencies:
  
2. Copy and paste the code from [main.py](main.py) into your Python environment.

3. Run the script.



## Code Breakdown

1. Loading Pre-trained Model and Tokenizer:
The code begins by importing necessary libraries and loading a pre-trained BERT-based sentiment analysis model and tokenizer using the AutoTokenizer and AutoModelForSequenceClassification classes from the Transformers library.

2. Example Sentence and Sentiment Analysis:
The code tokenizes and decodes example sentences to ensure the tokenizer and decoding processes function correctly. It then performs sentiment analysis on one of the examples to showcase the model's sentiment scoring.

3. Web Scraping Yelp Reviews:
Using the requests library, the code makes a GET request to a Yelp page specified by its URL. It utilizes BeautifulSoup for parsing the HTML content and regex to find elements representing review comments.

4. Sentiment Analysis on Reviews:
A function named sentiment_score is defined to perform sentiment analysis on a given review. This function tokenizes the review, feeds it into the model, and calculates the predicted sentiment score.

5. Applying Sentiment Analysis to Reviews:
The sentiment analysis function is applied to each extracted review, and the results are stored in a DataFrame. Each review is associated with its sentiment score.

6. Creating a Sentiment Score Histogram:
The code generates a histogram using the matplotlib.pyplot library to visualize the distribution of sentiment scores in the Yelp reviews. The x-axis represents sentiment scores, and the y-axis represents the frequency of each score.



## Acknowledgments
This project utilizes the Hugging Face Transformers library, which provides access to pre-trained language models for various natural language processing tasks. The example code demonstrates the capabilities of these models for sentiment analysis on Yelp reviews.

Feel free to customize and extend this project for your own analysis and visualization needs.

## License
This project is licensed under the MIT License.

