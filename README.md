Machine Learning Detection of Prompt Injection Attacks

This repository contains the materials for the CSCU9DA empirical data science case study critique and data audit. It examines a published study of machine-learning methods for detecting prompt injection in large language model (LLM) prompts.

Project overview

The project reviews the methods and claims in Dzhaliuk et al. and independently inspects the public train/test dataset. The notebook checks the downloaded files, explores data quality, and evaluates a TF–IDF Logistic Regression baseline.

The task is binary text classification (benign or malicious prompt). The dataset does not measure whether an AI agent actually reveals a secret, so benchmark detection results should not be interpreted as proof of real-world data-leak prevention.

File

Description

CSCU9DA_Assessment_Coversheet_Filled.pdf

Completed institutional assessment coversheet.

Dzhaliuk_2026_Prompt_Injection_ML.pdf

Research paper selected for the case study.

CSCU9DA_Prompt_Injection_Critique.pdf

Written critique of the paper, including its methods, findings, and limitations.

CSCU9DA_Prompt_Injection_Data_Audit.ipynb

Executable notebook for loading the public data, verifying row counts, performing exploratory checks, and evaluating an independent baseline.

Data source

The notebook uses the public jayavibhav/prompt-injection dataset on Hugging Face. It downloads the train and test Parquet files when they are not already available beside the notebook. Raw dataset files are not included in this repository.

Run the notebook

Use Python 3 and install the required packages:

pip install pandas pyarrow scikit-learn matplotlib jupyter

Then start Jupyter and open the notebook:

jupyter notebook CSCU9DA_Prompt_Injection_Data_Audit.ipynb

Run the cells from top to bottom. An internet connection is needed the first time the notebook downloads the dataset files.

AI use

AI assistance was not used in this project
