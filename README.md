# Decoding Sentiments in NFT Social Media Discourse: Leveraging Large Language Models for Human Sentiment Analysis

## General information
- **Author**: Yutong Quan, Political Economy (Economics), Class of 2024, Duke Kunshan University
- **Signature Work Mentor**: Prof. Luyao Zhang, Duke Kunshan University
- **Disclaimer**: Submissions to the Duke Kunshan University Signature Work Project.
- **Acknowledgments**: First, I would like to express my deepest gratitude to Prof. Luyao Zhang for her invaluable guidance and inspiration throughout my undergraduate journey. Her insightful teachings in ECON 211 and STATS 201 have been fundamental in shaping my research career. I am also immensely thankful for the support provided by the DKU Summer Research Scholars program, which played a pivotal role in the inception of my research idea. My heartfelt thanks go out to all my classmates and friends for their invaluable support and constructive feedback on this project.

## Project Summary
- **Background & Motivation**:
In Spring 2023, I had the privilege of co-authoring a research paper titled "On the Mechanics of NFT Valuation: AI Ethics and Social Media" with Prof. Luyao Zhang, Prof. Xin Tong, and fellow DKU students. This study explored the impact of sentiment, gender, and skin tone on NFT valuations using social media, blockchain, and cryptocurrency exchange data. We primarily utilized lexicon and rules-based sentiment analysis tools, like VADER (Valence Aware Dictionary and sEntiment Reasoner), for analyzing social media content. The advent of advanced sentiment analysis tools such as ChatGPT and LlaMA has spurred my interest in furthering this research. This project seeks to build upon our previous methodologies, focusing on the application of AI large language models for sentiment analysis on the same dataset of CryptoPunks-related Twitter discussions, and to compare the efficacy of these advanced models against traditional NLP tools.
- **Research Questions**:
  -  What are the sentiment analysis results of CryptoPunks-related tweets performed by large language models?
  -  What are the similarities and differences between the sentiment analysis results performed by large language models (LlaMA2) and those of traditional NLP tools (VADER)?
- **Methodology**:
  - Utilizing the Snscrape API to gather tweets featuring the #cryptopunk hashtag.
  - Conducting sentiment analysis on the collected data using the LlaMA2 model.
  - Assessing and comparing the performance of LlaMA2 and VADER in sentiment analysis.
- **Expected Results**:
  - LLMs can be applied to conduct sentiment analysis for NFT-related social media content.
  - LLMs have superior performance compared to traditional NLP tools in analyzing sentiment in social media texts.
- **Intellectual Merit & Practical Impacts**: 
This project represents a step forward in applying advanced AI technologies, specifically large language model sentiment analysis, to the realms of social media and blockchain-based crypto assets. By integrating AI models with NFT discourse analysis, we aim to enhance the precision of sentiment analysis and contribute to the development of specialized sentiment analysis tools for the crypto asset domain. Improved sentiment analysis tools can more accurately reflect market sentiment towards crypto assets, offering valuable insights to stakeholders. Moreover, the data collected and analyzed in this research could be instrumental in improving NFT price-prediction models.

## Table of Contents
- [Data](https://github.com/yutongquan/llm-cryptopunk/tree/main?tab=readme-ov-file#data)
- [Code](https://github.com/yutongquan/llm-cryptopunk/tree/main?tab=readme-ov-file#code)
- [Images](https://github.com/yutongquan/llm-cryptopunk/tree/main?tab=readme-ov-file#images)
- [Reference](https://github.com/yutongquan/llm-cryptopunk/tree/main?tab=readme-ov-file#reference)

## Data

### Collected Data
- **Data Dictionary**

| **Variable Name**	| **Unit**	| **Data Type**	| **Description** |
|---|---|---|---|
|Date|day|int64|The timestamp indicates when each tweet was posted, providing a temporal dimension to the dataset.|
|Text|text|int64|The textual content of the tweet discussions with the #cryptopunk hashtag.|

### Analyzed Data
- **Data Dictionary**

| **Variable Name**	| **Unit**	| **Data Type**	| **Description** |
|---|---|---|---|
|Date|day|int64|The timestamp indicates when each tweet was posted, providing a temporal dimension to the dataset.|
|Text|text|int64|The textual content of the tweet discussions with the #cryptopunk hashtag.|
|Sentiment|/|int64|The sentiment (positive/negative/neutral) of each tweet related to CryptoPunks.|

## Code

| **Content** | **URL** |
|---|---|
|Sentiment analysis using large language model (LlaMa2) |https://github.com/yutongquan/llm-cryptopunk/blob/main/code/LlaMa2_CryptoPunks.ipynb|
|Sentiment analysis using traditional NLP tool (VADER) |https://github.com/yutongquan/llm-cryptopunk/blob/main/code/VADER_CryptoPunks.ipynb|

## Images

**Fig.1: LlaMa2 Sentiment of CryptoPunks-related Tweets (first 200 tweets)**
![fig.1](https://github.com/yutongquan/llm-cryptopunk/blob/main/image/llama2-sentiment-graph.png)

**Fig.2: LlaMa2 Sentiment Distribution of CryptoPunks-related Tweets (first 200 tweets)**
![fig.2](https://github.com/yutongquan/llm-cryptopunk/blob/main/image/llama2-distribution.png)

**Fig.3: VADER Sentiment of CryptoPunks-related Tweets (first 200 tweets)**
![fig.3](https://github.com/yutongquan/llm-cryptopunk/blob/main/image/vader-sentiment-graph.png)

**Fig.4: VADER Sentiment Distribution of CryptoPunks-related Tweets (first 200 tweets)**
![fig.4](https://github.com/yutongquan/llm-cryptopunk/blob/main/image/vader-distribution.png)

Based on the analysis of the initial 200 CryptoPunks-related tweets using both the LlaMa2 large language model and the traditional NLP tool VADER, we observed a notable trend: LlaMa2 generally identified more neutral sentiments compared to VADER. This discrepancy suggests that the fine-tuning of the model may significantly influence its performance. Currently, LlaMa2 hasn't been specifically fine-tuned with data related to the crypto asset domain, which might be impacting its autonomous decision-making capabilities. The next step of this research involves the selection of an apt dataset that reflects the social media discourse surrounding crypto assets. This dataset will be used to conduct targeted fine-tuning on the LlaMa2 model, aiming to achieve more precise and relevant sentiment analysis results.

## References
**Data Reference:** 
https://github.com/HCI-Blockchain/NFT-2023

**Code Reference:** 
https://github.com/Rising-Stars-by-Sunshine/STATS201_Yiwei_Final_Project
