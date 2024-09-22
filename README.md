# Capstone Modul  3 : Telco Customer Churn Prediction

## Introduction

Salah satu tantangan utama yang dihadapi perusahaan telekomunikasi Telco adalah customer churn, yaitu ketika customer berhenti berlangganan dan beralih ke penyedia layanan lain. Upaya retensi menjadi hal yang harus diprioritaskan karena biaya akuisisi customer baru seringkali lebih besar dibandingkan biaya retensi customer (bisa 5-25 kali lebih mahal).

### Objectives

1. **Data Understanding**: Menganalisis dataset untuk memahami perilaku pelanggan dan mengidentifikasi fitur kunci yang mempengaruhi churn.
2. **Data Preparation**: Membuat fitur baru yang dapat meningkatkan kemampuan prediktif model.
3. **Data Analysis**: Melatih dan mengevaluasi beberapa model klasifikasi, termasuk Naive Bayes, AdaBoost, dan XGBoost, untuk menentukan yang terbaik.
4. **Model Evaluation**: Menggunakan metrik yang sesuai (seperti recall dan precision) untuk menilai kinerja model, terutama pada kelas yang tidak seimbang.
5. **Recommendation**: Memberikan rekomendasi berdasarkan hasil evaluasi model untuk meningkatkan strategi retensi pelanggan.

### Dataset

Dataset yang digunakan untuk proyek ini berisi berbagai atribut pelanggan, termasuk informasi demografis, penggunaan layanan, dan data historis churn. Tujuan utama adalah memprediksi apakah seorang pelanggan akan churn berdasarkan atribut-atribut ini.

### Tools and Technologies

- Pandas, Numpy, Seaborn, Matplotlib
- MinMaxScaler, OneHotEncoder, OrdinalEncoder
- SMOTE, SelectKBEST
- Scikit-learn
- XGBoost, CatBoost, AdaBoost, LGBM
- Voting Classifier
- cross_val_score, Pipeline, ImbPipeline

### Result
<img width="416" alt="Screenshot 2024-09-22 at 12 05 15" src="https://github.com/user-attachments/assets/f0c3208a-83b5-42d6-bffc-472bca18b23b">

**Model AdaBoost** dengan feature selection sebanyak 15 (**SelectKBest**) dan **SMOTE sampling** menunjukkan performa yang menjanjikan dalam memprediksi kemungkinan pelanggan akan churn. Setelah melalui tahap data preprocessing dan hyperparameter tuning, model ini hanya menggunakan fitur-fitur yang paling relevan dan mencapai **nilai recall sebesar 88%**.
