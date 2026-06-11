# Travel-App-Reviews-LDA-Topic-Modelling
LDA topic modelling + sentiment analysis of Google Play Store travel-app reviews (scraping, text preprocessing, DTM, pyLDAvis)
Travel App Reviews — LDA Topic Modelling & Sentiment Analysis

A machine learning project that analyzes Google Play Store reviews of travel apps to discover hidden themes using Latent Dirichlet Allocation (LDA) topic modelling, supported by sentiment analysis.

Overview

The project takes thousands of real user reviews and answers a business question: what are people actually talking about, and how do they feel about it? It runs end-to-end from data collection to interpretable, labelled topics.

Pipeline


Data Collection – Large-scale scraping of travel-app reviews from the Google Play Store using the google-play-scraper library.
Data Loading & Exploration – Reloads the dataset with defensive parsing logic and reviews its structure.
Text Preprocessing – Cleans and standardizes raw review text (lowercasing, removing noise, tokenization, stopword removal).
Document-Term Matrix (DTM) – Built using scikit-learn's vectorizers.
Optimal Topic Selection – Searches for the best number of topics, K, before fitting the final model.
Final LDA Model – Trains the model with K = 6 topics.
Topic Visualization – Uses beta distributions, word frequencies, and interactive visualizations to communicate findings.
Topic Assignment & Labelling – Maps each review to a dominant topic and assigns human-readable labels for business insight.


Tech Stack


Python
google-play-scraper – data collection
pandas, numpy – data handling
scikit-learn – Document-Term Matrix, LDA model
matplotlib, pyLDAvis – visualization
NLP preprocessing libraries


How to Run

bashpip install google-play-scraper pandas numpy scikit-learn matplotlib pyLDAvis nltk

Open ML_Final_Project.ipynb in Jupyter Notebook or Google Colab and run the cells in order.

Output Files

FileDescriptionfig1_word_frequency.pngTop 20 most frequent terms in the corpusLDA topic chartsBeta distribution and per-topic top wordsTopic-labelled datasetEach review tagged with its dominant topic

Key Learnings


Unsupervised learning with LDA for theme discovery
Choosing the optimal number of topics for an LDA model
Turning abstract topics into actionable business insights
