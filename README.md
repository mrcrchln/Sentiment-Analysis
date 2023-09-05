# Google News Sentiment Analyzer
This project is a Python script that extracts news articles related to a specified company from Google News RSS feeds and analyzes their sentiment using the VADER sentiment analyzer from the NLTK library. It then creates a Pandas DataFrame with the article titles, their sentiment scores, publication dates, and URLs, exports a .csv, and visualizes the daily average sentiment score over time.

## Installation
To use this script, you will need to have Python and the required libraries installed on your system. You can install the necessary libraries using pip:
  ```
  pip install feedparser nltk beautifulsoup4 pandas matplotlib
  ```
Additionally, you need to download the VADER sentiment lexicon by running the following command:
  ```
  import nltk
  nltk.download('vader_lexicon')
  ```
## Usage
1. Clone this repository to your local machine or download the script directly.
2. Modify the company_name variable to specify the company you want to analyze. Replace "Aptiv" with the name of the desired company.
3. The script will fetch news articles related to the specified company from Google News and analyze their sentiment. It will then display the average sentiment score for the article titles and the number of titles analyzed.

## Notes
- The script uses the Google News RSS feed to fetch news articles related to the specified company. You can customize the RSS feed URL by modifying the rss_url variable if needed.

- The sentiment analysis is performed on the titles of the news articles using the VADER sentiment analyzer. The sentiment score ranges from -1 (negative sentiment) to 1 (positive sentiment).

- The script removes anchor tags from the description of each news article to extract the URL.

- The results are stored in a Pandas DataFrame as well as .csv for further analysis or visualization.

- You can adapt this script for different companies and use cases by changing the company_name variable and customizing the data processing and analysis as needed.

## Author
This project was created by Marc Reichlin.

## License
This project is licensed under the MIT License. See the LICENSE file for details.





