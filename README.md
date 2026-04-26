# 🎬 Movie Sales & Performance Dashboard (2007–2011)

## 📸 Dashboard Preview
![Movie Sales Dashboard](Dashboard.png)

An interactive Excel dashboard analyzing the financial performance and critical reception of Hollywood films (2007–2011).  
Built using the Kaggle dataset: [Hollywood’s Most Profitable Stories](https://www.kaggle.com/datasets/brendan45774/hollywood-most-profitable-stories).

---

## 📊 Project Overview
This project explores how **financial success** (Worldwide Gross, Profitability) aligns with **audience and critic reception**.  

The dashboard enables users to identify trends across **genres, studios, and years**, while evaluating whether highly rated films are always the most profitable.

---

## 📊 Key KPIs
- **Total Movies Analyzed:** 74  
- **Total Worldwide Gross:** $10.09B  
- **Average Profitability Index:** 4.74  
- **Top Grossing Movie:** *The Twilight Saga: New Moon*  
- **Most Profitable Movie:** *Fireproof*  
- **Top Studio:** Warner Bros.  
- **Top Genre:** Comedy  

---

## 🛠️ Data Transformation & Logic

### 🔹 Combined Score
A custom metric was created to balance audience and critic perspectives:

```excel
Combined Score = (Audience Score % + Rotten Tomatoes %) / 2
