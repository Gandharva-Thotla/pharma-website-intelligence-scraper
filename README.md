# Pharma Website Intelligence Scraper

This project contains a lightweight Python-based website scraper designed for early-stage pharma intelligence and business screening.

The goal is to extract **observable website-level signals** and support structured analysis without making assumptions or forcing incomplete data.

---

## Project Scope

The project focuses on:
- Identifying probiotic-related signals from public company websites
- Supporting early-stage screening of probiotics-focused businesses
- Handling real-world constraints such as JavaScript-rendered websites

---

## What the Scraper Does

- Fetches commonly used website pages (homepage, about, products, research, contact)
- Extracts visible HTML text
- Counts probiotic-related keyword occurrences
- Flags whether probiotics are mentioned
- Logs inaccessible or JavaScript-rendered pages as "not found"
- Outputs structured results in JSON format

---

## Case Study: Yakult

Yakult was used as a reference case study to apply the analysis framework.

Due to heavy JavaScript rendering and regional redirects, key content on yakult.com is not accessible via static HTML requests.  
The scraper explicitly records this limitation instead of inferring missing information.

This demonstrates transparent handling of incomplete or inaccessible data.

---

## Additional Example

A second probiotics-focused website (Lallemand Health Solutions) was analyzed to demonstrate successful extraction on a static HTML site.

---

## Limitations

- JavaScript-heavy websites may return incomplete or empty HTML
- No deep crawling, pagination, or form interaction
- Scientific claims and regulatory compliance are not validated
- Intended for screening and prioritization, not final due diligence

---

## Tech Stack

- Python
- requests
- beautifulsoup4

---

## Intended Use

This project is intended for educational and exploratory purposes, simulating early-stage pharma intelligence workflows.
