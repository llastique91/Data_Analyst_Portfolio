# 🏙️ Spreadsheet Data Analysis: Manhattan Airbnb Market

## 📊 Project Overview
In this Business Intelligence Analytics project, I analyzed the Manhattan vacation rental market using spreadsheet tools to support a client's investment decisions. The goal was to identify which neighborhoods and property sizes perform best on Airbnb and estimate their revenue potential.

This project is part of Sprint 1 from my Business Intelligence Analytics program.

## 🔍 Key Business Questions
1. Which neighborhoods and property sizes are most attractive for vacation rentals?
2. How much revenue did the top-performing listings generate?

## 🛠 Tools & Techniques
- Microsoft Excel
- Pivot Tables
- Data Cleaning & Transformation (IF, SUMIF)
- Data Visualization (Bar Charts)
- Documentation (Changelog, Executive Summary)

---

## 🧹 Data Cleaning Steps

### Listings Sheet
- Created a `neighborhood_clean` column to standardize inconsistent neighborhood names.
- Created a `bedrooms_clean` column to clean empty bedroom values (converted nulls to 0 = studio).

### Calendar Sheet
- Added a `revenue_earned` column:  
  - If `available = "f"` (i.e., rented), used `adjusted_price` as revenue.  
  - Else, revenue set to `$0`.

---

## 📈 Analysis Highlights

### 🏘️ 1. Top 10 Most Attractive Neighborhoods
Defined attractiveness using `number_of_reviews_ltm` (last 12 months).  
**Top 3 neighborhoods:**
- Lower East Side  
- Hell's Kitchen  
- Harlem  

> ✅ Included a bar chart visualizing the top 10 neighborhoods by review count.

---

### 🛏️ 2. Most Popular Property Sizes
Most commonly rented units across all listings:
- Studios (0 bedrooms)  
- 1-bedroom  
- 2-bedroom  

Neighborhood-specific preferences were identified, such as:
- **Harlem**: Most popular = 1-bedroom  
- **Midtown**: Most popular = Studio

---

### 💰 3. Revenue Estimation
- Used 30-day calendar data to estimate revenue per listing.
- Multiplied monthly revenue by 12 for annual projections.
- Flagged listings in top 10 neighborhoods with their most popular bedroom size using a `top_listing` indicator.

**Top-Earning Listing**
- **Listing ID**: `49946551`  
- **Monthly Revenue**: $29,940  
- **Projected Annual Revenue**: ~$359,280  

---

## ✅ Final Deliverables
- Executive Summary and Table of Contents
- Changelog with documented cleaning steps and assumptions
- Hidden irrelevant columns for clarity
- Consistent formatting (borders, font styles, background colors)

---


## 💡 Key Takeaways
- Lower East Side and Hell’s Kitchen are among the best neighborhoods to invest in for Airbnb rentals.
- 1-bedroom and studio apartments are the most attractive property sizes across Manhattan.
- Revenue modeling using calendar data provides strong investment insight.

---

## 🚀 Next Steps
This project is the foundation for more advanced analysis in future sprints involving SQL, Tableau, and Python.

---

## 📬 Let’s Connect
Interested in BI, data analytics, or real estate tech?  
Check out more of my work on GitHub or reach out via [LinkedIn](your-linkedin-url).
