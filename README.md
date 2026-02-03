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