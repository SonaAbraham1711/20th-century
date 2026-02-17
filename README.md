# 20th Century Geopolitical Text & Network Mining

This repository contains a Python-based analysis of 20th-century history. By combining **Natural Language Processing (NLP)** and **Network Science**, the project uncovers hidden structures of global diplomacy and conflict based on historical data scraped from Wikipedia.

## 🚀 Project Overview

The project is structured into four distinct stages:

### 1. Data Collection
Textual data related to key events of the twentieth century is scraped from Wikipedia and stored as a plain text file.
* **Files:** `20th_century_scrape.ipynb`, `key_events_20th_century.txt`

### 2. Text Mining & Analysis
The scraped text is processed to extract patterns related to language structure, country mentions, and overall sentiment.
* **Files:** `text_mining/20th_century_text_mining_analysis.ipynb`, `text_mining/countries_lookup.csv`

### 3. Geopolitical Relationship Mining
Analysis of how countries are mentioned together to identify historical co-occurrence and build a relationship dataset.
* **Files:** `Geopolitical-Relationship-Mining-20th-Century.ipynb`, `country_relationships_20th_century.csv`, `cleaned_text_20th_century.txt`

### 4. Interactive Network Analysis (Final Submission)
The latest phase utilizes **Graph Theory** to visualize and analyze the 20th-century geopolitical landscape.
* **Community Detection:** Implementation of the **Leiden Algorithm** to identify historical "blocs" (e.g., Eastern Bloc vs. Western Alliance).
* **Interactive Visualization:** Dynamic, browser-based maps built with **Pyvis**.
* **Centrality Metrics:** Analysis of Degree, Closeness, and Betweenness centrality to identify "bridge" nations.
* **Files:** `Geopolitical_Bridges_and_Blocs_20th_Century.ipynb`, `historical_blocs_leiden.html`

## 📊 Key Observations

* **Historical Partitions:** The Leiden algorithm successfully identified the "Iron Curtain," grouping the USSR and its allies into a distinct community, while NATO-aligned nations formed another.
* **The "Bridge" Role:** Centrality analysis highlights countries like **France** and **Germany** as high-betweenness nodes, meaning they acted as vital diplomatic brokers between different global communities.
* **Network Density:** The visualization reveals the high connectivity of the 20th century, showing how localized conflicts were often linked to global superpower dynamics.

## 🛠️ How to Run (Virtual Environment)

This project uses a `venv` to manage dependencies (including `networkx`, `pyvis`, `cdlib`, and `leidenalg`).

1. **Activate the environment:**
   - **Mac/Linux:** `source venv/bin/activate`
   - **Windows:** `.\venv\Scripts\activate`
2. **Explore the Notebooks:** Open JupyterLab and run the cells from top to bottom.
3. **View Interactive Maps:** Open the `.html` files (like `historical_blocs_leiden.html`) directly in any web browser.

## 📝 Notes

* **Sentiment Analysis:** Based on lexical methods; it reflects the tone of the source text rather than historical importance.
* **Geopolitical Context:** Includes historical country aliases (e.g., USSR, West Germany) to ensure accurate mapping of 20th-century events.
