# EKSPERIMEN MODEL REGRESI UNTUK PREDIKSI CUSTOMER LIFETIME VALUE PADA SEBUAH PERUSAHAAN ASURANSI KENDARAAN

### **Gambaran Umum**
Proyek ini berfokus pada pengembangan model prediksi Customer Lifetime Value (CLV) berbasis machine learning untuk perusahaan asuransi kendaraan. CLV adalah metrik penting untuk memahami nilai jangka panjang pelanggan dan mengoptimalkan sumber daya pemasaran. 

Pendekatan non-parametrik seperti Random Forest dan XGBoost dipilih untuk menangani tantangan data multikolinearitas. Dengan model yang lebih canggih dibandingkan sistem berbasis aturan, diharapkan dapat meningkatkan akurasi prediksi, efisiensi operasional, dan profitabilitas perusahaan.

---

### **Pemahaman Permasalahan Bisnis**
**Latar Belakang:**  
- Sistem berbasis rule-based memiliki MAE sebesar $4161.14.
- Prediksi CLV yang tidak akurat dapat menyebabkan kerugian besar akibat alokasi sumber daya yang salah.
- CLV yang ideal memiliki rasio CLV-to-CAC minimal 3:1, sehingga penting untuk membangun model yang andal.
- Algoritma machine learning, khususnya Random Forest, menawarkan solusi untuk menangkap pola kompleks dalam data dan memberikan prediksi yang lebih akurat.

**Stakeholder:**  
1. **Tim Keuangan:** Meningkatkan profitabilitas.
2. **Tim Manajemen Produk:** Merancang produk berdasarkan wawasan CLV.
3. **Tim Data Science:** Membuat model prediktif.
4. **Tim Pemasaran:** Mengarahkan strategi berdasarkan analisis CLV.

**Tujuan:**  
1. Meningkatkan akurasi prediksi CLV dibandingkan sistem rule-based (MAE: $4161.14).
2. Memahami fitur penting seperti premi bulanan dan klaim.
3. Memanfaatkan hyperparameter tuning untuk performa optimal
4. Meningkatkan efisiensi pengambilan keputusan untuk divisi pemasaran.

---

### **Pendekatan Analitik**
**Tahapan Analisis:**
1. **Preprocessing Data:**
   - Menangani nilai yang hilang (missing values).
   - Encoding fitur kategorikal.
   - Normalisasi data numerik.

2. **Benchmarking Model:**
   - Evaluasi algoritma regresi seperti Linear Regression, Random Forest, dan XGBoost.

3. **Hyperparameter Tuning:**
   - Optimasi parameter seperti `n_estimators`, `max_depth`, dan `min_samples_split` pada model Random Forest.

4. **Evaluasi Model:**
   - Menggunakan metrik evaluasi: MAE, RMSE, MAPE, dan R-Squared.

---

### **Hasil Eksperimen**
- **Model Terbaik:** Random Forest.  
  - MAE: $382.38  
  - RMSE: $995.20  
  - MAPE: 4.35%  
  - R²: 0.911 (meningkatkan akurasi hingga 91.1%).
- **Fitur Penting:**  
  1. Number of Policies (60.44%)  
  2. Monthly Premium Auto (33.07%)  
  3. Total Claim Amount (2.07%)  
  4. Income (1.91%).
 
- **Peningkatan Kinerja:**
  1. Error MAE model Random Forest berkurang $3778.76 dibandingkan sistem berbasis aturan.
  2. Perusahaan berpotensi mengurangi kerugian hingga 47.6%.

---

### **Rekomendasi**

**Untuk Model:**
1. **Eksplorasi Data Tambahan:** Tambahkan data pelanggan seperti *Policy Type* atau *Sales Channel* untuk meningkatkan akurasi model.
2. **Identifikasi Outlier:** Analisis pelanggan dengan error prediksi tinggi (CLV > $8000) untuk mengidentifikasi pola unik.
3. **Eksperimen Model Lain:** Coba algoritma seperti Support Vector Regression (SVR) atau Neural Networks.
4. **Pemantauan Kinerja:** Lakukan validasi berkala untuk memastikan akurasi model tetap optimal.

**Untuk Bisnis:**
1. **Segmentasi Pelanggan:** Gunakan prediksi CLV untuk mengelompokkan pelanggan berdasarkan nilai potensial mereka.
2. **Personalisasi Penawaran:** Fokuskan upaya pemasaran pada pelanggan bernilai tinggi dengan penawaran yang sesuai.
3. **Strategi Upselling dan Cross-Selling:** Tingkatkan pendapatan dari pelanggan dengan nilai prediksi CLV tinggi melalui produk tambahan.
4. **Pengembangan Program Loyalitas:** Buat program loyalitas berbasis CLV untuk meningkatkan retensi pelanggan.
---

### **Kesimpulan**
Model Random Forest terbukti menjadi solusi terbaik untuk prediksi CLV dalam proyek ini. Dengan pengurangan error yang signifikan dan kontribusi fitur yang relevan, model ini memberikan nilai bisnis yang besar bagi perusahaan asuransi kendaraan. Integrasi prediksi CLV dengan sistem CRM perusahaan dapat membuka peluang untuk retensi pelanggan yang lebih baik, peningkatan loyalitas, dan optimalisasi strategi pemasaran.


