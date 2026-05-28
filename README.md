# Competitor Price Scraper: Automated Market Intelligence Engine

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
├── src/
│   ├── __init__.py            # Packages directory for clean modular lookups
│   └── price_scraper.py       # Main production data acquisition script
│
├── docs/
│   └── Business_Problem_Statement.md  # Detailed business case and metric goals
│
├── .gitignore                 # Preconfigured rules blocking runtime cache clutter
├── LICENSE                    # Standard open-source MIT License
├── README.md                  # Comprehensive recruiter landing document
└── requirements.txt           # Environment execution dependencies

How to Run

Step 1 — Clone the Repository

git clone [https://github.com/Khushi-Dhargawe/Competitor-Price-Scraper.git](https://github.com/Khushi-Dhargawe/Competitor-Price-Scraper.git)
cd Competitor-Price-Scraper

Step 2 — Install Project Dependencies

pip install -r requirements.txt

Step 3 — Run the Automated Extraction Engine

python src/price_scraper.py

Key Insights & Business Value
Scalable Infrastructure Baseline: The core logic inside price_scraper.py can easily scale to handle pagination or multi-page product grids, forming the foundational architecture for enterprise market-monitoring crawlers.

Automated Margin Protection: Integrating these scripts directly into price-monitoring schedules protects gross profit margins by turning competitor price trends into immediate operational alerts.

Project developed as part of a Professional Data & Business Analytics Portfolio.
