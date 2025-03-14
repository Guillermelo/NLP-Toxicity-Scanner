# Toxicity Detector for Reddit

## Overview
This project is an AI-powered system that detects toxic language in Reddit comments and Discord messages. It leverages Natural Language Processing (NLP) to classify messages based on their toxicity levels, helping moderators maintain healthier online discussions.

## Features
- **Reddit Integration**: Fetches real-time comments using `PRAW`.
- **Text Preprocessing**: Cleans and prepares text for analysis using `NLTK`.
- **Toxicity Analysis**: Utilizes `Perspective API` or `Toxic-BERT` for classification.
- **Visualization & Reporting**: Generates toxicity distribution charts using `Matplotlib` and `Seaborn`.

## Installation
To set up the project, install the required dependencies:
```bash
pip install praw nltk transformers torch perspective-api-client matplotlib seaborn pandas
```

## Configuration
1. Create a `config.json` file with the following structure:
```json
{
    "REDDIT_CLIENT_ID": "your_client_id",
    "REDDIT_CLIENT_SECRET": "your_client_secret",
    "REDDIT_USER_AGENT": "your_user_agent"
}
```


## How It Works
1. **Data Extraction**: Retrieves comments/messages from Reddit or Discord.
2. **Preprocessing**: Cleans text by removing stopwords, punctuation, and unnecessary characters.
3. **Toxicity Analysis**: Classifies messages using an NLP model.
4. **Visualization**: Generates insights from the data.

