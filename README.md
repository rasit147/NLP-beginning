Sentiment Analysis and Text Mining on Web Articles


This repository contains a Python-based project for extracting and analyzing text data from web articles. The primary goal is to perform sentiment analysis by computing various scores, such as positive and negative word counts, polarity, and subjectivity scores, based on the content of the articles.

Project Overview
This project is structured to achieve the following objectives:

Text Extraction: Extract text data from web articles based on URLs provided in an Excel file (Input.xlsx).
Sentiment Analysis: Perform sentiment analysis on the extracted text using predefined positive and negative word lists.
Score Computation: Calculate several metrics, including word count, positive and negative scores, polarity, and subjectivity.
Features
URL-Based Text Extraction: The script reads URLs from an Excel file and extracts the article title and content using BeautifulSoup.
Sentiment Analysis: Utilizes predefined word lists (positive-words.txt and negative-words.txt) to compute sentiment scores.
Polarity and Subjectivity: Calculates polarity and subjectivity scores to gauge the overall sentiment of the articles.
Modular Design: The project is designed with modular functions, making it easy to extend and modify.
Project Structure
Input Files:

Input.xlsx: Contains URLs for the articles to be analyzed, with columns like URL_ID and URL.
positive-words.txt: A text file listing positive words for sentiment analysis.
negative-words.txt: A text file listing negative words for sentiment analysis.
Output Files:

Output_Data_Structure.xlsx: (Optional) An Excel file for storing analysis results.
Text Files:

A series of .txt files named after the URL_ID (e.g., bctech2011.txt, bctech2012.txt, etc.) containing the extracted content from each article.
Code Files:

analysis_script.py: The main Python script containing the logic for text extraction, sentiment analysis, and score computation.
Untitled1.ipynb: A Jupyter notebook used during development for testing and validation.
How to Run the Project
Install Dependencies:
Ensure you have the necessary Python libraries installed:

bash
Copy code
pip install pandas requests beautifulsoup4 textblob nltk openpyxl
Prepare Input Data:
Place the URLs you wish to analyze in the Input.xlsx file. Ensure that the columns URL_ID and URL are correctly filled.

Run the Script:
Execute the script to perform text extraction and analysis:

bash
Copy code
python analysis_script.py
View Results:
The results will be saved in the text files corresponding to each URL_ID. If specified, you can save the results in Output_Data_Structure.xlsx.

Example Output
For an example article (bctech2011.txt), the sentiment analysis might yield the following insights:

json
Copy code
{
    "word_count": 994,
    "positive_score": 34,
    "negative_score": 8,
    "polarity_score": 0.619,
    "subjectivity_score": 0.042
}
These metrics help in understanding the overall sentiment and content of the analyzed article.

Contributing
Contributions are welcome! If you find a bug or have a feature request, please create an issue or submit a pull request.
nltk"Conducting Sentiment Analysis and Text Mining on Web Articles"
