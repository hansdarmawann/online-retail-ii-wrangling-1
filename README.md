# 🧹 Online Retail II Data Wrangling Case Study: From Messy Transactions to Data Gold

## **Struktur Proyek**

```
online-retail-ii-wrangling-1/
│
├── datasets/
│   ├── online_retail_ii_2009-2010.csv.zstd      # Raw dataset (2009–2010)
│   ├── online_retail_ii_2010-2011.csv.zstd      # Raw dataset (2010–2011)
│   └── online-retail-ii-cleaned.csv.zstd        # Cleaned dataset (hasil wrangling)
│
├── notebooks/
│   └── code.ipynb                               # Notebook utama data wrangling
│
├── environment.yml                              # Environment dependencies (conda)
├── README.md                                    # Dokumentasi project
```

## 📌 **Overview**

Proyek ini merupakan studi kasus **data wrangling** pada dataset **Online Retail II** yang bertujuan mengubah data transaksi mentah menjadi dataset analitik yang bersih, terstruktur, dan reusable untuk berbagai proyek data-driven.

Dataset awal mengandung berbagai permasalahan kualitas data seperti missing values, duplikasi, transaksi pembatalan, serta nilai ekstrem pada variabel numerik. Oleh karena itu, dilakukan serangkaian proses data wrangling untuk meningkatkan kualitas dan konsistensi dataset sebelum digunakan dalam analisis lanjutan.

## 📦 **Dataset**

Dataset yang digunakan adalah **Online Retail II** dari UCI Machine Learning Repository.

👉 [https://archive.ics.uci.edu/dataset/502/online+retail+ii](https://archive.ics.uci.edu/dataset/502/online+retail+ii)

Dataset ini berisi transaksi retail online dari perusahaan berbasis di Inggris pada periode **2009–2011** dengan lebih dari **1 juta transaksi**.

## 🎯 **Tujuan Proyek**

Proyek ini bertujuan untuk:

* Mengidentifikasi permasalahan kualitas data pada dataset transaksi retail
* Menerapkan tahapan data wrangling (discovering, structuring, cleaning, enriching, validating)
* Menghasilkan dataset analitik yang bersih dan reusable untuk berbagai proyek data-driven

## 🧠 **Apa itu Data Wrangling**

Data wrangling merupakan proses pembersihan, penataan, dan pengayaan data mentah agar menjadi dataset yang bersih, konsisten, dan siap digunakan untuk analisis, visualisasi, maupun machine learning.

Referensi:
👉 [https://www.ibm.com/think/topics/data-wrangling](https://www.ibm.com/think/topics/data-wrangling)

## ⚙️ **Tools & Libraries**

* Python
* Pandas
* Seaborn
* Matplotlib

## 🔎 **Workflow Data Wrangling**

### 1️⃣ Discovering

* Dataset overview
* Missing values analysis
* Duplicate detection
* Unique value exploration
* Invoice anomaly detection
* Outlier visualization

### 2️⃣ Structuring

* Rename columns
* Type conversion
* Memory optimization

### 3️⃣ Cleaning

* Remove duplicates
* Fill missing Description
* Handle missing CustomerID
* Add guest indicator

### 4️⃣ Enriching

* Feature engineering berbasis waktu
* Business flags (cancellation, adjustment, negative values)
* TotalPrice calculation

### 5️⃣ Validating

* Recheck missing values
* Outlier detection (IQR)
* Final dataset verification

## ✅ **Hasil Akhir**

Dataset akhir:

* 1.033.036 transaksi
* 23 variabel
* Tidak ada missing values
* Struktur data konsisten
* Feature bisnis & temporal lengkap

Dataset disimpan dalam format:

```bash
online-retail-ii-cleaned.csv.zstd
```

## 📘 **Data Dictionary (Cleaned Dataset)**

| Column                | Description                |
| --------------------- | -------------------------- |
| InvoiceID             | ID transaksi               |
| StockCode             | Kode produk                |
| Description           | Nama produk                |
| Quantity              | Jumlah produk              |
| InvoiceDate           | Tanggal transaksi          |
| Price                 | Harga per unit             |
| CustomerID            | ID pelanggan               |
| Country               | Negara pelanggan           |
| IsGuest               | Indikator pelanggan anonim |
| Hour–MonthName        | Feature temporal           |
| IsNegQty / IsNegPrice | Indikator nilai negatif    |
| IsCanceled            | Indikator pembatalan       |
| IsAdjusted            | Indikator penyesuaian      |
| TotalPrice            | Nilai transaksi            |
| IsQuantityOutlier     | Outlier Quantity           |
| IsPriceOutlier        | Outlier Price              |

# 🚀 **Pengembangan Lebih Lanjut**

Dataset hasil wrangling ini dapat digunakan untuk:

| Area                | Ide Proyek             |
| ------------------- | ----------------------- |
| Customer Analytics  | RFM Segmentation        |
| Predictive Modeling | Sales Forecasting       |
| Predictive Modeling | Regression Modeling     |
| Customer Value      | Customer Lifetime Value |
| Recommendation      | Product Recommendation  |
| Market Basket       | Association Rules       |
| Anomaly Detection   | Fraud detection         |
| BI                  | Dashboard interaktif    |
| Geospatial          | Country analysis        |

## 📊 **Key Insight**

Dataset hasil wrangling berfungsi sebagai:

* Analytical dataset
* Gold data layer
* Foundation dataset untuk berbagai proyek data science

## 📚 **References**

* Chen, D. (2012). Online Retail II Dataset — UCI Machine Learning Repository
* IBM Think — What is Data Wrangling