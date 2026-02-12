# 20th Century Text Mining Project

This repository contains a Python-based text mining project focused on analyzing key events of the twentieth century using data scraped from Wikipedia.
The project demonstrates an end-to-end workflow including data collection, text preprocessing, linguistic analysis, geographic analysis, and sentiment analysis.

## Project Overview

The project is organized into three main stages:

### 1. Data Collection
Textual data related to key events of the twentieth century is scraped from Wikipedia and stored as a plain text file. 
* **Files:** * `20th_century_scrape.ipynb` — web scraping notebook
    * `key_events_20th_century.txt` — scraped text content

### 2. Text Mining and Analysis
The scraped text is processed and analyzed to extract meaningful patterns related to language structure, country mentions, and overall sentiment.
* **Files:** * `text_mining/20th_century_text_mining_analysis.ipynb` — original analysis notebook
    * `text_mining/countries_lookup.csv` — list of country names used for matching

### 3. Geopolitical Relationship Mining (New)
The project now includes advanced analysis of how countries are mentioned together to identify historical relationships and clusters.
* **Files:**
    * `Geopolitical-Relationship-Mining-20th-Century.ipynb` — relationship mining notebook
    * `country_relationships_20th_century.csv` — frequency of mentions between country pairs
    * `cleaned_text_20th_century.txt` — input text used for this analysis

## How to Run (Virtual Environment)

This project uses a `venv` to manage dependencies.
1. **Activate the environment:**
   * Mac/Linux: `source venv/bin/activate`
   * Windows: `.\venv\Scripts\activate`
2. **Open the notebooks** in JupyterLab and run the cells from top to bottom.

## Notes
* Sentiment analysis is based on lexical methods and reflects overall tone rather than historical importance.
* Historical country aliases (e.g., USSR, West Germany) are included to better represent twentieth-century geopolitical context.