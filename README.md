# 20th Century Text Mining Project

This repository contains a Python-based text mining project focused on analyzing key events of the twentieth century using data scraped from Wikipedia.

The project demonstrates an end-to-end workflow including data collection, text preprocessing, linguistic analysis, geographic analysis, and sentiment analysis.

---

## Project Overview

The project is organized into two main stages:

### 1. Data Collection
Textual data related to key events of the twentieth century is scraped from Wikipedia and stored as a plain text file. This data serves as the foundation for further analysis.

### 2. Text Mining and Analysis
The scraped text is processed and analyzed to extract meaningful patterns related to language structure, country mentions, and overall sentiment.

---

## Data Collection

### Description
A Jupyter notebook is used to scrape the Wikipedia page **“Key events of the 20th century”** using Selenium.  
The extracted content is saved as a text file for downstream analysis.

### Files
- `20th_century_scrape.ipynb` — web scraping notebook  
- `key_events_20th_century.txt` — scraped text content  

---

## Text Mining and Analysis

### Description
The main analysis notebook applies several natural language processing techniques, including:

- text cleaning and tokenization  
- word frequency analysis  
- part-of-speech (POS) tagging  
- country mention analysis using a lookup list and regular expressions  
- sentiment analysis using sentence-level polarity and subjectivity scores  

The results are visualized to support interpretation of linguistic structure, geographic focus, and overall sentiment.

### Files
- `text_mining/exercise_1_5_text_mining_20th_century.ipynb` — text mining and analysis notebook  
- `text_mining/countries_lookup.csv` — list of country names used for matching  
- `text_mining/country_mentions.csv` — frequency of country mentions  
- `text_mining/key_events_20th_century.txt` — input text used for analysis  

---

## How to Run

1. Open the notebooks in JupyterLab  
2. Ensure required libraries are installed  
3. Run the notebook cells from top to bottom  

---

## Notes

- Sentiment analysis is based on lexical methods and reflects overall tone rather than historical importance.
- Historical country aliases (e.g., *USSR*, *West Germany*) are included to better represent twentieth-century geopolitical context.

