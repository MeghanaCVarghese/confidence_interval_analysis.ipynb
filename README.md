# 📊 Estimation of Confidence Intervals for Print-Head Durability

![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python)
![Statistics](https://img.shields.io/badge/Statistics-Inference-green)
![Confidence Interval](https://img.shields.io/badge/Concept-Confidence%20Interval-orange)
![Hypothesis Testing](https://img.shields.io/badge/Concept-Hypothesis%20Testing-yellow)
![Data Analysis](https://img.shields.io/badge/Data-Analysis-purple)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)
![Status](https://img.shields.io/badge/Project-Completed-brightgreen)
---

## 📌 Project Overview

This project focuses on estimating the **mean durability of print-heads** using statistical techniques.

Since the testing process is **destructive and costly**, only a small sample is available.  
Hence, **confidence intervals** are used to estimate the true population mean.

---

## 🎯 Problem Statement

A manufacturer wants to estimate how long print-heads last (in millions of characters printed before failure).

- Testing destroys the product  
- Only **15 samples** are available  
- Need a **reliable estimate of the population mean**

---

## 📊 Dataset

Durability values (in million characters):

1.13, 1.55, 1.43, 0.92, 1.25, 1.36, 1.32,  
0.85, 1.07, 1.48, 1.20, 1.33, 1.18, 1.22, 1.29  

---

## ⚙️ Objective

- Construct **99% Confidence Intervals** using:
  - Sample standard deviation (t-distribution)
  - Known population standard deviation (z-distribution)
- Compare both approaches
- Interpret the results

---

## 🔍 Methodology

### 📌 Case 1: t-distribution (σ unknown)
- Used when population standard deviation is unknown  
- Sample standard deviation is used  
- Suitable for **small sample sizes (n < 30)**  

### 📌 Case 2: z-distribution (σ known)
- Used when population standard deviation is known  
- Provides more precise estimation  

---

## 📈 Results

### Sample Statistics
- Sample Size (n): 15  
- Sample Mean: **1.2387 million characters**  
- Sample Standard Deviation: **0.1932**

---

### (a) 99% CI using t-distribution (df = 14)

**(1.0902, 1.3871)** million characters  

---

### (b) 99% CI using z-distribution (σ = 0.2)

**(1.1057, 1.3717)** million characters  

---

## 🧠 Interpretation

- The **t-distribution interval is wider** because:
  - Population standard deviation is unknown  
  - More uncertainty is considered  

- The **z-distribution interval is narrower** because:
  - Population standard deviation is known  
  - Less uncertainty in estimation  

👉 This demonstrates how **uncertainty affects statistical estimation**

---

## 💡 Key Learnings

- Difference between t-distribution and z-distribution  
- Importance of sample size in confidence intervals  
- Handling real-world constraints (destructive sampling)  
- Understanding uncertainty in statistical inference  

---

## 📊 Business Impact

- Helps estimate product reliability with limited samples  
- Reduces cost of destructive testing  
- Supports data-driven decision making in manufacturing

---

## 🚀 How to Run

```bash
git clone https://github.com/MeghanaCVarghese/Confidence-Interval-Estimation.git
cd Confidence-Interval-Estimation
pip install -r requirements.txt

---

## 👩‍💻 Author

Meghana C Varghese
Data Scientist | Machine Learning Enthusiast
