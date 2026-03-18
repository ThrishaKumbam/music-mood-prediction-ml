# Music Mood Prediction Using Neural Networks

This project implements a multi-class neural network classifier to predict mood categories from structured audio feature data. The project was completed as part of the **Artificial Intelligence course** in the **Master’s in Computer Science program at SUNY Polytechnic Institute**.

## Project Overview

The goal of this project is to classify mood categories such as **Happy, Sad, Energetic, Calm**, etc., using numerical audio features extracted from music data.

The project includes:
- data preprocessing
- exploratory data analysis (EDA)
- neural network model development
- model evaluation and comparison

## Dataset

The dataset contains over **1100 records** with **18+ audio features**, including:

- danceability
- energy
- valence
- tempo
- acousticness

Target variable: **mood (multi-class classification)**

Dataset file:

`data_moods.csv`

## Model Architecture

### Base Model
- Dense(128) → Dropout(0.3) → ReLU  
- Dense(64) → Dropout(0.2) → ReLU  

### Final Model (Wider Network)
- Dense(256) → Dropout(0.3) → ReLU  
- Dense(128) → Dropout(0.2) → ReLU  

Output Layer: Softmax  
Loss: Categorical Crossentropy  
Optimizer: Adam  

## Methodology

1. Data cleaning and preprocessing  
2. Label encoding for mood categories  
3. Feature scaling using StandardScaler  
4. Exploratory Data Analysis (EDA)  
5. Train / validation / test split (70/15/15)  
6. Neural network training  
7. Model evaluation using performance metrics  

## Results

- Accuracy: ~88%  
- Precision: ~0.89  
- Recall: ~0.88  
- F1-score: ~0.88  

The model demonstrated strong generalization across all mood classes.

Some confusion occurred between similar moods such as **Sad and Calm**, while distinct moods like **Energetic** were classified accurately.

## Project Files
```
music-mood-prediction-ml
│
├── mood_classification_model.ipynb
│ Jupyter notebook containing full implementation
│
├── data_moods.csv
│ Dataset used for training and testing
│
├── mood_classification_presentation.pptx
│ Presentation explaining model architecture, EDA, and results
│
├── README.md
├── requirements.txt
└── .gitignore
```

## How to Run

Clone the repository:
git clone <repo-url>

cd music-mood-prediction-ml

Install dependencies:
pip install -r requirements.txt

Run Jupyter Notebook:
jupyter notebook

Open:
mood_classification_model.ipynb

## Learning Outcomes

This project helped develop practical understanding of:

- neural networks and deep learning fundamentals  
- feature engineering and preprocessing  
- classification algorithms  
- evaluation metrics  
- overfitting and regularization techniques  
- real-world data analysis  

## Academic Context

This project was completed for the **Artificial Intelligence course**  
Master’s in Computer Science  
**SUNY Polytechnic Institute**

## Author

**Thrisha Reddy Kumbam**  
Master’s Student – Computer Science  
SUNY Polytechnic Institute  
```
The repository contains the following files:
