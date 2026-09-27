# Statprob-Proyek-1-EDA

Repositori ini disusun untuk memenuhi tugas Proyek 1: Eksplorasi Data. Fokus dari proyek ini adalah melakukan pengenalan awal terhadap data (Exploratory Data Analysis / EDA) yang meliputi pemahaman struktur data, pengecekan data kosong, statistik deskriptif, serta visualisasi data awal tanpa menggunakan uji hipotesis atau machine learning.

## Anggota Kelompok (Kelompok 15)
- Ali Riza Alayubi (NRP: 5027261020)
- Farras Ananda Pramana (NRP: 5027261068)
- Maghfur Nara (NRP: 5027261129)

## Informasi Dataset
- Topik Project: Smart City 
- Sumber Dataset: Air Quality Index in Jakarta (Taufiq Pohan, Daily Air Quality Index (AQI) in Jakarta from January 2010 - February 2025) 
- Link Dataset: "https://www.kaggle.com/datasets/senadu34/air-quality-index-in-jakarta-2010-2021"
- Ukuran Dataset: 5538 baris dan 10 kolom
- Lisensi: Database Contents License (DbCL) v1.0 "https://opendatacommons.org/licenses/dbcl/1-0/"
- Kamus Data:

| Kolom | Arti / Deskripsi | Jenis Variabel | Satuan |
|---|---|---|---|
| `tanggal` | Tanggal pencatatan kualitas udara | Kategorial (Interval/Waktu) | Tanggal |
| `stasiun` | Lokasi stasiun pemantauan kualitas udara | Kategorial (Nominal) | — |
| `pm25` | Konsentrasi partikulat udara berukuran ≤ 2,5 mikrometer | Numerik (Rasio) | µg/m³ |
| `pm10` | Konsentrasi partikulat udara berukuran ≤ 10 mikrometer | Numerik (Rasio) | µg/m³ |
| `so2` | Konsentrasi sulfur dioksida di udara | Numerik (Rasio) | µg/m³ |
| `co` | Konsentrasi karbon monoksida di udara | Numerik (Rasio) | µg/m³ |
| `o3` | Konsentrasi ozon di udara | Numerik (Rasio) | µg/m³ |
| `no2` | Konsentrasi nitrogen dioksida di udara | Numerik (Rasio) | µg/m³ |
| `max` | Nilai maksimum indeks kualitas udara pada hari tersebut | Numerik (Rasio) | ISPU |
| `critical` | Parameter pencemar yang menjadi parameter kritis/dominan | Kategorial (Nominal) | — |

## Tahap Pengerjaan
1. Cek anggota Kelompok yang tergabung di Kelompok 15 melalui [Tautan Pembagian Kelompok EDA Kelas B dan C](https://docs.google.com/spreadsheets/d/1DYGqZP-cE1R45a5qWif2PWlgk_qH0jmYWobGNppLXaE/edit?gid=698955458#gid=698955458).
2. Membuat Group komunikasi dengan anggota yang terdaftar di kelompok 15 kelas B.
3. Menentukan topik dan cari dataset di Kaggle yang memenuhi kriteria (minimal 200 baris, 5 kolom, format CSV/Excel di bawah 25 MB).
4. Mengintall dan menggunakan anaconda dan jupyter notebook lalu menyiapkan lingkungan lokal secara mandiri tanpa asisten AI, agar terbiasa menggunakan sintaks Python.
5. Melakukan eksplorasi data, pengecekan nilai kosong, statistik deskriptif, dan visualisasi grafik sesuai struktur yang ditentukan.
6. Mengunggah notebook (.ipynb), dataset, dan berkas README.md ini ke repositori kelompok, lalu mengumpulkan tautannya di myITS Learning.
7. Demo di Kelas (Minggu ke-5): Menjalankan notebook di depan kelas dan menjawab pertanyaan dosen pengampu.

##  Panduan Instalasi & Menjalankan Jupyter Notebook (Lokal)
1. Unduh installer dari halaman instalasi Miniconda. Untuk Windows, pilih opsi Just Me dan gunakan pengaturan bawaan.
2. Buat environment untuk mata kuliah ini
   Buka **Anaconda Prompt** (untuk Windows) atau **Terminal** (untuk macOS/Linux), lalu jalankan perintah berikut untuk membuat *environment* baru bernama `statprob`:
   ```bash
   conda create -n statprob python=3.11 -y
   conda activate statprob
   ```
3. Instal paket yang dibutuhkan
   ```bash
   conda install -c conda-forge jupyter pandas matplotlib seaborn -y
   ```
4. Jalankan Jupyter Notebook
   Masuk ke folder proyek kalian, lalu jalankan Jupyter. Browser akan terbuka otomatis.
   ```bash
   cd lokasi/folder/proyek1
   jupyter notebook
   ```
   Buat notebook baru lewat menu New, lalu pilih Python 3. Setiap kali membuka Anaconda Prompt lagi, jalankan `conda activate statprob` sebelum `jupyter notebook`.
