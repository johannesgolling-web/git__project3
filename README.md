# Build Your Own Custom Chatbot – Fashion Trend Assistant

This project was completed as part of the Udacity Data Scientist II for Porsche Nanodegree program.  
It demonstrates how to build a lightweight custom chatbot using the OpenAI API and a domain-specific dataset (without external frameworks).
The goal is to show how Retrieval-Augmented Generation (RAG) works.


## Project Overview

The chatbot uses the dataset **2023 Fashion Trends**, which contains short text snippets describing the fashion trends and style directions for the year 2023.  
Using this data, the chatbot can answer focused questions about different topics like sustainability or materials and silhouettes that defined the year.

The workflow consists of four parts:
1. Dataset Preparation*
   Load and clean the CSV file so that all text snippets are stored in a single column called `text`.

2. Custom Query Process
   Create a simple retrieval pipeline using TF-IDF and cosine similarity in embedded vectors to select the most relevant snippets for each query.

3. Prompt Engineering
   Combine the retrieved snippets with the user’s question to build a custom prompt for the OpenAI Completion model.

4. Performance Measuring
   Compare answers with and without the custom context to show how the dataset improves relevance and accuracy.



## Repository Structure

- `notebooks/project3_custom_chatbot.ipynb`  
  The main notebook with all analysis and implementation steps.

- `data/raw/2023_fashion_trends.csv`  
  Original dataset with 82 text snippets about 2023 fashion trends.

- `README.md`  
  Project description and overview.


