# AI-Driven SQL Injection Detection System

This repository contains the official implementation for the research paper: **"Evaluating AI-Driven SQL Injection Detection: A Comparative Analysis of Random Forest and CNN-LSTM Architectures."**

## 📂 Project Overview
This study compares the efficacy of traditional Machine Learning (Random Forest) against Deep Learning (CNN-LSTM) in detecting obfuscated SQL Injection attacks.

* **Baseline Model:** Random Forest (TF-IDF Vectorization)
* **Advanced Model:** CNN-LSTM (Character-level Tokenization)
* **Key Feature:** Custom Adversarial Mutation Engine to stress-test robustness.

## 🚀 How to Run
1. Open the `SQLi_Detection_System.ipynb` file in this repository.
2. Click the "Open in Colab" badge (if available) or download the file to Google Colab.
3. Download the .zip file ( ) for the dataset
4. Upload the three dataset files (`sqli.csv`, `sqliv2.csv`, `SQLiV3.csv`)  to the Colab session storage. (If you encounter some files in Sample Data folder, delete the files.)
5. Run all cells to produce the results. (Result will be difference based on the computational performances)

## 📊 Results Summary
| Model | Accuracy | FPR | Bypass Rate (Robustness) |
|-------|----------|-----|--------------------------|
| Random Forest | 99.89% | 0.00% | 26% Missed |
| CNN-LSTM | 99.72% | 0.15% | 8% Missed |

## 🛠️ Tech Stack
* Python 3.10
* TensorFlow / Keras
* Scikit-Learn
* Pandas & NumPy
