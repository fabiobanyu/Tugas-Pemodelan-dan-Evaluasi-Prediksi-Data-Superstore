<div align="center">

# 📘 Machine Learning: Superstore Profit Prediction
**Tugas Besar — Pemodelan & Evaluasi Prediksi** *Mata Kuliah: Artificial Intelligence | Kelompok 3*

![Python](https://img.shields.io/badge/Python-3.9%2B-blue?style=for-the-badge&logo=python&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-FL-red?style=for-the-badge&logo=xgboost&logoColor=white)
![Status](https://img.shields.io/badge/Status-Active-success?style=for-the-badge)

<p align="center">
  <b>Mengimplementasikan model klasifikasi end-to-end untuk memprediksi profitabilitas transaksi retail.</b>
</p>

</div>

---

## 👨‍💻 Tim Penyusun
Berikut adalah anggota **Kelompok 3** yang berkontribusi dalam penelitian ini:

| No | Nama Anggota | NIM |
|:--:|:---|:---:|:---|
| 1 | **Fabio Banyu Cyto** | `123450104` |
| 2 | **Gusti Putu Ferazka D.** | `123450046` |
| 3 | **Aliya Amara Ananta** | `123450075` |
| 4 | **Hafsa Fazila Arradhi** | `123450079` |

---

## 📌 Deskripsi Proyek
Repository ini berisi proses lengkap dalam melakukan **pemodelan klasifikasi** pada **Dataset Superstore**, dimulai dari penentuan tujuan penelitian, penetapan variabel target, pembersihan data, eksplorasi data, pemilihan model, hingga evaluasi performa. Tugas ini dikembangkan melalui diskusi terstruktur bersama rekan kelompok untuk menentukan variabel target yang paling tepat, model yang paling sesuai, serta landasan ilmiah dari pemilihan tersebut.

> **Highlight:** Tugas ini dikembangkan melalui diskusi terstruktur untuk memastikan pemilihan model dan metode evaluasi memiliki landasan ilmiah yang kuat.

---

## 🎯 Tujuan Penelitian
Fokus utama dari penelitian ini adalah:

### *"Membangun model klasifikasi untuk memprediksi apakah suatu transaksi penjualan akan menghasilkan PROFIT atau LOSS."*

### 🏷️ Variabel Target: `ProfitStatus`
Kami mentransformasi variabel numerik `Profit` menjadi variabel kategorikal biner:

| Label | Kelas | Deskripsi |
|:---:|:---:|:---|
| **1** | **Profit** | Transaksi Menguntungkan 📈 |
| **0** | **Loss** | Transaksi Merugi 📉 |

**Mengapa Target Ini Dipilih?**
* ✅ **Simple & Direct**: Representasi langsung dari kesehatan finansial transaksi.
* ✅ **Actionable**: Hasil prediksi dapat digunakan untuk mencegah transaksi yang berpotensi rugi.
* ✅ **Unbiased**: Menghindari bias demografis (seperti Region atau Customer Segment).

---

## 📂 Tentang Dataset
Dataset ini memuat informasi detail transaksi ritel. Fitur-fitur utama meliputi:

<details>
<summary><b>Klik untuk melihat detail fitur</b></summary>

* **Waktu & Pengiriman**: `Order Date`, `Ship Mode`
* **Pelanggan**: `Customer Segment`
* **Produk**: `Category`, `Sub-Category`
* **Metrik Keuangan**: `Sales`, `Quantity`, `Discount`, `Profit`
* **Lokasi**: `Region`, `City`, `State`

</details>

---

## ⚙️ Metodologi & Preprocessing
Agar model dapat bekerja optimal, kami melakukan tahapan berikut:

1.  **Target Engineering**: Konversi `Profit` $\rightarrow$ `ProfitStatus` (0/1).
2.  **Cleaning**: Penghapusan duplikat dan penanganan *missing values*.
3.  **Encoding**: Mengubah data kategori (teks) menjadi angka menggunakan *LabelEncoder* atau *OneHotEncoder*.
4.  **Scaling**: Normalisasi fitur numerik menggunakan *MinMaxScaler/StandardScaler*.

---

## 🧠 Model Klasifikasi
Kami membandingkan tiga algoritma populer untuk menentukan performa terbaik:

### 1. 🌲 XGBoost (Extreme Gradient Boosting)
> Dipilih karena performanya yang sangat tinggi dalam menangani data tabular dan kemampuannya menangani pola kompleks.

### 2. 🌳 Random Forest Classifier
> Model *ensemble* yang kuat terhadap *overfitting* dan memberikan wawasan mengenai *Feature Importance*.

### 3. ➗ Logistic Regression
> Digunakan sebagai *baseline model* karena kesederhanaannya dan kemudahan interpretasi (Explainability).

---

## 🧪 Metrik Evaluasi
Performa model diukur menggunakan parameter berikut:

* 🎯 **Accuracy**: Seberapa sering model memprediksi dengan benar secara keseluruhan.
* ⚖️ **Precision**: Seberapa akurat model saat memprediksi kelas "Profit".
* 🔍 **Recall**: Seberapa baik model menemukan seluruh data yang benar-benar "Profit".
* 🎼 **F1-Score**: Rata-rata harmonis antara Precision dan Recall (penting jika data tidak seimbang).
* 🔲 **Confusion Matrix**: Peta detail kesalahan prediksi (False Positive vs False Negative).

---

<div align="center">
  <small>Copyright © 2024 Kelompok 3 Artificial Intelligence. All Rights Reserved.</small>
</div>
