### Extracting Text Data from URLs and Performing Text Analysis

This project aims to extract textual data articles from given URLs and perform text analysis to compute various variables as outlined in the project objectives.

#### Approach to the Solution:

1. **Data Extraction**: The Python script utilizes the `requests` library to fetch webpage content and `BeautifulSoup` for HTML parsing. It iterates through each URL provided in the input Excel file, extracts the article title and text, and saves them in text files.

2. **Text Analysis**: After extracting the article text, additional code needs to be added to compute the provided variables. Below are the steps to calculate each variable:

   1. **Positive Score** and **Negative Score**:
      - Create lists of positive and negative words.
      - Tokenize the article text into words.
      - Count occurrences of positive and negative words.
      - Calculate positive and negative scores.

   2. **Polarity Score**:
      - Compute the polarity score using the formula:
        ```
        Polarity Score = (Positive Score - Negative Score) / (Positive Score + Negative Score + 1)
        ```

   3. **Subjectivity Score**:
      - Determine the subjectivity score using sentiment analysis or lexicon-based approach.

   4. **Average Sentence Length**:
      - Tokenize the article text into sentences.
      - Calculate the average length of sentences.

   5. **Percentage of Complex Words**:
      - Define criteria for identifying complex words.
      - Calculate the percentage of complex words.

   6. **FOG Index**:
      - Compute the FOG index using the formula:
        ```
        FOG Index = 0.4 * (Average Sentence Length + Percentage of Complex Words)
        ```

   7. **Average Number of Words per Sentence**:
      - Calculate the average number of words per sentence.

   8. **Complex Word Count**:
      - Count the number of complex words.

   9. **Word Count**:
      - Calculate the total number of words.

   10. **Syllable per Word**:
       - Count the number of syllables in each word and calculate the average.

   11. **Personal Pronouns**:
       - Count the occurrences of personal pronouns.

   12. **Average Word Length**:
       - Calculate the average word length.

3. **How to Run the Python Script**:
   
   1. **Dependencies**:
      - Python 3.x
      - pandas
      - requests
      - BeautifulSoup

   2. **Setup**:
      - Ensure Python is installed on your system.
      - Install the required dependencies using pip:
        ```
        pip install pandas requests beautifulsoup4
        ```

   3. **Execution**:
      - Clone or download the repository containing the Python script (`Data_analytics.py`) and the input Excel file (`Input.xlsx`).
      - Open a terminal or command prompt and navigate to the directory containing the Python script and input Excel file.
      - Run the Python script using the following command:
        ```
        python Data_analytics.py
        ```
      - The script will extract article text from the provided URLs and save them as text files in the specified output directory.

#### Additional Notes:

- Make sure to replace the file paths in the Python script (`Data_analytics.py`) with the appropriate paths on your system.
- For performing text analysis and computing variables, additional code needs to be added to the Python script after extracting the article text.

#### Contributors:

- Abhishek Bodkhe
- abofficial777@gmail.com

Feel free to reach out for any questions or assistance!
