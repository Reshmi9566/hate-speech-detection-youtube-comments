# Hate Speech Detection in YouTube Comments on Lok Sabha Elections

This project aims to detect hate speech in multilingual YouTube comments related to the Lok Sabha elections. By leveraging pretrained models for labeling, the project provides a high-quality dataset and insights for future classification tasks. This repository contains the code for data collection, preprocessing, labeling, and initial model development.

---

## Table of Contents
1. [Project Overview](#project-overview)
2. [Data Collection](#data-collection)
3. [Data Preprocessing](#data-preprocessing)
4. [Labeling with Pretrained Models](#labeling-with-pretrained-models)
5. [Model Training](#model-training)
6. [Insights and Visualizations](#insights-and-visualizations)
7. [Future Work](#future-work)
8. [Installation and Usage](#installation-and-usage)
9. [Technologies Used](#technologies-used)
10. [Contributors](#contributors)

---

### Project Overview
This project focuses on building a reliable labeled dataset of YouTube comments for hate speech detection. The primary task is to label comments as *hate* or *non-hate* using pretrained models like **Detoxify** and **DistilBERT**. These labels form a foundation for ML models that can later be used for real-time hate speech detection in online content.

### Data Collection
Using the YouTube Data API, we scraped **23,989 comments** from election-related videos on news channels like Hindustan Times, India Today, and Aaj Tak. The dataset includes multilingual comments in languages like Hindi, Tamil, Malayalam, and Arabic.

### Data Preprocessing
- Removed duplicate comments and links to ensure data quality.
- Translated non-English comments into English using Google Translate for consistency in the labeling process.

### Labeling with Pretrained Models
- **Detoxify:** Labeled comments based on a set threshold to classify as *hate* or *non-hate*.
- **DistilBERT:** Further categorized comments into *offensive*, *hate*, and *non-hate* categories.

### Model Training
- Built and trained a logistic regression model for each labeled dataset.
- Used **Sentence-BERT embeddings** for vectorization, and tuned the models to improve classification accuracy.

### Insights and Visualizations
- Displayed insights from the labeled data using word clouds, bar charts, and bigram analysis.
- Generated visualizations to analyze comment sentiment, frequency of hate speech, and language trends.

### Future Work
- **Enhanced Labeling:** Integrate generative tools and adaptive thresholds for more context-aware labeling.
- **Dataset Expansion:** Scrape more comments for a broader dataset.
- **Model Improvement:** Experiment with ensemble models for better classification accuracy.


## Technologies Used
- **Python:** Programming language
- **YouTube Data API:** For data scraping
- **Google Translate API:** For translation
- **Detoxify and DistilBERT:** Pretrained models for labeling
- **Sentence-BERT:** For embedding creation
- **Matplotlib & Seaborn:** For data visualization

---

## Contributors
- [Reshmi C R](https://github.com/Reshmi9566) - Project Lead


