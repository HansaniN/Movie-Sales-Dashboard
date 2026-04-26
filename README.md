# 🎬 Movie Sales Dashboard

## 📸 Dashboard Preview
![Movie Sales Dashboard](Dashboard.png)

## 📊 Project Overview
This Excel dashboard analyzes Hollywood’s most profitable movies (2007–2011) using a Kaggle dataset.  
The objective is to evaluate movie performance through revenue, profitability, and audience/critic reception.

Dataset used:  
[Hollywood’s Most Profitable Stories](https://www.kaggle.com/datasets/brendan45774/hollywood-most-profitable-stories)

---

## 📊 Key KPIs
- **Total Titles Analyzed:** 74 films  
- **Total Global Revenue:** $10.09B  
- **Average Profitability Index:** 4.74  
- **Top Grossing Movie:** *The Twilight Saga: New Moon*  
- **Most Profitable Movie:** *Fireproof*  
- **Top Studio:** Warner Bros.  
- **Top Performing Genre:** Comedy  

---

## 🧮 Feature Engineering: Combined Score

To better evaluate movie reception, a new metric was created by combining audience and critic ratings.

### 📊 Combined Score Formula

:contentReference[oaicite:0]{index=0}

This metric balances:
- Audience perception (Audience Score %)
- Critical reviews (Rotten Tomatoes %)

---

### 🏷️ Sentiment Classification

A derived column was created to categorize movies based on Combined Score:

```excel
=IF([@[Combined Score]]>=75,"High",
IF([@[Combined Score]]>40,"Medium","Low"))
