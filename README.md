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


### Example summary

#### ORIGINAL

Human activities are estimated to have caused approximately 1.0°C of global warming5 above pre-industrial levels, with a likely range of 0.8°C to 1.2°C. Global warming is likely to reach 1.5°C between 2030 and 2052 if it continues to increase at the current rate. (high confidence) (Figure SPM.1) Reflecting the long-term warming trend since pre-industrial times, observed global mean surface temperature (GMST) for the decade 2006–2015 was 0.87°C (likely between 0.75°C and 0.99°C)6 higher than the average over the 1850–1900 period (very high confidence). Estimated anthropogenic global warming matches the level of observed warming to within ±20% (likely range). Estimated anthropogenic global warming is currently increasing at 0.2°C (likely between 0.1°C and 0.3°C) per decade due to past and ongoing emissions (high confidence). Warming greater than the global annual average is being experienced in many land regions and seasons, including two to three times higher in the Arctic. Warming is generally higher over land than over the ocean. (high confidence)  Trends in intensity and frequency of some climate and weather extremes have been detected over time spans during which about 0.5°C of global warming occurred (medium confidence).

#### LSA Summary
Human activities are estimated to have caused approximately 1.0°C of global warming5 above pre-industrial levels, with a likely range of 0.8°C to 1.2°C. Reflecting the long-term warming trend since pre-industrial times, observed global mean surface temperature (GMST) for the decade 2006–2015 was 0.87°C (likely between 0.75°C and 0.99°C)6 higher than the average over the 1850–1900 period (very high confidence). Warming greater than the global annual average is being experienced in many land regions and seasons, including two to three times higher in the Arctic. Trends in intensity and frequency of some climate and weather extremes have been detected over time spans during which about 0.5°C of global warming occurred (medium confidence).

#### LexRank Summary
Human activities are estimated to have caused approximately 1.0°C of global warming5 above pre-industrial levels, with a likely range of 0.8°C to 1.2°C. Reflecting the long-term warming trend since pre-industrial times, observed global mean surface temperature (GMST) for the decade 2006–2015 was 0.87°C (likely between 0.75°C and 0.99°C)6 higher than the average over the 1850–1900 period (very high confidence). Warming greater than the global annual average is being experienced in many land regions and seasons, including two to three times higher in the Arctic. Trends in intensity and frequency of some climate and weather extremes have been detected over time spans during which about 0.5°C of global warming occurred (medium confidence). 

## Limitations

- The goal is to make the relevant facts as accessible as possible - this means not misrepresenting the report by making up facts. It does not mean creating a definitive summary that completely represents all required details. A summary means that we are losing details, and policy experts should verify what is required

- images, supplementary info will be collected in future iterations - current project is only focused on the paragraph content

## Schedule

1. Initial experiments, identify usable technologies and evaluation methods, identify input/output required at each step (data structure for JSON files - which features to include)
2. web scraping into JSON format
3. Reading difficulty of JSON assessed via functions- starting reading difficulty, word count, reading time (paragraph wise and total), Initial summarization 
4. Finalized summarization of text, insight generation (percent reduction of each)

## TO DO:
- Containerize / add requirements.txt
- Discussion of results