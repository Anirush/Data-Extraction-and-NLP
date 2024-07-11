# Data-Extraction-and-NLP



Code description:

Setup and Data Loading: The script begins by downloading necessary NLTK data and loading positive and negative words from specified text files. It also initializes the CMU Pronouncing Dictionary for syllable counting.
Article Extraction: The script reads URLs from an input Excel file and fetches the content of these web pages using the requests library. It extracts the article's title and body using BeautifulSoup and saves the combined text to a local directory.
Text Processing and Metrics Calculation: For each saved article, the script tokenizes the text into words and sentences. It calculates several metrics like positive/negative scores, polarity, subjectivity, average sentence length, percentage of complex words, Fog Index, and more. These metrics are derived from the word and sentence counts, syllable counts, and predefined lists of positive and negative words.
Results Compilation: The computed metrics for each article are stored in a list of dictionaries. Each dictionary holds the metrics for a single article, identified by the URL ID.
Output: Finally, the script converts the list of dictionaries into a pandas DataFrame and saves it to an Excel file named 'Output_Data_Structure.xlsx'. This file contains all the calculated metrics for each article, structured for easy analysis and review.

How to Run the code:
 Install the required libraries by using the command – “pip install nltk textblob pandas requests beautifulsoup4”.
Give path for input data, positive wordslist, negative word list
Run the code for output
