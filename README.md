# Women's Perfume Sales Analysis on eBay
**Data Preprocessing & Exploratory Data Analysis (EDA)**

## Project Overview

Proyek ini bertujuan untuk menganalisis data produk parfum wanita pada marketplace eBay menggunakan Python melalui tahapan **Data Preprocessing** dan **Exploratory Data Analysis (EDA)**.

Analisis dilakukan untuk memahami hubungan antara harga produk (*price*), ketersediaan stok (*available*), dan jumlah produk terjual (*sold*), serta mengidentifikasi karakteristik penjualan berdasarkan merek (*brand*) dan jenis parfum (*type*).

Pendekatan analisis menggunakan konsep penawaran dan permintaan untuk mengeksplorasi pola penjualan, mengidentifikasi produk dengan tingkat penjualan tinggi, serta menghasilkan insight yang dapat mendukung pengambilan keputusan bisnis.

## Dataset

Dataset yang digunakan adalah `ebay_womens_perfume.csv`, yang terdiri dari **1.000 baris dan 10 kolom**, mencakup informasi:

- **Brand & Product:** Nama merek, judul produk, dan jenis parfum.
- **Price:** Harga produk dalam USD.
- **Availability:** Jumlah stok produk yang tersedia.
- **Sales:** Jumlah unit produk yang tercatat terjual.
- **Additional Information:** Informasi ketersediaan, waktu pembaruan, dan lokasi penjual.

## Project Workflow

### 1. Data Understanding & Preprocessing

Melakukan pemeriksaan kualitas data sebelum analisis, meliputi:

- Identifikasi dan penanganan *missing values*.
- Penghapusan data duplikat.
- Perbaikan inkonsistensi penulisan merek dan jenis parfum.
- Standardisasi format dan tipe data.
- Identifikasi outlier menggunakan metode Interquartile Range (IQR).
- Encoding variabel kategorikal.
- Feature engineering untuk menghitung estimasi penjualan dan potensi pendapatan.

### 2. Exploratory Data Analysis (EDA)

Melakukan eksplorasi data menggunakan pendekatan statistik deskriptif dan visualisasi, meliputi:

- **Univariate Analysis:** Menganalisis distribusi harga, stok, dan jumlah produk terjual.
- **Bivariate Analysis:** Membandingkan total penjualan dan potensi pendapatan berdasarkan brand dan jenis parfum.
- **Multivariate Analysis:** Mengeksplorasi hubungan antara harga dan jumlah penjualan berdasarkan brand dan jenis parfum.
- **Correlation Analysis:** Mengukur hubungan antarvariabel numerik dan variabel kategorikal yang telah melalui proses encoding.

## Key Findings

Berdasarkan hasil analisis, diperoleh beberapa temuan utama:

1. **Sales Performance:** Gloria Vanderbilt merupakan brand dengan total unit terjual tertinggi, sedangkan Eau de Parfum menjadi jenis parfum dengan total penjualan tertinggi.
2. **Revenue Potential:** Burberry menunjukkan potensi pendapatan tertinggi berdasarkan brand, sementara Eau de Parfum memiliki potensi pendapatan tertinggi berdasarkan jenis parfum.
3. **Correlation:** Hubungan antara harga, ketersediaan produk, dan jumlah penjualan cenderung lemah. Hal ini menunjukkan bahwa variabel yang dianalisis belum cukup untuk menjelaskan pola penjualan secara menyeluruh.
4. **Data Distribution:** Variabel numerik memiliki distribusi yang cenderung miring ke kanan (*right-skewed*) akibat adanya nilai ekstrem.
5. **Potential Revenue:** Hasil perhitungan pada tahap preprocessing menunjukkan estimasi potensi pendapatan sekitar **USD 571.049**, yang merupakan nilai estimasi berdasarkan data, bukan pendapatan aktual yang telah terealisasi.

## Business Recommendations

Berdasarkan hasil analisis, rekomendasi yang diberikan meliputi:

- Melakukan validasi terhadap produk yang terindikasi sudah tidak dijual (*discontinued*).
- Memprioritaskan evaluasi strategi pemasaran pada brand dan jenis parfum dengan potensi pendapatan tinggi.
- Memanfaatkan informasi harga sebagai pertimbangan awal dalam penyusunan strategi promosi.
- Mempertimbangkan faktor tambahan di luar harga dan ketersediaan stok untuk memahami pola penjualan secara lebih komprehensif.

## Tools & Technologies

- **Python** — Pengolahan dan analisis data.
- **Pandas & NumPy** — Data manipulation dan preprocessing.
- **Matplotlib & Seaborn** — Visualisasi data.
- **Scikit-learn** — Label encoding variabel kategorikal.
- **Jupyter Notebook** — Lingkungan pengembangan dan analisis.

## Conclusion

Proyek ini menunjukkan pentingnya proses data preprocessing untuk meningkatkan kualitas data sebelum dilakukan analisis. Melalui EDA, diperoleh gambaran mengenai distribusi harga, ketersediaan produk, performa penjualan berdasarkan brand dan jenis parfum, serta estimasi potensi pendapatan.

Hasil analisis dapat digunakan sebagai dasar pertimbangan dalam menyusun strategi pemasaran dan penjualan berbasis data. Namun, hubungan antarvariabel yang relatif lemah menunjukkan bahwa diperlukan informasi tambahan untuk menjelaskan faktor-faktor yang memengaruhi penjualan secara lebih mendalam.

---

**Author:** Irwan Lazuardi Saldeni

**Project:** Data Preprocessing & Exploratory Data Analysis — Women's Perfume eBay Dataset
