# Organizing Medical Transcriptions with the OpenAI API

This project is part of Datacamp's Associate AI Enginner for Developer's course. It aims to extract structured patient details from medical transcriptions and map recommended treatments to ICD-10 / ICD-10-PCS codes using the OpenAI API.

## Files
- [notebook.ipynb](notebook.ipynb) — main analysis notebook (contains the actual code).
- [data/transcriptions.csv](data/transcriptions.csv) — dataset of anonymized medical transcriptions.

## Quick overview
- The notebook loads [data/transcriptions.csv](data/transcriptions.csv) into a pandas DataFrame (`df`) and calls the OpenAI chat completion API to:
  1. Extract patient age and recommended treatment from medical transcripts.
  2. Map the recommended treatment to an ICD-10 or ICD-10-PCS code.
  3. NOTE: We use the openAI API and specifically the function calling ability to extract details and consequently map the ICD code.
- Results are combined into a single final dataframe.

## Requirements
- Python 3.8+
- pip packages: pandas, openai 
- An OpenAI API key set in the environment.

Install example
```bash
pip install pandas openai