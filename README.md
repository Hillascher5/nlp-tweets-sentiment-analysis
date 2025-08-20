# NLP Tweet Sentiment Classification: COVID-19
This project fine-tunes transformer-based models (e.g., BERT, RoBERTa, DeBERTa) for tweet sentiment classification using a COVID-19 tweets dataset.

## Project Structure
- `notebooks/` - EDA, training HF, training manually, models compression, evaluation notebooks
- `models/` - Fine-tuned models (see access instructions below)
- `data/` - raw data and preprocessed datasets

## Setup Instructions
#### 1. Clone the repository
git clone https://github.com/Hillascher5/nlp-tweets-sentiment-analysis.git
cd nlp-tweets-sentiment-analysis

#### 2. Install dependencies
pip install -r requirements.txt

#### 3. if using Colab - Enable GPU for faster training

## Notebooks Overview
1) **EDA**
   
Run: Text_Classification_Tweets_Sentiment_eda.ipynb

2) **Training Approaches**
   
Option A — Manual Training

Run: Full_fine_tune.ipynb

Option B — HuggingFace Trainer

Run: Train_HF_models.ipynb

3) **Model Compression**
   
Applies multiple compression techniques (pruning, distillation, quantization).

Run: Model_compression.ipynb

4) **Final Evaluation**
   
**Note - test file to run: Corona_NLP_test_to_evaluate.csv** - already in code

Run: Evaluate_saved_models.ipynb


## **Pretrained Models (Google Drive)**

Trained models are available here:

Google Drive Folder:

MyDrive/NLP_tweet_classification_covid19_project/models/

link:

https://drive.google.com/drive/folders/1v8jLPWNaS66_8lwHb36_GchlCp2toq7S?usp=drive_link

You will find:

HF_Trainer/ - models trained with HuggingFace Trainer

HF_Trainer/Compressed_models/ - models after compression
      
Manual_finetune_min_preproc_5000_samples_opt/ - manually fine-tuned models


## How to Use the Pretrained Models and all paths in notebooks

**Option 1: Mount Google Drive**

model_path_hf = "/content/drive/MyDrive/NLP_tweet_classification_covid19_project/models/HF_Trainer/"

model_path_manual = "/content/drive/MyDrive/NLP_tweet_classification_covid19_project/models/Manual_finetune_min_preproc_5000_samples_opt/"

**Option 2: Download & Load Locally**

- Download model folders from the Google Drive link above
- Place them under your local models/ directory
- Modify paths in code:
  
      model_path_hf = "models/HF_Trainer/"
  
      model_path_manual = "models/Manual_finetune_min_preproc_5000_samples_opt/"
  
Replace the commenting inside code, according to the option you choose.

**Contact**

Hilla Scher

Email: hillas@mail.tau.ac.il

GitHub: Hillascher5
