# Prediksi Customer Churn - Telco

Proyek Machine Learning untuk memprediksi pelanggan yang berpotensi *churn* (berhenti berlangganan) pada perusahaan telekomunikasi.

---

## 📌 Unduh Dataset
> **Wajib:** Sebelum menjalankan proyek ini, Anda harus mengunduh dataset terlebih dahulu.

1. Unduh dataset didalam github.
2. Simpan file CSV di folder utama proyek ini.

---

## 🚀 Cara Menjalankan

### 1. Clone & Install Dependensi
```bash
git clone (https://github.com/yahyaabdulloh28/project_churntelco.git)
cd telco-churn-prediction
pip install -r requirements.txt
```

### 2. Jalankan Notebook
```bash
jupyter notebook telco_churn.ipynb
```

---

## ⚙️ Ringkasan Workflow

1. **Pembersihan Data:** Memperbaiki *missing values* pada `TotalCharges` & menghapus `customerID`.
2. **Encoding:** Menggunakan One-Hot Encoding (`drop_first=True`) untuk fitur kategorikal & ubah `Churn` ke $1$/$0$.
3. **Split Data:** Membagi data *Train* & *Test* ($80/20$).
4. **Resampling:** Penanganan *class imbalance* menggunakan **SMOTE** (hanya pada data *train*).
5. **Pemodelan:** Membandingkan Logistic Regression, Random Forest, dan XGBoost dengan fokus metrik **Recall** & **ROC-AUC**.

---

## 📦 Pustaka yang Dibutuhkan (`requirements.txt`)
```text
pandas
numpy
scikit-learn
imbalanced-learn
xgboost
matplotlib
seaborn
jupyter
```
