# Data Dictionary (Relational Star Schema)

Dataset disimulasikan sebagai data historis 24 bulan (Jan 2024 - Des 2025) dengan struktur relasional.

### 1. Dimension Table: `dim_clients.csv`
*Kunci utama informasi klien.*
- `client_id`: Primary Key.
- `client_tier`: Klasifikasi Enterprise/Small-Mid.
- `industry`: Sektor bisnis klien.
- `account_manager_id`: ID AE penanggung jawab.

### 2. Fact Table: `fact_revenue.csv`
*Catatan transaksi pendapatan.*
- `period`: Timestamp bulanan.
- `client_id`: Foreign Key.
- `service_line`: Jenis layanan (Digital/Creative/Media).
- `monthly_revenue`: Nilai tagihan (Gross).

### 3. Fact Table: `fact_costs.csv`
*Catatan operasional dan beban biaya.*
- `man_hours_billed`: Investasi waktu tim.
- `external_production_cost`: Biaya vendor/produksi.
- `internal_cost_per_hour`: Standar biaya internal (IDR 350.000).