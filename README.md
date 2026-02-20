# online-retail-ii-wrangling-1
Online Retail II Data Wrangling

Dataset Reference: https://archive.ics.uci.edu/dataset/502/online+retail+ii

## Data Specification

| Column | Description | Sample |
|---|---|---|
| **InvoiceID** | Nomor invoice untuk setiap transaksi. Umumnya berupa angka 6 digit unik dan dapat diawali huruf **“C”** yang menandakan transaksi pembatalan. Digunakan untuk mengidentifikasi dan mengelompokkan item dalam satu transaksi. | 536365 |
| **StockCode** | Kode produk atau item yang mengidentifikasi setiap produk secara unik. Biasanya berupa angka 5 digit atau kombinasi alfanumerik yang merepresentasikan item tertentu. | 85123A |
| **Description** | Nama atau deskripsi produk dalam bentuk teks yang menjelaskan item pada baris transaksi. Nilai dapat kosong pada beberapa kasus data. | WHITE HANGING HEART T-LIGHT HOLDER |
| **Quantity** | Jumlah unit produk pada setiap baris transaksi dalam bentuk numerik. Nilai positif menunjukkan pembelian, sedangkan nilai negatif dapat mengindikasikan pengembalian atau pembatalan item. | 6 |
| **InvoiceDate** | Tanggal dan waktu saat transaksi dibuat dalam format datetime. Kolom ini merepresentasikan waktu terjadinya transaksi. | 2010-12-01 08:26:00 |
| **Price** | Harga per unit produk dalam bentuk numerik (float). Nilai ini merupakan harga item sebelum dikalikan dengan Quantity. | 2.55 |
| **CustomerID** | Nomor pelanggan yang mengidentifikasi customer secara unik. Biasanya berupa angka 5 digit dan dapat bernilai kosong jika pelanggan tidak teridentifikasi. | 17850 |
| **Country** | Nama negara tempat pelanggan berdomisili dalam bentuk kategorikal teks. Digunakan untuk menunjukkan lokasi pelanggan. | United Kingdom |
| **IsGuest** | Flag boolean yang menunjukkan transaksi tanpa CustomerID. Nilai True menandakan pelanggan tidak teridentifikasi. | False |
| **IsQuantityOutlier** | Flag boolean yang menandai apakah nilai Quantity terdeteksi sebagai outlier berdasarkan proses analisis data. | False |
| **IsPriceOutlier** | Flag boolean yang menandai apakah nilai Price terdeteksi sebagai outlier berdasarkan proses analisis data. | False |
| **Hour** | Jam transaksi dalam bentuk numerik yang diturunkan dari InvoiceDate. | 8 |
| **Year** | Tahun transaksi dalam bentuk numerik yang diturunkan dari InvoiceDate. | 2010 |
| **Month** | Bulan transaksi dalam bentuk numerik (1–12) yang diturunkan dari InvoiceDate. | 12 |
| **Day** | Hari dalam bulan transaksi dalam bentuk numerik yang diturunkan dari InvoiceDate. | 1 |
| **Week** | Minggu dalam tahun transaksi dalam bentuk numerik yang diturunkan dari InvoiceDate. | 48 |
| **DayName** | Nama hari transaksi dalam bentuk teks yang diturunkan dari InvoiceDate. | Wednesday |
| **MonthName** | Nama bulan transaksi dalam bentuk teks yang diturunkan dari InvoiceDate. | December |
| **IsNegQty** | Flag boolean yang menunjukkan Quantity bernilai negatif. | False |
| **IsNegPrice** | Flag boolean yang menunjukkan Price bernilai negatif. | False |
| **IsCanceled** | Flag boolean yang menunjukkan transaksi pembatalan, umumnya berdasarkan InvoiceID yang diawali huruf “C”. | False |
| **IsAdjusted** | Flag boolean yang menandakan baris transaksi merupakan hasil penyesuaian atau koreksi data. | False |
| **TotalPrice** | Nilai total baris transaksi yang merupakan hasil perkalian Quantity dan Price. | 15.30 |