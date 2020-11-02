# NLP Project - Text Summarization of IPCC Report

## Motivation 

Climate change reporting suffers from a number of communication disadvantages. Specifically, the process of reading climate change reports suffers from a high level of complexity and jargon. 

This project aims to make the IPCC summary more readable with the following objectives (one or more can be accomplished):

- Reduce the average reading difficulty (Fliesh Kincaid or other)
- Reduce the length of the report via text summarization (Spacy NLP packages)
- Reduce the reading time using standard word calculations (ex: assuming a reading pace of 241 words per minute, new reading time is ... )

## Functions to develop

- assess_difficulty(), word_count(), reading_time() for a given string
- assess_JSON() - input json with text, output new JSON with numbers and values
- summarize_para() for a given string, return the summarized string
- summarize_report - for a giv

## Limitations

- The goal is to make the relevant facts as accessible as possible - this means not misrepresenting the report by making up facts. It does not mean creating a definitive summary that completely represents all required details. A summary means that we are losing details, and policy experts should verify what is required

- images will be collected in future iterations 

## Schedule

Week 1: initial experiments, identify usable technologies and evaluation methods, identify input/output required at each step (data structure for JSON files - which features to include)
Week 2: web scraping into JSON format
Week 3: Reading difficulty of JSON assessed via functions- starting reading difficulty, word count, reading time (paragraph wise and total), Initial summarization 
Week 4: finalized summarization of text, insight generation (percent reduction of each)