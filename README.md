# 📊 Dataset dan Analisis Bencana Kota Batu (2021-2023)

**Sumber Data**: BPBD Kota Batu  
**Periode**: 2021 - 2023  
**Pemrosesan**: Data diolah menjadi dataset akumulatif dari kejadian bencana selama tiga tahun untuk analisis lebih lanjut.

---

## 📖 Deskripsi

Dataset ini memuat informasi terkait bencana yang terjadi di Kota Batu antara tahun 2021 hingga 2023. Data ini diperoleh dari **Badan Penanggulangan Bencana Daerah (BPBD) Kota Batu** dan telah melalui proses pengolahan untuk memberikan gambaran yang lebih jelas mengenai pola dan distribusi bencana di wilayah tersebut.

Dataset ini mencakup berbagai jenis bencana yang terjadi di setiap desa/kelurahan, termasuk koordinat geografis untuk setiap lokasi, yang dapat membantu dalam analisis geospasial dan perencanaan mitigasi bencana.

---

## 📂 Struktur Dataset

| Kolom                     | Deskripsi                                                                                   |
|---------------------------|---------------------------------------------------------------------------------------------|
| `Desa/Kelurahan`          | Nama desa atau kelurahan tempat kejadian bencana                                           |
| `Kecamatan`               | Nama kecamatan di Kota Batu                                                                |
| `Latitude`                | Koordinat lintang dari lokasi desa/kelurahan                                               |
| `Longitude`               | Koordinat bujur dari lokasi desa/kelurahan                                                 |
| `Banjir`                  | Jumlah kejadian banjir di desa/kelurahan tersebut                                          |
| `Tanah Longsor`           | Jumlah kejadian tanah longsor di desa/kelurahan tersebut                                   |
| `Cuaca Ekstrem`           | Jumlah kejadian yang disebabkan oleh cuaca ekstrem                                         |
| `Kebakaran Hutan dan Lahan` | Jumlah kejadian kebakaran hutan dan lahan                                               |
| `Gempa Bumi`              | Jumlah kejadian gempa bumi yang mempengaruhi wilayah                                       |
| `Erupsi Gunung Api`       | Jumlah kejadian erupsi gunung api                                                          |
| `Epidemi dan Wabah Penyakit` | Jumlah kejadian epidemi atau wabah penyakit yang tercatat                              |
| `Gagal Teknologi`         | Jumlah kejadian yang melibatkan gagal teknologi                                            |
| `Konflik Sosial`          | Jumlah kejadian konflik sosial                                                             |
| `Total`                   | Total keseluruhan kejadian bencana di desa/kelurahan tersebut                              |

Setiap kolom di atas menggambarkan jenis dan jumlah bencana yang terjadi di setiap wilayah. Kolom `Total` mencatat jumlah total kejadian untuk semua jenis bencana di masing-masing desa/kelurahan, memberikan gambaran mengenai tingkat risiko di tiap lokasi.

---

## ⚙️ Skrip Analisis: `project_magang.py`

Skrip `project_magang.py` berfungsi sebagai alat untuk memproses dan menganalisis data bencana yang terdapat dalam dataset ini. Berikut adalah ringkasan fungsi-fungsi utama dalam skrip tersebut:

1. **Data Loading**  
   Skrip ini memuat dataset mentah dari BPBD dan menyiapkannya untuk analisis lebih lanjut.

2. **Data Preprocessing**  
   Menggunakan `StandardScaler` untuk normalisasi data, sehingga seluruh nilai berada dalam skala yang seragam, yang memudahkan analisis dan mengurangi bias dalam klasterisasi.

3. **Clustering**  
   Menggunakan algoritma **KMeans** untuk mengelompokkan data berdasarkan lokasi atau jenis bencana. Pengelompokan ini dapat membantu dalam mengidentifikasi pola wilayah yang paling rawan atau jenis bencana tertentu yang lebih sering terjadi di lokasi tertentu.

4. **PCA (Principal Component Analysis)**  
   Menggunakan **PCA** untuk mereduksi dimensi data, memungkinkan visualisasi data dalam ruang berdimensi rendah, yang memudahkan pemahaman pola distribusi bencana secara keseluruhan.

---

## 🎯 Tujuan Penggunaan

Dataset dan skrip ini dapat digunakan untuk berbagai tujuan, antara lain:

- **Perencanaan Mitigasi dan Kesiapsiagaan**: Membantu pihak BPBD dan pemerintah daerah dalam merencanakan langkah mitigasi di wilayah-wilayah rawan bencana.
- **Penelitian Akademik**: Dataset ini juga dapat menjadi dasar bagi peneliti yang ingin mengembangkan studi lebih lanjut terkait mitigasi bencana atau analisis spasial di bidang kebencanaan.

---

## 🚀 Cara Menggunakan

1. **Download** dataset dalam format CSV dari repositori ini.
2. **Jalankan** skrip `project_magang.py` untuk melakukan analisis. Anda memerlukan Python dan pustaka yang relevan (seperti `pandas`, `sklearn`, `matplotlib`, dll.) untuk menjalankan skrip.
3. **Visualisasi** hasil analisis, seperti klaster lokasi rawan bencana atau distribusi jenis bencana, menggunakan alat visualisasi (contoh: Matplotlib, Seaborn).

---

## 📝 Lisensi

Dataset ini tersedia untuk kepentingan penelitian, analisis, dan perencanaan mitigasi bencana. Harap menyertakan atribusi kepada **BPBD Kota Batu** jika dataset ini digunakan dalam publikasi atau penelitian.

---
