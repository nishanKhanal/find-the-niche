# **Find the Niche – E-Commerce Analytics for "Dashcam Front and Rear"**

## **Overview**
This project leverages **Business Intelligence (BI)** and **Data Analytics** to identify potential opportunities in the e-commerce space.  
The analysis focuses on the **"Dashcam Front and Rear"** niche, using **Helium 10 data**, advanced NLP techniques, and visualization dashboards to uncover market trends, brand dominance, and customer sentiment.

---

## **Objectives**
- Identify profitable and underserved niches in the e-commerce market.
- Analyze product, seller, and market performance for the selected keyword.
- Extract and interpret customer feedback to inform product improvement strategies.

---

## **Data Source**
- **Helium 10 Extension** export for the search term: `"Dashcam front and rear"`.
- Contains product, pricing, sales, ratings, reviews, fulfillment, and seller location data for Amazon listings.

---

## **Key Steps**
### **1. Keyword Selection**
- Keyword: *Dashcam front and rear*  
- Chosen based on **Google Trends** search volume and **Helium 10 ASIN revenue**.

### **2. Preliminary Analysis**
- Data cleaning and preprocessing.
- Filtering out **non-Amazon sellers**.
- Correlation analysis:
  - **Positive correlation** between ASIN revenue and seller age.
  - **Negative correlation** between ASIN revenue and ratings (suggesting aggressive marketing drives revenue even for lower-rated products).

### **3. Review Analysis**
- **Sentiment Analysis:**  
  - Higher ratings generally correspond to more positive review language.  
  - Some 5-star reviews contain neutral or negative sentiment (possible mismatched ratings).
- **Topic Modeling:**  
  - Most frequent review topics include generic terms such as *cam*, *dashcam*, and brand names.
- **Word Cloud:**  
  - Highlights prominent terms in customer reviews.
- **Zero-Shot Classification (facebook/bart-large-mnli):**  
  - Candidate labels: `bad mount`, `good video quality`, `works as expected`, `bad video quality`, `durability problems`, `overheating and deformation`, `stops recording`.

---


### **Features**
- **Top Products Table:** Key metrics like ASIN, BSR, review count, ratings, price, and revenue.
- **Seller Country/Region Map:** Geographic distribution of revenue.
- **Brand & Seller Revenue Pie Charts:** Market share analysis by brand and seller.

---

## **Technologies Used**
- **Python** – Data cleaning, analysis, NLP (`pandas`, `matplotlib`, `seaborn`, `nltk`, `transformers`).
- **Helium 10** – Amazon marketplace data export.
- **Plotly / Matplotlib** – Data visualization.
- **Dash / Power BI** – Dashboard creation.
- **NLP Models:** `facebook/bart-large-mnli` for zero-shot classification.

---

## **Insights**
- A few brands (e.g., **REDTIGER**, **VANTRUE**) dominate the market share (~63% combined revenue).
- Lower-rated products can still achieve high revenue through pricing and marketing strategies.
- Customer sentiment shows alignment with ratings, but with notable exceptions.
- Product improvement opportunities exist in mounting systems, video quality, durability, and heat resistance.
