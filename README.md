# Decoding Sentiments in NFT Social Media Discourse: Leveraging Large Language Models for Human Sentiment Analysis

## General information
- **Author**: Yutong Quan, Political Economy (Economics), Class of 2024, Duke Kunshan University
- **Signature Work Mentor**: Prof. Luyao Zhang, Duke Kunshan University
- **Disclaimer**: Submissions to the Duke Kunshan University Signature Work Project.
- **Acknowledgments**: First, I would like to express my most sincere gratitude to Prof. Luyao Zhang for her generous and inspiring guidance on this signature work project, her ECON 211 and STATS 201 courses provided an important foundation for my research career. Also, I would like to thank the support of the DKU Summer Research Scholars program, which laid the foundation for the birth of this research idea. Thanks to all my classmates and friends for their valuable support and comments on this project.

## Project Summary
- **Background & Motivation**:
In the spring of 2023, I had the privilege of co-authoring a research paper titled "On the Mechanics of NFT Valuation: AI Ethics and Social Media" with Prof. Luyao Zhang, Prof. Xin Tong, and two other DKU students. In that previous study, we conducted empirical analysis on social media, blockchain, and cryptocurrency exchange data to investigate how sentiment, gender, and skin tone influence the valuation of NFTs. A key aspect of the study was sentiment analysis of social media discussions, but the methodology was limited to using lexicon and rules-based sentiment analysis tools like the Valence Aware Dictionary and sEntiment Reasoner (VADER). The recent popularity of sentiment analysis tools like ChatGPT and LlaMA has increased my curiosity. Therefore, this signature work project aims to extend previous research methods to explore whether AI large language models can perform sentiment analysis on the same NFT Twitter (X) data, and examine the performance differences between large language models and traditional NLP tools in performing sentiment analysis tasks.
- **Research Questions**:
  -  What are the sentiment analysis results of CryptoPunks-related tweets performed by large language models?
  -  What are the similarities and differences between the sentiment analysis results performed by large language models (LlaMA2) and those of traditional NLP tools (VADER)?
- **Application Scenario**: 

- **Methodology**:
  - Apply Snscrape API to collect tweets with the #cryptopunk hashtag.
  - Apply LlaMA2 to collected text to perform sentiment analysis.
  - Evaluate the performance of LlaMA2 and VADER.
- **Expected Results**:
  - LLMs can be applied to conduct sentiment analysis for NFT-related social media content.
  - LLMs perform better than traditional NLP tools when performing sentiment analysis tasks for social media texts.
- **Intellectual Merit & Practical Impacts**: 
As a cutting-edge technology, LLM sentiment analysis has not been widely used in various fields, especially social media content related to cryptocurrencies or non-homogeneous tokens. This signature work project expands our understanding of NFT's social media discourse by combining AI large language models with the field of blockchain-based crypto assets. It not only enhances the accuracy of sentiment analysis but also paves the way for the development of domain-specific (crypto asset) sentiment analysis tools based on large language models. In addition, the development of more accurate sentiment analysis tools helps us to more accurately capture the market sentiment of crypto assets, thus providing valuable references for stakeholders. Relevant research data can also contribute to further NFT price forecasts.

## Table of Contents
- [Data](https://github.com/yutongquan/llm-cryptopunk/edit/main/)
- [Code](https://github.com/yutongquan/llm-cryptopunk/edit/main/)
- [Images](https://github.com/yutongquan/llm-cryptopunk/edit/main/)
- [Reference](https://github.com/yutongquan/llm-cryptopunk/edit/main/)

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

Based on observations from these four images, we noticed that LlaMa2 tended to judge more neutral emotions than VADER by performing sentiment analysis with both a large language model and a traditional NLP tool on the first 200 tweets related to CryptoPunks. My initial judgment is that this may be influenced by fine-tuning because the current model has not been fine-tuned based on data from the crypto asset-related fields, thus affecting the autonomous judgment of the model. The next step is to select appropriate fine-tuning data sets for the social media discourse of crypto assets and conduct targeted training on the LlaMa2 model, thus obtaining a more accurate sentiment analysis result.

## References
**Data Reference:** 
https://github.com/HCI-Blockchain/NFT-2023

**Code Reference:** 
https://github.com/Rising-Stars-by-Sunshine/STATS201_Yiwei_Final_Project
