# 📈 Mutual Fund Recommendation System  
### A Similarity-Based, Explainable Recommendation Engine Using Time-Series NAV Data

---

## 🔍 Project Overview
This project implements a **real-world mutual fund recommendation system** using **similarity-based techniques** on **historical NAV time-series data**. The system recommends the **top 5 similar mutual funds** based on engineered financial and categorical features using **cosine similarity**.

The focus of this project is on **explainability, transparency, and real-life usability**, rather than black-box machine learning models.

---

## 🎯 Motivation
Investors often struggle to choose suitable mutual funds due to:
- A large number of available schemes
- Difficulty in comparing risk–return characteristics
- Over-dependence on ratings without understanding similarity

The motivation for this project came from **real-life investment discussions with my father**, which helped identify the need for a system that recommends **similar funds** rather than simply “top-performing” ones. This guided the selection of practical and meaningful features.

---

## 📊 Data Source
The raw data used in this project was collected from a public GitHub repository containing Indian mutual fund data.

🔗 **Data Source Repository**:  
https://github.com/InertExpert2911/Mutual_Fund_Data

The dataset includes:
- Mutual fund scheme metadata
- Historical NAV time-series
- Category and subcategory information

---

## 🧠 Feature Engineering
All features were **engineered from raw NAV time-series data**, ensuring full transparency.

### 📈 Performance Features
- CAGR (1 Year, 3 Years, 5 Years)
- Fund Age (in years)

### ⚠️ Risk Features
- Volatility (standard deviation of returns)
- Sharpe Ratio
- Maximum Drawdown

### 🏷 Structural Features
- Fund Category (One-Hot Encoded)
- Fund Subcategory (One-Hot Encoded)
- Minimum Investment Amount

Only features **available in the original dataset** were used to avoid artificial assumptions.

---

## 🤖 Recommendation Methodology
This is a **content-based recommendation system** inspired by academic research.

### Algorithms Used
- **Cosine Similarity** (primary similarity metric)
- Feature normalization using `StandardScaler`
- One-hot encoding for categorical features

The approach was studied and adapted from the following research paper:

📄 **Reference Paper**:  
*Enhancing Investment Decisions: A Machine Learning Approach to Recommending Stocks and Mutual Funds* (IEEE)

The implementation focuses on the **similarity-based components** of the paper for interpretability and real-world relevance.

---

 

## 🛠 Tech Stack
- Python  
- Pandas, NumPy  
- Scikit-learn  
- Cosine Similarity  
- Jupyter Notebook  
 
---

## 📊 Evaluation Strategy
Since explicit user feedback data was not available, the system was evaluated using:
- Manual sanity checks
- Category consistency across recommendations
- Comparison with and without categorical features

---

## 🚀 Future Improvements
- Incorporating expense ratio and fund ratings (if data becomes available)
- Adding investor risk-profile based filtering
- Hybrid recommendation (content + popularity)
- Real-time NAV updates

---

## 📌 Key Highlights
- Built from **raw time-series NAV data**
- Emphasis on **explainable recommendations**
- Inspired by **real investor needs**
- Research-backed methodology

---

## 🧾 Summary
> Designed and implemented a similarity-based mutual fund recommendation system using cosine similarity on engineered financial features derived from historical NAV time-series data, with an interactive web interface for real-time recommendations.

---

## 🙌 Acknowledgements
- Public GitHub data repositories
- IEEE research paper reference
- Real-world investment insights


