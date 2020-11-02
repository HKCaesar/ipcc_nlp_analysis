# NLP Project - Text Summarization of IPCC Report

## Motivation 

Climate change reporting suffers from a number of communication disadvantages. Specifically, the process of reading climate change reports suffers from a high level of complexity and jargon. 

This project aims to make the IPCC summary more readable with the following objectives (one or more can be accomplished):

- Reduce the average reading difficulty (Flesch Kincaid or other)
- Reduce the length of the report via text summarization (Spacy NLP packages)
- Reduce the reading time using standard word calculations (ex: assuming a reading pace of 250 words per minute, new reading time is ... )

## Results

![results](img/results.png)

![baseline comparison](img/baseline.png)

## Limitations

- The goal is to make the relevant facts as accessible as possible - this means not misrepresenting the report by making up facts. It does not mean creating a definitive summary that completely represents all required details. A summary means that we are losing details, and policy experts should verify what is required

- images, supplementary info will be collected in future iterations - current project is only focused on the paragraph content

## Schedule

1. Initial experiments, identify usable technologies and evaluation methods, identify input/output required at each step (data structure for JSON files - which features to include)
2. web scraping into JSON format
3. Reading difficulty of JSON assessed via functions- starting reading difficulty, word count, reading time (paragraph wise and total), Initial summarization 
4. Finalized summarization of text, insight generation (percent reduction of each)

## TO DO:
- export full text (raw, summaries x2)
- Clean code 
- Docstrings
- Containerize / add requirements.txt