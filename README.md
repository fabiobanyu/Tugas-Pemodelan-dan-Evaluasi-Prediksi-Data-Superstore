# Tugas Pemodelan dan Evaluasi Prediksi – Dataset Superstore  
**Mata Kuliah:** Artificial Intelligence  
**Nama:** Fabio Banyu Cyto (123450104)

---

<div align="center">

### 📘 *“Machine Learning Classification for Profit Prediction using Superstore Dataset”*  
Mengimplementasikan model klasifikasi untuk memprediksi apakah suatu transaksi menghasilkan **profit** atau **loss**, melalui proses end-to-end mulai dari preprocessing, modeling, hingga evaluasi.

</div>

---

## 📌 Deskripsi Tugas
Repository ini berisi proses lengkap dalam melakukan **pemodelan klasifikasi** pada **Dataset Superstore**, dimulai dari penentuan tujuan penelitian, penetapan variabel target, pembersihan data, eksplorasi data, pemilihan model, hingga evaluasi performa. Tugas ini dikembangkan melalui diskusi terstruktur bersama rekan kelompok untuk menentukan variabel target yang paling tepat, model yang paling sesuai, serta landasan ilmiah dari pemilihan tersebut.

---

## 🎯 Tujuan Penelitian  
Tujuan utama dari penelitian ini adalah:

### **“Membangun model klasifikasi untuk memprediksi apakah suatu penjualan menghasilkan profit atau tidak.”**

Variabel target yang digunakan adalah:

### **`ProfitStatus`**
- **1 = Profit / Menguntungkan**  
- **0 = Loss / Merugi**

**Alasan pemilihan target ini:**  
- Penentuan sangat **sederhana dan langsung**, hanya membandingkan nilai profit.
- Relevan secara bisnis dan **dapat diterapkan untuk rekomendasi operasional**.
- Tidak menimbulkan bias seperti region atau kategori produk.
- Cocok untuk **model-model klasifikasi dasar hingga menengah**.

---

## 📂 Dataset Superstore  
Dataset Superstore merupakan data penjualan retail populer yang terdiri dari informasi transaksi seperti:

- **Order Date**  
- **Ship Mode**  
- **Customer Segment**  
- **Category & Sub-Category**  
- **Sales**  
- **Discount**  
- **Quantity**  
- **Profit**  
- **Region**  
- **City**  
- **State**

Dataset ini digunakan untuk:  
- Mengklasifikasikan apakah transaksi menghasilkan profit atau loss  
- Mengidentifikasi pola transaksi yang menyebabkan kerugian  
- Memberikan insight bisnis yang dapat membantu strategi penjualan

---

## 🧹 Tahap Pembersihan dan Persiapan Data  
Tahapan preprocessing yang dilakukan mencakup:

- Mengonversi nilai profit menjadi kategori **profit/loss (`ProfitStatus`)**
- Encoding variabel kategori (LabelEncoder/OneHot)
- Menghapus data duplikat  
- Menangani outlier jika diperlukan  
- Normalisasi fitur numerik (MinMaxScaler / StandardScaler)

Proses ini penting agar model dapat belajar dengan lebih efektif dan menghasilkan prediksi yang stabil.

---

## 📊 Pemodelan Klasifikasi  
Model yang digunakan pada penelitian ini dipilih karena:

- **Mudah digunakan**
- Cocok untuk dataset tabular**
- Performa baik pada data klasifikasi**
- Mudah dipahami hasil dan karakteristiknya

### **Model yang digunakan:**

#### 1. 🌲 **XGBoost**  
#### 2. 🌳 **Random Forest Classifier**  
#### 3. ➗ **Logistic Regression**  

---

## 🧪 Evaluasi Model  
Untuk mengukur performa ketiga model, digunakan metrik evaluasi berikut:

- 🎯 **Accuracy** — tingkat keseluruhan prediksi yang benar  
- 🎯 **Precision** — akurasi model dalam memprediksi kelas profit  
- 🎯 **Recall** — kemampuan model menemukan semua instance profit  
- 🎯 **F1-Score** — keharmonisan antara precision dan recall  
- 🎯 **Confusion Matrix** — visualisasi prediksi benar/salah per kelas  
