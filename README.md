# 🎬 Movie Sales & Performance Dashboard (2007–2011)

## 📸 Dashboard Preview
![Movie Sales Dashboard](Dashboard.png)

---

## 📊 Project Overview
This Excel dashboard analyzes Hollywood’s most profitable movies (2007–2011) using the Kaggle dataset:  
Hollywood’s Most Profitable Stories → https://www.kaggle.com/datasets/brendan45774/hollywood-most-profitable-stories

The objective is to evaluate movie performance through **Worldwide Gross**, **Profitability**, and **Audience/Critic reception**.  
A custom metric called **Combined Score** was engineered to balance audience and critic perspectives, and movies were further classified into performance tiers using Rating Category Logic.

---

## 📊 Key KPIs
- Total Titles Analyzed: 74 films  
- Total Global Revenue: $10.09B  
- Average Profitability Index: 4.74  
- Top Grossing Movie: *The Twilight Saga: New Moon*  
- Most Profitable Movie: *Fireproof*  
- Top Studio: Warner Bros.  
- Top Performing Genre: Comedy  

---

## 🛠️ Data Transformation & Logic

### 🔹 Combined Score
A new column was created to combine audience and critic ratings:

Formula:
(Audience Score % + Rotten Tomatoes %) / 2

### 🔹 Rating Category Logic
Movies were categorized into tiers using a nested IF function:

High: ≥ 75  
Medium: 41 – 74  
Low: ≤ 40  

Excel Formula:
=IF([@[Combined Score]]>=75,"High",IF([@[Combined Score]]>40,"Medium","Low"))

---

## 📊 Visualizations
- Top 10 Movies by Worldwide Gross  
- Top 10 Most Profitable Movies  
- Top Genres by Worldwide Gross  
- Box Office Trend (2007–2011)  
- Average Profitability by Year  
- Average Profitability by Genre (Pie Chart)  
- Sentiment Classification (High / Medium / Low)  

---

## 💡 Insights
- Comedy emerged as the most consistently profitable genre.  
- Smaller budget films like *Fireproof* achieved exceptional profitability despite modest gross revenue.  
- Audience and critic alignment (via Combined Score) highlighted films with balanced reception.  
- Warner Bros. dominated as the top studio in terms of revenue contribution.  
- Profitability trends varied year to year, showing resilience in certain genres despite market fluctuations.  

---

## 🛠️ Tools & Techniques
- Microsoft Excel  
- PivotTables for aggregations  
- Slicers for interactive filtering  
- Charts (Bar, Line, Pie) for visualization  
- Custom number formatting for clarity  
- Feature engineering (Combined Score metric)  
- Nested IF logic for sentiment classification  

---

## 📂 Files in Repository
- MovieSalesDashboard.xlsx → Interactive Excel dashboard  
- HollywoodsMostProfitableStories.csv → Source dataset  
- Dashboard.png → Screenshot preview  
- README.md → Documentation  

---

## 🚀 How to Use
1. Download the Excel file (MovieSalesDashboard.xlsx).  
2. Open in Microsoft Excel.  
3. Use slicers to filter by genre, studio, or year.  
4. Explore KPIs and charts for insights.  

---

## 📝 Notes
- Dataset source: Kaggle (linked above).  
- Combined Score and Rating Category Logic were engineered to enhance analysis.  
- Dashboard designed for recruiter‑friendly portfolio presentation.  




