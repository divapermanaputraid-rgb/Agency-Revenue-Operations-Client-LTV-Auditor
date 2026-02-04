# Agency Revenue Operations & Client LTV Auditor

![Version](https://img.shields.io/badge/version-1.0--foundation-blue)
![Python](https://img.shields.io/badge/Python-3.9+-yellow?logo=python)
![Industry](https://img.shields.io/badge/Industry-Advertising--Tech-green)

## Executive Summary
Proyek ini melakukan audit komprehensif terhadap kesehatan finansial dan efisiensi operasional pada **Apex Media Group (AMG)**, sebuah agensi periklanan *full-service*. Fokus utama adalah membedah *Unit Economics* klien untuk memastikan pertumbuhan pendapatan (*top-line*) sejalan dengan profitabilitas bersih (*bottom-line*).

Audit ini menjawab tantangan **Resource Misallocation** dengan memetakan biaya tenaga kerja internal terhadap pendapatan per klien untuk mengidentifikasi akun yang memberikan dampak ekonomi tertinggi.

## Business Case: Operational Efficiency & Profitability Audit

**Apex Media Group (AMG)** adalah agensi periklanan *full-service* yang mengelola portofolio klien lintas industri. Dalam operasionalnya, pertumbuhan pendapatan (*Top-line*) seringkali tidak sejalan dengan pertumbuhan laba bersih (*Bottom-line*).

Masalah utama yang diidentifikasi adalah **"Resource Misallocation"**, di mana klien-klien besar (*Enterprise*) mengonsumsi jam kerja tim yang sangat tinggi sehingga menggerus margin keuntungan. Audit ini bertujuan untuk membedah *Unit Economics* per klien dan per layanan guna mengidentifikasi kebocoran profitabilitas.

### **Business Questions (BQ) v1.0:**
1. **Service Profitability (Efficiency):** Lini layanan mana (Digital, Creative, atau Media) yang menghasilkan margin keuntungan paling sehat relatif terhadap konsumsi sumber daya?
2. **Client Tiering (Profitability):** Apakah klien Tier 1 memberikan laba bersih yang lebih besar dibandingkan Tier 2 setelah memperhitungkan biaya kompleksitas operasional (*Complexity Overhead*)?
3. **Industry Excellence (Strategic Context):** Industri mana yang menunjukkan loyalitas tertinggi (*Retention*) dan *Lifetime Value* (LTV) paling panjang?


## Project Documentation
* 📄 [Business Case & Strategic Objectives](docs/business_case.md)
* 📖 [Data Dictionary & Schema](docs/data_dictionary.md)

---

## Project Structure
```text
agency-revenue-auditor/
├── data/
│   ├── raw/                # dim_clients, fact_revenue, fact_costs
│   └── processed/          
├── docs/                   # Business & Data Documentation
├── notebooks/
│   └── 01_data_generation.ipynb
├── README.md
└── requirements.txt