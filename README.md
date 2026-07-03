# skin-lesion-mobilenetv2

# README Proyek Kecerdasan Buatan - Klasifikasi Acne, Eczema, dan Rosacea

## Deskripsi Proyek
Proyek ini bertujuan untuk mengembangkan model klasifikasi citra kulit menggunakan Convolutional Neural Network (CNN) berbasis arsitektur MobileNetV2. Model ini digunakan untuk mengenali tiga kelas penyakit kulit, yaitu:
- Acne
- Eczema
- Rosacea

Proyek ini dibuat berdasarkan notebook utama yang tersedia pada [KODE_PROGRAM_AI_KELOMPOK_12_4A_IF (1).ipynb](KODE_PROGRAM_AI_KELOMPOK_12_4A_IF%20(1).ipynb).

## Tujuan
- Membangun model klasifikasi gambar penyakit kulit dengan akurasi yang baik.
- Menggunakan transfer learning agar pelatihan lebih cepat dan efisien.
- Menyediakan hasil evaluasi model melalui akurasi, loss, confusion matrix, dan prediksi citra.

## Metode yang Digunakan
- Dataset gambar dikumpulkan dari folder pelatihan.
- Data dipilih hanya untuk tiga kelas target: acne, eczema, dan rosacea.
- Data dibagi menjadi data train, validation, dan test.
- Digunakan teknik augmentasi data untuk meningkatkan generalisasi model.
- Arsitektur model yang dipakai adalah MobileNetV2 dengan transfer learning.
- Model dievaluasi menggunakan classification report dan confusion matrix.

## Tools dan Library
Library yang digunakan dalam proyek ini antara lain:
- Python
- TensorFlow / Keras
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Pillow

## Persiapan Environment
Install dependency yang dibutuhkan dengan perintah berikut:

```bash
pip install tensorflow pandas numpy matplotlib seaborn scikit-learn pillow
```

## Cara Menjalankan
1. Buka notebook [KODE_PROGRAM_AI_KELOMPOK_12_4A_IF.ipynb](KODE_PROGRAM_AI_KELOMPOK_12_4A_IF%20.ipynb).
2. Jalankan semua cell secara berurutan.
3. Pastikan path dataset sudah sesuai.
4. Model akan disimpan dalam file:
   - mobilenetv2_skin_3classes_ai.h5

## Struktur Hasil Proyek
- Dataset preprocessing dan splitting data
- Pembuatan generator gambar untuk train, validation, dan test
- Pelatihan model MobileNetV2
- Fine-tuning model
- Evaluasi hasil model
- Simpan model untuk prediksi lebih lanjut

## Hasil yang Diharapkan
Model diharapkan mampu memprediksi jenis penyakit kulit dari citra input dengan tingkat akurasi yang baik. Hasil evaluasi dapat dilihat melalui:
- accuracy
- loss
- confusion matrix
- classification report

## Pembagian Peran Anggota Tim (3 Orang)
Berikut pembagian peran yang sesuai dengan isi kode dan workflow proyek:

### Anggota 1 - Adelyn Sulaeman (Data Preparation & Exploratory Data Analysis)
Tanggung jawab:
- Menyiapkan dataset dan memastikan path gambar benar.
- Memfilter kelas data menjadi acne, eczema, dan rosacea.
- Membuat visualisasi distribusi data.
- Membagi data menjadi train, validation, dan test.

### Anggota 2 - Mediana Santosa (Model Development & Training)
Tanggung jawab:
- Membangun pipeline data augmentation.
- Membuat arsitektur model MobileNetV2.
- Melakukan training awal dan fine-tuning model.
- Mengevaluasi performa model melalui loss, accuracy, confusion matrix, dan classification report.

### Anggota 3 - Devika Lorensa (Inference, Dokumentasi & Reporting)
Tanggung jawab:
- Menguji model dengan gambar baru untuk prediksi.
- Menyimpan model hasil training.
- Menyusun dokumentasi proyek dan hasil akhir.
- Menyiapkan penjelasan singkat untuk presentasi atau laporan.

## Catatan
Jika ingin menjalankan proyek di lingkungan lokal, pastikan path dataset disesuaikan dengan lokasi penyimpanan masing-masing. Jika menggunakan Kaggle, path dataset yang dipakai sudah sesuai dengan notebook.

## Penutup
Proyek ini merupakan contoh implementasi klasifikasi gambar menggunakan deep learning dengan transfer learning. Hasil yang baik sangat bergantung pada kualitas dataset, proses preprocessing, dan pemilihan hyperparameter yang tepat.
