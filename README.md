# 🎵 Analisis Data Spotify

Proyek analisis data untuk mengeksplorasi popularitas musik dan karakteristik audio lagu Spotify menggunakan Python dan Exploratory Data Analysis (EDA).

## 📌 Tentang Proyek

Proyek ini menganalisis dataset yang berisi **114.000 lagu Spotify** dari berbagai genre musik.

Analisis dilakukan untuk mengeksplorasi pola popularitas lagu, karakteristik audio, konten eksplisit, serta hubungan antarfitur audio.

Proses analisis terdiri dari beberapa tahapan, yaitu pemahaman data, pembersihan data, feature engineering, dan exploratory data analysis (EDA).

## 🎯 Tujuan Analisis

- Mengidentifikasi genre musik dengan rata-rata popularitas tertinggi.
- Mengeksplorasi karakteristik audio pada lagu dengan tingkat popularitas yang berbeda.
- Menganalisis hubungan antara konten eksplisit dan popularitas lagu.
- Menganalisis hubungan antara konten eksplisit dan danceability.
- Mengeksplorasi hubungan antarfitur audio Spotify menggunakan analisis korelasi.

## 📊 Dataset

Dataset terdiri dari **114.000 lagu Spotify** dari berbagai genre musik.

Dataset mencakup informasi mengenai:

- Informasi lagu dan artis
- Genre musik
- Popularitas
- Konten eksplisit
- Danceability
- Energy
- Loudness
- Acousticness
- Instrumentalness
- Liveness
- Valence
- Tempo
- Durasi lagu

## 🔍 Tahapan Analisis

### 1. Pemahaman Data

Dataset dieksplorasi untuk memahami struktur dan karakteristik data melalui:

- Dimensi dataset
- Tipe data
- Statistik deskriptif
- Nilai unik
- Identifikasi nilai yang hilang
- Deteksi outlier
- Deteksi data duplikat

### 2. Pembersihan Data

Beberapa tahapan pembersihan data yang dilakukan meliputi:

- Menangani nilai yang hilang.
- Mendeteksi dan menangani outlier menggunakan IQR Capping (Winsorization).
- Menghapus data duplikat.
- Menormalisasi data kategorikal dengan mengubah teks menjadi huruf kecil dan menghapus spasi yang tidak diperlukan.
- Memverifikasi tipe data dan kualitas data setelah proses pembersihan.

### 3. Feature Engineering

Beberapa fitur baru dibuat untuk mendukung proses analisis:

- `duration_min` — mengubah durasi lagu dari milidetik menjadi menit.
- `popularity_category` — mengelompokkan lagu menjadi Low, Medium, dan High berdasarkan kuantil.
- `tempo_category` — mengelompokkan tempo menjadi Slow, Medium, dan Fast berdasarkan kuantil.
- `explicit_encoded` — mengubah nilai explicit dari format boolean menjadi nilai numerik (0/1).

### 4. Exploratory Data Analysis (EDA)

Analisis eksploratif yang dilakukan meliputi:

- Distribusi lagu berdasarkan genre musik.
- 10 genre dengan jumlah lagu terbanyak.
- 10 genre dengan rata-rata popularitas tertinggi.
- Distribusi popularitas lagu.
- Perbandingan popularitas lagu eksplisit dan non-eksplisit.
- Perbandingan danceability berdasarkan konten eksplisit.
- Profil karakteristik audio berdasarkan kategori popularitas.
- Hubungan antara energy dan danceability.
- Hubungan antara energy dan valence.
- Analisis korelasi antarfitur audio numerik.

## 💡 Hasil dan Insight

- Dataset terdiri dari 114.000 lagu yang mencakup berbagai genre musik.
- Terdapat perbedaan rata-rata popularitas pada berbagai genre musik.
- Lagu dengan tingkat popularitas tinggi menunjukkan karakteristik audio yang berbeda dibandingkan dengan lagu pada kategori popularitas yang lebih rendah.
- Lagu eksplisit dan non-eksplisit menunjukkan perbedaan dalam distribusi popularitas dan danceability.
- `energy` dan `loudness` memiliki korelasi positif yang kuat (r ≈ 0,76).
- `energy` dan `acousticness` memiliki korelasi negatif yang kuat (r ≈ -0,73).
- `valence` dan `danceability` memiliki hubungan positif sedang.
- `popularity` tidak menunjukkan korelasi linear yang kuat dengan masing-masing fitur audio, sehingga popularitas lagu tidak dapat dijelaskan hanya berdasarkan karakteristik audio.

## 📊 Dashboard

Hasil analisis data Spotify divisualisasikan dalam dashboard interaktif menggunakan Looker Studio.

Dashboard menyajikan berbagai informasi mengenai popularitas lagu, genre musik, karakteristik audio, konten eksplisit, serta hubungan antarfitur audio.

🔗 **Lihat Dashboard:** [Dashboard Analisis Spotify](https://datastudio.google.com/reporting/6b7ec764-b513-4e50-835c-b2f42dcb3bf9)

## 🛠️ Tools dan Library

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- SciPy
- Jupyter Notebook
- Looker Studio

## 📁 Struktur Repository

```text
spotify-data-analysis/
├── README.md
└── spotify-data-analysis.ipynb
