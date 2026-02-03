# Agency Revenue Operations & Client LTV Auditor (v1.0)

##  Overview
Proyek ini berfokus pada audit kesehatan finansial dan operasional dalam ekosistem agensi iklan (AdTech/Creative Agency). Proyek ini menjembatani peran **Account Executive (AE)** dalam mengelola hubungan klien dan **Data Analyst (DA)** dalam memvalidasi profitabilitas bisnis melalui metrik *Unit Economics*.

Tujuan utama dari versi 1.0 ini adalah memberikan visibilitas penuh terhadap **Net Profit Margin** per klien dan estimasi **Lifetime Value (LTV)** berdasarkan data historis.

---

##  Repository Structure
```text
agency-revenue-auditor/
├── data/
│   ├── raw/                # Data asli (tidak boleh diedit manual)
│   └── processed/          # Data yang sudah dibersihkan/dihitung margin-nya
├── notebooks/
│   ├── 01_data_generation.ipynb   # Script untuk membuat mock data
│   ├── 02_eda_profitability.ipynb # Analisis profitabilitas klien
│   └── 03_ltv_analysis.ipynb      # Perhitungan LTV & Churn
├── src/                    # Script Python (.py) untuk fungsi reusable
│   ├── __init__.py
│   ├── calculation.py      # Rumus LTV, CAC, Margin
│   └── visualization.py    # Template chart agar konsisten
├── visuals/                # Export chart (.png/.jpg) untuk slide presentasi
├── .gitignore              # Mengabaikan venv, .DS_Store, dan cache
├── requirements.txt        # Daftar library (pandas, matplotlib, dll)
└── README.md               # Dokumentasi Business Case & Temuan Utama

## Metrik Utama (Business Logic)
Proyek ini menggunakan beberapa perhitungan standar industri untuk mengukur kesehatan akun:

**1. Net Profit Margin per Client:**
Menghitung keuntungan bersih setelah dikurangi biaya langsung (ads spend/vendor) dan biaya tenaga kerja operasional (man-hours).
$$Margin = \frac{Revenue - (Direct Costs + Operational Labor)}{Revenue}$$

**2. Customer Lifetime Value (LTV):**
Estimasi total nilai ekonomi klien selama durasi kerja sama.
$$LTV = \text{Avg. Monthly Revenue} \times \text{Gross Margin} \times \text{Customer Lifespan}$$

---

## Project Status: v1.0 - The Foundation (Ongoing)
- [x] Repository Setup & Folder Structuring
- [ ] Business Questions (BQ) Definition
- [ ] Mock Data Generation
- [ ] Exploratory Data Analysis (EDA)
- [ ] Final Dashboard & Insights