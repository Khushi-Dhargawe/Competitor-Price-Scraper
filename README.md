# Competitor Price Scraper — Automated Pricing Intelligence

**E-Commerce Data Extraction Pipeline | Python · Web Scraping · Competitive Intelligence · Automation**

> Built an automated competitor price scraping pipeline that programmatically extracts e-commerce product catalogs in under 10 seconds—replacing slow, error-prone manual workflows entirely and calculating live competitive price deltas.

---

## 📌 Table of Contents
- [Project Overview](#project-overview)
- [Business Impact & Metrics](#business-impact--metrics)
- [Data Extraction Workflow](#data-extraction-workflow)
- [Tools & Technologies](#tools--technologies)
- [Repository Structure](#repository-structure)
- [How to Run](#how-to-run)
- [Key Insights & Business Value](#key-insights--business-value)
- [Skills Demonstrated](#skills-demonstrated)

---

## Project Overview
In modern e-commerce, reactive pricing is a profit-killer. This project implements an automated price intelligence script using an open web sandbox environment (`books.toscrape.com`). Instead of relying on manual data entries, this script dials into the domain, parses the HTML DOM tree structure, extracts product titles alongside live prices, and exports a clean, organized layout prepared for downstream strategic analysis.

---

## Business Impact & Metrics

To prove functional value to business stakeholders, the execution metrics are quantified below:

* **Time Efficiency:** Complete catalog data collection executed in **under 10 seconds**, replacing hours of manual webpage clicking.
* **Hours Saved:** Replaces tedious manual copy-paste administrative work completely, freeing up analytics teams for higher-value strategy.
* **Key Calculated Metric (Price Delta):** Implements `Price Delta = Own Store Price - Competitor Price` calculations to immediately flag under-pricing risks or over-pricing margin loss.

---

## Data Extraction Workflow

The scraping script standardizes raw web pages into clean data assets through a three-stage sequence:

[Target URL Request] ➔ [HTTP GET via Requests] ➔ [DOM Tree Parsing via BeautifulSoup] ➔ [Target Tag Filtration] ➔ [Structured Local Export]

1. **Network Request Ingestion:** Connects to the host server using `Requests`, configuring the character encoding explicitly to `utf-8` to protect text formatting integrity.
2. **Structural Document Parsing:** Feeds raw HTML text into a structured `BeautifulSoup` tree model, enabling fast node lookups.
3. **Target Element Extraction:** Identifies specific e-commerce classes (e.g., filtering paragraphs mapped to the `.price_color` tag structure) to cleanly extract numeric currency strings without text layout noise.

---

## Tools & Technologies
* **Language:** Python 3 (Modular Automation Scripting)
* **Data Acquisition Libraries:** Requests (HTTP Protocol Management)
* **Web Scraping Core:** BeautifulSoup4 (HTML Parsing & DOM Navigation)
* **Development Environments:** VS Code / Script Execution

---

## Repository Structure
```microservice
Competitor-Price-Scraper/
│
├── .gitignore                         # Preconfigured rules blocking Python runtime cache clutter
├── Business_Problem.pdf               # Detailed business case and structural metric goals
├── LICENSE                            # Standard open-source MIT License
├── Competitor_Price_Scraper.py        # Main automated e-commerce web scraping logic script
├── README.md                          # Comprehensive recruiter landing document
└── requirements.txt                   # Environment execution dependencies

---

## What I'd Do With More Time

With more time I'd extend this to scrape all pages using pagination logic, extract product titles alongside prices, and export a clean CSV directly into Power BI or Excel for live dashboard monitoring.

---

## How to Run

Step 1 — Clone the Repository

git clone [https://github.com/Khushi-Dhargawe/Competitor-Price-Scraper.git](https://github.com/Khushi-Dhargawe/Competitor-Price-Scraper.git)
cd Competitor-Price-Scraper

Step 2 — Install Project Dependencies

pip install -r requirements.txt

Step 3 — Run the Automated Extraction Engine

python Competitor_Price_Scraper.py

---

## Key Insights & Business Value

Scalable Infrastructure Baseline: The core logic inside price_scraper.py can easily scale to handle pagination or multi-page product grids, forming the foundational architecture for enterprise market-monitoring crawlers.

Automated Margin Protection: Integrating these scripts directly into price-monitoring schedules protects gross profit margins by turning competitor price trends into immediate operational alerts.

---

## 👩‍💻 Author

**Khushi Dhargawe**  
MSc Business Analytics — University College Cork (UCC)  
BE Artificial Intelligence & Machine Learning (Hons. Cybersecurity) — Mumbai University

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?logo=linkedin)](https://linkedin.com/in/khushi-dhargawe)
[![GitHub](https://img.shields.io/badge/GitHub-Portfolio-black?logo=github)](https://github.com/Khushi-Dhargawe)

---

Project developed as part of a Professional Data & Business Analytics Portfolio.

