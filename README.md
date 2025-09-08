# Analisis Kepadatan Penduduk Muara Enim Menggunakan Algoritma DBSCAN pada Data Spasial

## 📌 Deskripsi
Proyek ini merupakan implementasi algoritma **DBSCAN (Density-Based Spatial Clustering of Applications with Noise)** untuk menganalisis **kepadatan penduduk Kabupaten Muara Enim** berbasis data spasial.  
Hasil clustering divisualisasikan dalam bentuk peta dan grafik untuk mengidentifikasi wilayah dengan kepadatan penduduk **rendah, sedang,** dan **noise**.

## 📂 Struktur Folder
ADSPSip 👍 saya bantu buatkan **README.md** yang rapi untuk repository GitHub kamu berdasarkan struktur folder dan hasil penelitian yang sudah ada.

Berikut contoh isi README:

---

# Analisis Kepadatan Penduduk Muara Enim Menggunakan Algoritma DBSCAN pada Data Spasial

## 📌 Deskripsi

Proyek ini merupakan implementasi algoritma **DBSCAN (Density-Based Spatial Clustering of Applications with Noise)** untuk menganalisis **kepadatan penduduk Kabupaten Muara Enim** berbasis data spasial.
Hasil clustering divisualisasikan dalam bentuk peta dan grafik untuk mengidentifikasi wilayah dengan kepadatan penduduk **rendah, sedang,** dan **noise**.

## 📂 Struktur Folder

```
ADSP/
│── Data/                          # Dataset mentah / pendukung
│── Hasil/                         # Hasil eksperimen dan visualisasi
│   ├── Data_Muara Enim.png
│   ├── Hasil Cluster DBSCAN Sebelum Definisi.png
│   ├── Hasil Cluster DBSCAN Setelah Definisi.png
│   ├── Rata-rata Kepadatan Penduduk.png
│   ├── DBSCAN Muara Enim.png
│   └── (REVISI) Laporan_Tugas_Besar_Kelompok04_RA.docx.pdf
│── Code_Tugas Besar_Kelompok04_RA.ipynb   # Notebook utama (implementasi DBSCAN)
│── README.md                      # Dokumentasi proyek
```


## 🛠️ Teknologi yang Digunakan
- Python (Jupyter Notebook)
- Library: `scikit-learn`, `matplotlib`, `geopandas`
- PostgreSQL (opsional, untuk penyimpanan data spasial)
- Git & GitHub (version control)

## 📊 Metodologi
1. **Pengumpulan Data**  
   Data spasial dan kepadatan penduduk dari Kabupaten Muara Enim.
2. **Preprocessing**  
   - Normalisasi data spasial (latitude, longitude).  
   - Pembersihan data noise.  
3. **Clustering dengan DBSCAN**  
   Parameter:  
   - `eps = 0.23`  
   - `minPts = 5`  
4. **Visualisasi**  
   - Peta sebaran kepadatan penduduk.  
   - Grafik perbandingan rata-rata kepadatan tiap cluster.  

## 📈 Hasil Visualisasi

### 1. Peta Kabupaten Muara Enim
![Peta Kabupaten Muara Enim](Hasil/Data_Muara%20Enim.png)

### 2. Hasil Clustering DBSCAN
- **Sebelum Definisi**
![Cluster DBSCAN Sebelum Definisi](Hasil/Hasil%20Cluster%20DBSCAN%20Sebelum%20Definisi.png)  

- **Setelah Definisi (Cluster 0, Cluster 1, Noise)**
![Cluster DBSCAN Setelah Definisi](Hasil/Hasil%20Cluster%20DBSCAN%20Setelah%20Defenisi.png)  

### 3. Rata-rata Kepadatan Penduduk per Cluster
![Rata-rata Kepadatan Penduduk](Hasil/Rata-rata%20Kepadatan%20Penduduk.png)

### 4. Poster Penelitian
![Poster Penelitian](DBSCAN%20Muara%20Enim.png)

## 📊 Evaluasi Model
- **Silhouette Score**: `0.475289`  
- **Davies-Bouldin Index**: `0.634530`  
- **Dunn Index**: `0.99822`  

## 📝 Kesimpulan
Metode DBSCAN berhasil mengelompokkan wilayah Kabupaten Muara Enim menjadi:  
- **Cluster 0** → Wilayah dengan kepadatan penduduk sedang (dekat pusat kota).  
- **Cluster 1** → Wilayah dengan kepadatan rendah (pinggiran/akses terbatas).  
- **Noise** → Wilayah yang tidak termasuk dalam cluster karena distribusi jarang.  

Dengan parameter yang tepat (`eps=0.23`, `minPts=5`), model menghasilkan clustering yang cukup akurat dan representatif.

## 👥 Anggota Kelompok
- Anastashya Rachman  
- Balqis Dwian Fitri Zamzami  
- Ghozi Alvin Karim  
- Rafi Fadhillah  
- Khalda Luthfi A  

## 📚 Referensi
- Silitje, E. K., Rangku, Y. M., & Karo, K. (2024). *Analisis Pengelompokan Titik Sebaran Hotspot Menggunakan DBSCAN pada Data Spasial*. Jurnal SAINTEKOM, 230–231.

