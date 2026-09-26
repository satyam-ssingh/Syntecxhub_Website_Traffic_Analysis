## 🎯 Objective
Analyze a Google Analytics 4 (GA4) website traffic export to understand where visitors come from,
when they visit, how engaged they are, and how the site performs — then turn that into KPIs,
trends, and a business dashboard with clear, actionable recommendations.

## 📁 Dataset
GA4 export (`data-export.csv`) at **Channel × Hour** granularity — 3,182 rows covering
**6 Apr 2024 – 3 May 2024** (28 days).

Columns: `Channel group`, `Date + hour`, `Users`, `Sessions`, `Engaged Sessions`,
`Average engagement time per session`, `Engaged sessions per user`, `Events per session`,
`Engagement rate`, `Event count`.

## 🛠️ Tools & Libraries
- Python 3
- pandas, numpy — data cleaning & analysis
- matplotlib, seaborn — visualization
- Jupyter Notebook

## 📌 What's Inside
| Section | Covers |
|---|---|
| 1–2 | Data loading, cleaning, null/duplicate checks |
| 3 | KPI summary (Sessions, Users, Engagement Rate, etc.) |
| 4 | Traffic trends — hourly, daily, weekly, day-of-week |
| 5 | Channel-wise performance (users, engagement, bounce-like rate) |
| 5.7 | Derived Bounce Rate (100% − Engagement Rate) |
| 6–7 | Correlation analysis & channel summary table |
| 8 | Notes on additional GA4 data needed for extended sections |
| 9–12 | Pages/Session, Conversion Rate, Goal Completions, Page-level performance |
| 13 | Final interactive business dashboard (date & channel filters) |
| 14 | Key insights & recommendations |
| 15 | Final requirement-completion check |

## 🔑 Key Insights
- **Organic Social** drives the most traffic (~47K users) but has a lower engagement rate than Referral.
- **Direct traffic** has more non-engaged than engaged sessions — a quality issue worth investigating.
- **Referral** is the smallest-volume but highest-quality channel (best engagement rate & time).
- Traffic peaks **late evening/midnight** and dips in the early morning — content and campaigns should be timed accordingly.

## ▶️ How to Run
```bash
pip install pandas numpy matplotlib seaborn
jupyter notebook Website_Traffic_Analysis.ipynb
```
Run all cells top to bottom. Sections needing additional GA4 metrics (Pages/Session, Conversion
Rate, Page-level data) will print a clear message if that data isn't present, instead of failing.

## 👤 Author
**[Satyam Kumar Singh]**
Data Analysis Intern @ SyntecXHub
[https://www.linkedin.com/in/satyam-kumar-singhh] · [satyamsinghb45@gmail.com]

---
*This project was completed as part of the SyntecXHub Internship Program.*
