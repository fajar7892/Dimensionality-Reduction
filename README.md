# Dimensionality Reduction dengan PCA dan t-SNE

## Deskripsi Kasus
Pada tugas ini dilakukan penerapan teknik dimensionality reduction menggunakan
Principal Component Analysis (PCA) dan t-Distributed Stochastic Neighbor Embedding (t-SNE).
Kasus yang diangkat adalah visualisasi dan eksplorasi pola data berdimensi tinggi
agar lebih mudah dipahami secara visual.

Dataset yang digunakan memiliki beberapa fitur numerik sehingga sulit
divisualisasikan secara langsung. Oleh karena itu, diperlukan reduksi dimensi
untuk memetakan data ke dalam ruang dua dimensi.

---

## Dataset
Dataset yang digunakan adalah **Iris Dataset** yang tersedia pada library
`scikit-learn`.

- Jumlah data: 150 sampel
- Jumlah fitur: 4 fitur numerik
- Jumlah kelas: 3 kelas bunga Iris
- Sumber: `sklearn.datasets.load_iris`

---

## Metode yang Digunakan
Tahapan analisis yang dilakukan adalah sebagai berikut:
1. **Standardisasi Data** menggunakan StandardScaler
2. **Principal Component Analysis (PCA)** untuk reduksi dimensi ke 2D
3. **t-Distributed Stochastic Neighbor Embedding (t-SNE)** untuk reduksi dimensi ke 2D
4. **Visualisasi hasil** PCA dan t-SNE menggunakan scatter plot

---

## Hasil dan Analisis

### Hasil PCA
PCA mampu mereduksi data ke dua dimensi dengan mempertahankan variasi terbesar
dalam data. Hasil visualisasi menunjukkan bahwa salah satu kelas terpisah dengan
cukup jelas, sementara dua kelas lainnya masih memiliki tumpang tindih.
PCA bersifat linear dan lebih menekankan struktur global data.

### Hasil t-SNE
t-SNE menghasilkan visualisasi cluster yang lebih jelas dibandingkan PCA.
Metode ini mampu menangkap hubungan non-linear dan mempertahankan kedekatan lokal
antar data, sehingga pemisahan antar kelas terlihat lebih tegas.

---

## Analisis Perbandingan PCA dan t-SNE
- PCA bersifat linear dan cocok digunakan untuk preprocessing sebelum modeling
- t-SNE bersifat non-linear dan sangat efektif untuk visualisasi cluster
- Untuk kasus eksplorasi dan visualisasi data, t-SNE memberikan hasil yang lebih informatif
- Untuk reduksi fitur sebelum pemodelan, PCA lebih direkomendasikan

---

## Kesimpulan
Dimensionality reduction menggunakan PCA dan t-SNE membantu dalam memahami
struktur data berdimensi tinggi. PCA efektif dalam merangkum informasi utama
data secara global, sedangkan t-SNE lebih unggul dalam menampilkan pola dan
cluster data. Pemilihan metode harus disesuaikan dengan tujuan analisis,
apakah untuk visualisasi atau preprocessing sebelum modeling.

---

## Anggota Kelompok
- Aufa Dhia Arkan (24523156)
- Muh. Fajar Rayhan Linta (24523117)

