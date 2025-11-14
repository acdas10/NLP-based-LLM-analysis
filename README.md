# NLP-Based LLM Analysis

## Overview

This repository contains the code and analysis data for the research paper "An NLP-Based Evaluation of LLM Across Creativity, Factual Accuracy, Open-Ended and Technical Explanations".

This study conducts a comparative analysis of three advanced Large Language Models (LLMs)—ChatGPT 4.0, DeepSeek, and Gemini—to evaluate their performance across four distinct categories:

Creativity (e.g., storytelling, poetry)

Factual Accuracy (e.g., scientific differences)

Open-Ended Discussion (e.g., ethical implications)

Technical Explanation (e.g., blockchain technology)

Using a combination of statistical and linguistic metrics, this project quantifies the quality, readability, and reliability of AI-generated text.

## Repository Structure


Response analysis-stage_1.ipynb

Contains data collection and preliminary analysis for Stage 1 prompts (e.g., Mars colonization story, AC vs DC current).

Response analysis-stage_2.ipynb

Contains data collection and preliminary analysis for Stage 2 prompts (e.g., Space exploration poem, Renewable energy benefits).

Final_llm.ipynb

The consolidated analysis file containing the final statistical evaluations, including ANOVA (F-tests) and Tukey HSD post-hoc tests, along with final visualizations (Boxplots, Pair plots).

## Methodology

Models Evaluated

ChatGPT 4.0 (OpenAI)

DeepSeek R1 (DeepSeek AI)

Gemini (Google DeepMind)

## Evaluation Metrics

The repository implements various NLP techniques to score model responses:

Readability: Measured using the Dale-Chall readability score (via textstat).

Lexical Diversity: Analyzed using Type-Token Ratio (TTR) to measure vocabulary richness.

Semantic Similarity: Calculated using Cosine Similarity with TF-IDF (via scikit-learn).

Sentiment Analysis: Polarity scores determined using TextBlob.

Grammatical Correctness: Error counts assessed using Language Tool.

## Statistical Analysis

To determine if performance differences were statistically significant, the project utilizes:

One-way ANOVA (F-test) ($p < 0.05$)

Tukey HSD (Honestly Significant Difference) for pairwise comparisons.

## Authors

This research and analysis is a collaborative work by:

Ashik Chandra Das - Institute of Computer Science, University of Potsdam

Novera Tansue Nasa - Institute of Computer Science, University of Potsdam

Citation

If you use this code or methodology in your research, please cite the associated paper:

Nasa, Q.N.T., & Das, A.C. (2025). An NLP-Based Evaluation of LLM Across Creativity, Factual Accuracy, Open-Ended and Technical Explanations. ICCK Transactions and Journals, 1(1), 1-9. http://dx.doi.org/10.62762/ICCK.2022.000000

Requirements

To run the notebooks, you will need the following Python libraries:
```bash
pip install nltk textblob scikit-learn textstat language-tool-python matplotlib seaborn
```
