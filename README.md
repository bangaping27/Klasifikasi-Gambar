
# Klasifikasi-Gambar

Project ini mengembangkan model jaringan saraf konvolusi (CNN) yang mampu mengenali gestur tangan yang mewakili gunting, batu, atau kertas dari gambar yang diunggah. Model ini mencapai akurasi 92% pada validation set, menunjukkan keefektifannya dalam pengenalan gestur tangan.

## Metodologi
Dataset:

Dataset rockpaperscissors digunakan untuk pelatihan dan validasi.
Dataset dibagi menjadi training set (1314 sampel) dan validation set (874 sampel).
Augmentasi Data Gambar:

Image data generator digunakan untuk melakukan augmentasi data (rescale, shear, zoom, horizontal flip) untuk meningkatkan variasi data dan mengurangi overfitting.
Model Jaringan Saraf Konvolusi (CNN):

Model CNN sekuensial dibangun menggunakan TensorFlow.
Arsitektur model menggunakan transfer learning dengan model MobileNetV2 terlatih, meningkatkan akurasi dengan waktu pelatihan terbatas.
Ensemble learning diterapkan dengan menggabungkan dua model CNN terpisah untuk lebih meningkatkan kinerja.
Pelatihan Model:

Model dilatih pada training set dan divalidasi pada validation set.
Fungsi loss categorical cross-entropy digunakan karena sifat klasifikasi multi-kelas dari masalah ini.
Pelatihan dilakukan di Google Colaboratory, mengikuti batasan waktu 30 menit.
Prediksi Gambar:

Fungsi dikembangkan untuk memprediksi gestur tangan dari gambar yang diunggah ke Colaboratory.
Hasil
Akurasi model yang dicapai pada validation set adalah 92%, menunjukkan pengenalan gestur tangan yang berhasil.

Kesimpulan
Project ini berhasil membangun model CNN yang mampu mengenali gestur tangan secara akurat. Penerapan teknik transfer learning dan ensemble learning berkontribusi signifikan terhadap kinerja model.

Referensi
Tutorial TensorFlow untuk Klasifikasi Gambar: https://www.tensorflow.org/tutorials/images/classification
Dokumentasi TensorFlow: https://www.tensorflow.org/tutorials
Dataset Gunting-Batu-Kertas: 
