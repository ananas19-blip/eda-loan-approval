# eda-loan-approval
# 📊 Loan Approval Risk Analysis — Exploratory Data Analysis

## 🧠 Project Overview

Pada proyek ini saya melakukan **Exploratory Data Analysis (EDA)** pada dataset pengajuan pinjaman bank untuk memahami **bagaimana bank menilai risiko kredit calon peminjam**.

Tujuan utama analisis bukan membuat model machine learning, melainkan:

> menemukan pola keputusan approval menggunakan pendekatan analisis data bisnis.

Dataset berisi ±45.000 data pemohon dengan informasi demografi, finansial, dan riwayat kredit.

---

## 🎯 Business Questions

Beberapa pertanyaan yang ingin dijawab:

* Faktor apa yang paling memengaruhi pinjaman disetujui atau ditolak?
* Apakah pendapatan tinggi selalu berarti pinjaman disetujui?
* Seberapa penting riwayat kredit dibanding besar gaji?
* Apakah pengalaman kerja berpengaruh terhadap keputusan bank?
* Bagaimana bank melihat kemampuan bayar pemohon?

---

## 🧹 Data Preparation

Sebelum analisis, dilakukan proses pembersihan data agar insight tidak bias:

**Data Quality Check**

* Tidak ditemukan missing value
* Tidak ditemukan duplikasi
* Standarisasi format kategori

**Handling Outlier (Business Logic Based)**
Beberapa nilai tidak realistis ditemukan (misal umur > 100 tahun atau pengalaman kerja melebihi usia).
Outlier ditangani menggunakan pendekatan logis, bukan sekadar dihapus, agar tetap mencerminkan kondisi dunia nyata.

**Transformasi Data**

* Transformasi log pada income & loan amount untuk mengurangi skew
* Capping nilai ekstrem pada variabel finansial

---

## 📊 Analysis Performed

Analisis difokuskan untuk memahami perilaku keputusan kredit bank:

* Distribusi profil pemohon
* Hubungan pendapatan dan jumlah pinjaman
* Dampak riwayat gagal bayar
* Pengaruh stabilitas pekerjaan
* Pengaruh rasio pinjaman terhadap pendapatan
* Hubungan panjang riwayat kredit dengan approval

---

## 🔍 Key Findings

### 1. Approval bukan ditentukan oleh gaji saja

Pemohon berpendapatan tinggi tetap bisa ditolak jika rasio pinjaman terlalu besar.

### 2. Riwayat kredit adalah faktor terkuat

Nasabah dengan riwayat gagal bayar memiliki kemungkinan penolakan jauh lebih tinggi dibanding faktor lain.

### 3. Bank menilai kemampuan bayar, bukan jumlah pinjaman

### 4. Stabilitas finansial meningkatkan kepercayaan

Pengalaman kerja dan panjang riwayat kredit meningkatkan peluang disetujui.

---

## 💡 Business Insight

Bank menggunakan pendekatan **risk-based lending**.

Artinya keputusan tidak berdasarkan satu faktor, tetapi kombinasi:

> kemampuan bayar + kebiasaan finansial + histori kredit

Sehingga approval lebih mencerminkan **perilaku finansial pemohon**, bukan hanya kondisi saat ini.

---

## 🛠️ Tools

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn

---

## 📁 Output

* Data cleaning process
* Exploratory analysis
* Risk interpretation
* Business insights

---

## 👤 Author

Portfolio Project — Data Analytics
