# LogRhythm Chatbot Project Overview:
This project aims to create an interactive chatbot for LogRhythm SIEM 7.15 documentation, using a multi-step approach involving web scraping, data analysis, text classification, and natural language processing. The project is segmented into different scripts, each handling a specific part of the process.

## Scripts Overview:
1. **Web Scraping Script for Data Extraction:**
   - **Purpose:** To scrape and extract information from the LogRhythm SIEM 7.15 documentation.
   - **Libraries and Techniques:**
     - `requests` and `BeautifulSoup` for scraping web pages.
     - `pandas` for data manipulation and storing the scraped data.
     - `urlparse` and `RobotFileParser` for URL processing and respecting robots.txt.
     - `langdetect` for detecting the language of the content.
   - **Challenges:** Handling dynamic web content, adhering to website's scraping policies, and ensuring efficient and robust scraping against network issues.

2. **Exploratory Data Analysis on Textual Data:**
   - **Purpose:** To analyze and visualize the scraped textual data.
   - **Libraries and Techniques:**
     - `pandas`, `matplotlib`, `seaborn` for data analysis and visualization.
     - `nltk` and `TextBlob` for natural language processing tasks.
     - `WordCloud` for generating word clouds.
   - **Challenges:** Processing large volumes of text, identifying meaningful patterns, and interpreting the results accurately.

3. **Text Classification and Analysis using Word2Vec and RandomForest:**
   - **Purpose:** To classify text using Word2Vec for feature extraction and RandomForest for classification.
   - **Libraries and Techniques:**
     - `gensim` for Word2Vec model.
     - `nltk` for text tokenization.
     - `sklearn` for RandomForest classifier and model evaluation.
     - `imblearn` for handling class imbalance with SMOTE.
   - **Challenges:** Balancing the classes in the dataset, choosing appropriate features, and tuning the classifier for optimal performance.

4. **LogRhythm Chatbot for Document Query and Summarization:**
   - **Purpose:** To develop a chatbot that can categorize, analyze, and summarize textual data from documentation.
   - **Libraries and Techniques:**
     - `spacy` and `transformers` for NLP tasks and summarization.
     - `Word2Vec` and `TF-IDF` for text embedding.
     - Cosine similarity for finding relevant documents.
   - **Challenges:** Developing an accurate and responsive chatbot that can understand and summarize technical documentation effectively.

## Comprehensive Analysis:
- **Data Collection and Processing:** The first phase involves scraping the LogRhythm documentation, where challenges include adhering to ethical scraping practices and handling potential data inconsistencies. The subsequent data analysis phase employs statistical and NLP techniques to gain insights and prepare the data for further processing.
- **Feature Extraction and Machine Learning:** Utilizing Word2Vec and RandomForest, the project demonstrates an effective approach to classify text data. Balancing the dataset with SMOTE is crucial to deal with class imbalance, a common issue in text classification tasks.
- **Chatbot Development:** The final phase integrates various NLP techniques to create a chatbot. This involves using embeddings for text representation, leveraging both extractive (spaCy) and abstractive (Hugging Face Transformers) summarization techniques to generate concise and relevant responses.

![LogRhythm Chatbot Python Scripts and Key Processes](https://github.com/knapp069/Knapp069-Practicum-1-Project/blob/LogRhythm-Chatbot/Images/Python%20Programs%20Key%20Processes.png)

## Possible Future Enhancements:
1. **Improved Scraping Techniques:** Implement advanced web scraping techniques to handle dynamically loaded content or to scrape data from complex web pages.
2. **Advanced NLP Features:** Incorporate more sophisticated NLP features like named entity recognition, dependency parsing, or sentiment analysis to enrich the analysis.
3. **Enhanced Classification Algorithms:** Experiment with different or more advanced machine learning algorithms like Neural Networks or SVMs for text classification.
4. **Chatbot Improvements:** Integrate a more conversational and context-aware system in the chatbot using technologies like RASA or Google Dialogflow.
5. **User Feedback Loop:** Implement a mechanism to collect user feedback on chatbot responses to continuously improve its accuracy and relevance.
6. **UI/UX for Chatbot:** Develop a user-friendly interface for the chatbot to enhance user engagement and accessibility.

## Running the Programs:

To utilize the full functionality of the LogRhythm Chatbot, you need to run the Python scripts in the following order, depending on your specific needs:

1. **Web Scraping Script for Data Extraction:**
This will execute the script designed to scrape and extract information from LogRhythm SIEM 7.15 documentation. The output will be a CSV file containing the scraped data.

2. **Exploratory Data Analysis on Textual Data**
After extracting the data, run the EDA script to analyze and visualize the information. This will help you understand the data patterns and prepare it for the classification process.  It also includes cleaning, normalizing, and structuring the data before it can be fed into the machine learning models.

3. **Text Classification and Analysis using Word2Vec and RandomForest:**
Once the data is preprocessed, you can run the text classification script. It uses Word2Vec for feature extraction and RandomForest for the classification task.

4. **LogRhythm Chatbot for Document Query and Summarization:**
Finally, to start interacting with the chatbot, run the chatbot script. This program uses the trained models to categorize, analyze, and summarize the textual data from the documentation.

Please ensure all required libraries are installed and that you have the necessary permissions to scrape the website. Additionally, make sure to run these scripts in a suitable environment where Python and all dependencies are properly set up.

A sample of the scraped data from the Web Scraping Script for Data Extraction is available in the Data_Files folder named 'section_data.csv'.
A sample of the processed/cleaned data from the Exploratory Data Analysis on Textual Data script is available in the Data_Files folder named 'cleaned_section_data.csv'.

## Conclusion:
This project is a comprehensive application of data science and NLP in the context of a practical, real-world problem. It demonstrates the entire workflow from data collection to the deployment of a functional chatbot, encapsulating various aspects of data science and machine learning. The challenges faced highlight the complexities of working with real-world data and the necessity of employing robust methods to extract, process, and analyze data. Future enhancements can focus on increasing the sophistication and user-friendliness of the solutions, thereby making the chatbot more effective and versatile.
