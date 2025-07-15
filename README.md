# Advanced Deep Learning Project – Tweets Sentiment Classification

This repository contains the code and resources for a sentiment classification project based on the **"Coronavirus tweets NLP - Text Classification"** dataset.

The project is part of the **Advanced Deep Learning** course and follows two main parts:


## Project Structure
├── Text_Classification_Tweets_Sentiment.ipynb # Main notebook (Part A + Part B)
├── data/
│ └── Corona_NLP_train.csv # Training data
│ └── Corona_NLP_test.csv # Testing data
├── models/ # Folder for saving trained model checkpoints
├── outputs/ # Folder for storing prediction results (optional)
├── README.md # This file


## Dataset

- **Source:** [Kaggle – Coronavirus tweets NLP](https://www.kaggle.com/datasets/datatattle/covid-19-nlp-text-classification)
- The data is available in the `data/` folder.


## How to Run

1. **Set up environment (recommended via Conda):**
   ```bash
   conda create -n adv_dl_env python=3.9
   conda activate adv_dl_env
   pip install -r requirements.txt
2. **Launch Jupyter Notebok**
3. **Open notebook:**
     Text_Classification_Tweets_Sentiment.ipynb
    

## Project Highlights

- Performed **Exploratory Data Analysis (EDA)** on a real-world tweet sentiment dataset.
- Applied **text preprocessing**: tokenization, stopword removal, lemmatization.
- Fine-tuned and compared **pretrained Transformer models** (BERT, RoBERTa) using Hugging Face.
- Tracked experiments with **Weights & Biases (W&B)** and optimized hyperparameters using **Optuna**.
- Performed **model compression** using three techniques for efficiency and deployment readiness.
