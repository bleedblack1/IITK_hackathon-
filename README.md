# IITK_hackathon-
Problem Statement by Overlayy Gen AI PS

# Website Scraper and Question Generator

This project provides a comprehensive solution for scraping website content, generating concise questions based on the scraped data, identifying relevant links, and evaluating the quality of generated questions and link relevance. The script is designed to help automate content analysis and question generation using the OpenAI GPT-3.5-turbo model.

## Features

- **Website Scraping**: Extracts all hyperlinks and their associated textual content from a given website.
- **Question Generation**: Automatically generates concise questions based on the content scraped from each webpage using OpenAI's GPT-3.5-turbo model.
- **Relevant Link Detection**: Identifies and ranks the most relevant links based on the similarity of the content.
- **Evaluation**: Includes basic evaluation functions to assess the relevance, clarity, conciseness, and coverage of the generated questions. Additionally, it evaluates the precision, recall, and F1-score of the relevance detection.

## Requirements

- Python 3.x
- `requests` library
- `BeautifulSoup` from the `bs4` library
- `openai` library
- `scikit-learn` library

Install the required Python packages with:

```bash
pip install requests beautifulsoup4 openai scikit-learn
```

## Usage

1. **Set up your OpenAI API key**: The script prompts you to enter your OpenAI API key at runtime.

2. **Run the script**: Execute the script and provide the URL of the website you wish to scrape. The script will automatically scrape the content, generate questions, and evaluate the results.

```bash
python script.py
```

3. **Output**: The generated questions, relevant links, and topics will be saved in an `output.json` file in the current directory. The script will also print the results and evaluations to the console.

## Example

Here's a basic example of how the script works:

- **Input**: A website URL (e.g., `https://example.com`).
- **Output**: A JSON file containing:
  - List of questions generated from each webpage.
  - Relevant links detected for each webpage.
  - Main topics extracted from each webpage's content.

## Evaluation

The script includes simple evaluation metrics for the generated questions and relevance detection. You can modify the evaluation logic as per your specific use case.

