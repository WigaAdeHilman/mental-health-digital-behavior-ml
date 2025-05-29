# 💡 Mental Health & Digital Behavior — Machine Learning Projects

Proyek ini terdiri dari tiga analisis machine learning yang membahas hubungan antara **perilaku digital** dan **kesehatan mental**, menggunakan satu dataset yang sama. Pendekatan yang digunakan meliputi **regresi**, **klasifikasi**, dan **clustering**.

---

## 📊 Dataset Overview

Dataset mencakup variabel-variabel yang merepresentasikan perilaku penggunaan perangkat digital dan kondisi mental, di antaranya:

- `daily_screen_time_min`: Durasi penggunaan layar per hari (menit)
- `num_app_switches`: Jumlah perpindahan aplikasi
- `sleep_hours`: Jam tidur per hari
- `notification_count`: Jumlah notifikasi yang diterima
- `social_media_time_min`: Waktu untuk media sosial (menit)
- `focus_score`, `mood_score`: Skor subjektif dari pengguna
- `anxiety_level`: Level kecemasan (rendah, sedang, tinggi)
- `digital_wellbeing_score`: Indeks keseluruhan kesejahteraan digital

---

## 🧠 Proyek 1 — Digital Wellbeing Regression

> **Tujuan:** Memprediksi skor kesejahteraan digital menggunakan fitur perilaku digital.

- 📈 Algoritma: **Linear Regression**
- ⚙️ Fitur: Semua kolom kecuali target (`digital_wellbeing_score`)
- 🧪 Evaluasi:
  - MAE: ~0.15
  - RMSE: ~0.18
  - R²: ~1.00 (sangat baik)

📁 Notebook: `01_digital_wellbeing_regression.ipynb`

---

## 🧪 Proyek 2 — Anxiety Level Classification

> **Tujuan:** Mengklasifikasikan tingkat kecemasan pengguna menjadi *Rendah*, *Sedang*, atau *Tinggi*.

- 🔍 Algoritma yang dibandingkan:
  - Decision Tree
  - Logistic Regression
  - Support Vector Machine (SVM)
  - K-Nearest Neighbors (KNN)
- 🧠 Fitur: Semua kolom kecuali `anxiety_level`
- 📊 Evaluasi: Akurasi, Confusion Matrix, Cross-Validation

📁 Notebook: `02_anxiety_level_classification.ipynb`

---

## 🔍 Proyek 3 — Clustering Tipe Pengguna Digital

> **Tujuan:** Mengelompokkan pengguna berdasarkan kebiasaan digital.

- 🧭 Algoritma: **K-Means Clustering**
- 📌 Fitur: 
  - `daily_screen_time_min`
  - `num_app_switches`
  - `social_media_time_min`
  - `notification_count`
- 🔍 Hasil:
  - 5 klaster: "Pengguna Berat", "Pengguna Sosial", "Pengguna Seimbang", dll.
  - Visualisasi: PCA 2D, Radar Chart, Profil Klaster

📁 Notebook: `03_Clustering_Tipe_Pengguna_Digital.ipynb`

---

## 🛠️ Teknologi & Library

- Python
- Scikit-learn
- Pandas & NumPy
- Seaborn & Matplotlib
- Jupyter Notebook

---

## 📁 Struktur Repositori

├── 01_digital_wellbeing_regression.ipynb
├── 02_anxiety_level_classification.ipynb
├── 03_Clustering_Tipe_Pengguna_Digital.ipynb
├── Dataset/mental_health_digital_behavior_data.csv
└── README.md