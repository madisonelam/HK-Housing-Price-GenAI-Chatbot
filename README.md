# hk-housing-price-genai-chatbot
GenAI chatbot for Hong Kong housing price prediction — combines KNN/linear regression models with an LLM-orchestrated conversational agent for buyers and sellers. Team project, COMP 1945.


HK Housing Price GenAI Chatbot
Team Final Project — COMP 1945 (AI: Data to Applications)
A generative AI chatbot that predicts Hong Kong housing transaction prices and assists both buyers and sellers through a natural-language conversational interface. Built by a 5-person team combining traditional ML (KNN, Linear Regression) with an LLM-orchestrated agent pipeline, trained on ~149,882 real transaction records.


Overview
Traditional real estate valuation in Hong Kong relies on manual, time-consuming appraisal methods with limited transparency. This project builds a GenAI-powered alternative: a conversational agent that infers user intent (buyer vs. seller) from unstructured natural language, then orchestrates role-specific data pipelines to deliver price predictions, comparable listings, and market analysis — without requiring users to navigate complex filters or forms.
The system was built end-to-end: data preprocessing, feature engineering, dual-model price prediction (KNN + Linear Regression), and an LLM-based conversational orchestration layer deployed via Dify.


What's Included
Data preprocessing pipeline — built in KNIME, handling categorical encoding, date parsing, missing value imputation, and normalization across ~149,882 Hong Kong housing transaction records (2020–2023)
Dual-model price prediction — KNN and Linear Regression models compared for accuracy, interpretability, and computational tradeoffs; both models informed the final deployed system
LLM-orchestrated conversational agent — built on Dify, the agent infers buyer/seller intent from natural language, extracts structured requirements, and runs parallel task pipelines (price prediction, comparable listings, marketing copy generation, competitor analysis)
Evaluation framework — mixed-method plan combining quantitative metrics (click-through rate, dialogue turn count, classification accuracy audits) with qualitative user feedback
Risk mitigation design — addressed LLM hallucination risk through strict prompt constraints requiring grounded transaction data, plus fallback disclaimers when comparable data is insufficient


My Contribution
Contributed across multiple areas of the project as part of a 5-person team, including data preprocessing and feature engineering, model evaluation (KNN vs. Linear Regression tradeoffs), and system design/documentation for the report and presentation.


Team
Cheng Kit Ling · Fu Chung Yan · Lam Madison Emily · Yang Yulai · Yang Zimo
Repository Structure
hk-housing-price-genai-chatbot/


Tools & Methods
KNIME (data preprocessing) · KNN · Linear Regression · Dify (LLM agent orchestration) · Prompt Engineering · Feature Engineering · Kaggle (Hong Kong Housing Price 2020–2023 dataset)


Results
The system performed accurately in live evaluation and received strong marks in both the written report and final presentation.


Dataset
Hong Kong Housing Price (2020–2023), sourced via Kaggle (CyrusTTF, 2020) — approximately 149,882 records across district-level location data, transaction dates, and price change history.


Full Report & Slides
See docs/final_report.pdf for complete methodology, model comparison, evaluation plan, and risk analysis. See docs/presentation_slides.pdf for the final presentation deck.
