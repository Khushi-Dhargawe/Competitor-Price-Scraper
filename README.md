# 🕷️ Competitor Price Scraper — Automated Pricing Intelligence

![Python](https://img.shields.io/badge/Python-3.11-blue?logo=python)
![Requests](https://img.shields.io/badge/Requests-2.31-orange)
![BeautifulSoup4](https://img.shields.io/badge/BeautifulSoup4-4.12-green)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen)

> **Skills:** Python · Requests · BeautifulSoup4 · Web Scraping · Data Collection · Automation · Competitive Intelligence  
> **Dataset:** books.toscrape.com — open e-commerce sandbox environment  
> **Execution Time:** Under 10 seconds

---

## Why This Matters

Manual price monitoring across competitor websites costs retail teams hours every week — error-prone, slow and always out of date. Even a simple automation script eliminates that entirely and gives analysts time back for higher-value work.

---

## 📌 Project Overview

An automated competitor price scraping script that connects to a live e-commerce website, parses the HTML DOM tree, extracts product pricing data, and calculates Price Delta — the difference between your store price and the competitor price — as a structured business metric.

**Three-stage pipeline:**
1. **Request** — HTTP GET via Requests library with utf-8 encoding configured
2. **Parse** — BeautifulSoup4 navigates the DOM tree and isolates the `.price_color` tag
3. **Calculate** — Price Delta = Own Store Price − Competitor Price

---

## 🗂️ Repository Structure

```
📁 Competitor-Price-Scraper/
│
├── 📄 Competitor_Price_Scraper.py     ← MAIN FILE: Scraping + Price Delta logic
├── 📄 Business_Problem_Statement.pdf  ← Business case and metric goals
├── 📦 requirements.txt                ← Python dependencies
├── 📜 LICENSE                         ← MIT License
└── 📜 .gitignore                      ← Python cache rules
```

---

## 🔗 Pipeline Flow

```
Target URL (books.toscrape.com)
        │
        ▼
[Step 1] HTTP GET Request              ← requests.get() + utf-8 encoding
        │  Raw HTML retrieved
        ▼
[Step 2] DOM Tree Parsing              ← BeautifulSoup(html, "html.parser")
        │  HTML structured into navigable tree
        ▼
[Step 3] Tag Extraction                ← .find('p', class_='price_color')
        │  Price string isolated cleanly
        ▼
[Step 4] Price Delta Calculation
           Price Delta = Own Store Price − Competitor Price
           Positive = you are priced higher (margin risk)
           Negative = you are priced lower (revenue opportunity)
```

---

## 📊 Key Results

| Metric | Value | Business Implication |
|---|---|---|
| Execution time | Under 10 seconds | Replaces hours of manual copy-paste work |
| Price Delta | Own Price − Competitor Price | Flags under-pricing and over-pricing instantly |
| Encoding | utf-8 configured | Currency symbols extracted cleanly — no data corruption |
| Scalability | Modular logic | Extendable to paginated catalogs and multiple URLs |

---

## 💼 Business Applications

- **Retail:** Real-time competitor price monitoring without manual audits
- **E-Commerce:** Automated margin protection — flag under-pricing before it impacts revenue
- **Pricing Strategy:** Feed structured price deltas into BI tools for live dashboard tracking
- **Operations:** Free up analyst time from repetitive data collection for higher-value work

---

## What I'd Do With More Data

With more time I'd extend this to scrape all pages using pagination logic, extract product titles alongside prices, and export a clean CSV directly into Power BI or Excel for live dashboard monitoring. I'd also add scheduling via cron jobs so the script runs automatically every morning before trading hours.

---

## 🚀 How to Run

```bash
git clone https://github.com/Khushi-Dhargawe/Competitor-Price-Scraper.git
cd Competitor-Price-Scraper
pip install -r requirements.txt
python Competitor_Price_Scraper.py
```

---

## 📁 Related Projects

| # | Project | Skills |
|---|---|---|
| 1 | [Customer Shopping Behaviour Analysis](../Customer-Shopping-Behaviour-Analysis) | Python · PostgreSQL · Power BI |
| 3 | [Zepto Retail Analytics](../Zepto-Retail-Analytics) | Python · SQL · Power BI |
| **13** | **Competitor Price Scraper ← You are here** | **Python · Requests · BeautifulSoup4** |
| 4 | [Customer Churn Prediction](../Customer-Churn-Prediction) | XGBoost · SHAP · LIME |

---

## 👩‍💻 Author

**Khushi Dhargawe**  
MSc Business Analytics — University College Cork (UCC)  
BE Artificial Intelligence & Machine Learning (Hons. Cybersecurity) — Mumbai University

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?logo=linkedin)](https://www.linkedin.com/in/khushi-dhargawe/)
[![GitHub](https://img.shields.io/badge/GitHub-Portfolio-black?logo=github)](https://github.com/Khushi-Dhargawe)

---

## 📜 License

This project is licensed under the MIT License — see [LICENSE](LICENSE) for details.
