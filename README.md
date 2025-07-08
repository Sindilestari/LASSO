## 📌 Latar Belakang
Overfitting merupakan masalah umum dalam model regresi logistik ketika jumlah variabel prediktor cukup banyak. Oleh karena itu, regularisasi LASSO digunakan untuk mengatasi overfitting sekaligus melakukan seleksi variabel pada data Breast Cancer Wisconsin.

## 🧪 Metode
- Model: Regresi Logistik Biner dengan Regularisasi LASSO
- Proses seleksi variabel dilakukan dengan meminimalkan fungsi deviance binomial yang ditambah penalti L1
- Pemilihan nilai penalti (λ) dilakukan melalui 10-fold Cross Validation

## 🛠️ Tools
- R Programming Language
- RStudio IDE
- Library: `glmnet`, `caret`, `dplyr`, `ggplot2`

## 📊 Hasil Evaluasi
- Nilai deviance binomial minimum: **0.2116** pada λ = **0.004394**
- Model akhir memilih **13 dari 30 variabel** dengan koefisien tidak nol
- Hasil menunjukkan peningkatan akurasi dan reduksi kompleksitas model dibandingkan regresi logistik tanpa penalti

## 📁 Isi Repository
- `Regresi terpenalti`: Script utama analisis
- `README.md`: Deskripsi proyek

## 🔍 Catatan
Dataset diperoleh dari [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+(Diagnostic)) dan digunakan hanya untuk keperluan akademik.
