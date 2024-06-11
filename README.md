# Apartment-Price-Prediction
# Prediksi Harga Apartemen di Daegu, Korea Selatan

Proyek ini bertujuan untuk mengembangkan model prediksi harga apartemen di Daegu, Korea Selatan. Model ini akan membantu `agen properti` dalam menetapkan harga yang sesuai dengan nilai pasar, dengan mempertimbangkan berbagai faktor yang mempengaruhi harga apartemen.


## Pendahuluan

Daegu, Korea Selatan, merupakan salah satu kota yang mengalami pertumbuhan ekonomi dan perkotaan yang pesat. Sebagai salah satu kota terbesar di Korea Selatan, Daegu menarik banyak penduduk dan pendatang yang mencari peluang ekonomi dan pendidikan tinggi. Seiring dengan pertumbuhan ini, kebutuhan akan perumahan, termasuk apartemen, juga meningkat secara signifikan.

## Masalah Penetapan Harga Apartment

Pasar apartemen di Daegu menawarkan berbagai tipe unit, mulai dari apartemen mewah hingga apartemen sederhana, dengan berbagai fasilitas dan lokasi yang beragam. Penetapan harga apartemen tetap menjadi tantangan karena pemilik apartemen sering kali kesulitan menentukan harga yang sesuai dengan nilai pasar. Harga yang terlalu tinggi dapat menyulitkan untuk menarik pembeli, sedangkan harga yang terlalu rendah dapat menyebabkan kerugian finansial.

## Problem Statement

Penetapan harga apartemen yang tidak tepat dapat mengakibatkan kerugian finansial atau kesulitan dalam menarik pembeli. Faktor-faktor kompleks seperti lokasi, fasilitas di sekitarnya, dan tren pasar mempengaruhi proses penetapan harga. Oleh karena itu, diperlukan pendekatan yang sistematis untuk memprediksi harga apartemen yang akurat.

## Stakeholder

Stakeholder utama dari proyek ini adalah `agen properti` yang bertanggung jawab dalam membantu pemilik properti menetapkan harga jual apartemen. Dengan bantuan model ini, mereka dapat membuat keputusan harga yang lebih tepat dan kompetitif, yang pada akhirnya dapat meningkatkan keuntungan dan kepuasan pelanggan.

## Tujuan

Tujuan dari proyek ini adalah untuk mengembangkan model prediksi harga apartemen yang dapat membantu agen properti dalam menetapkan harga yang sesuai dengan nilai pasar. Dengan menggunakan berbagai fitur yang relevan, model ini diharapkan dapat memberikan perkiraan harga yang lebih akurat.

## Analytics Approach

1. **Eksplorasi Data**: Melakukan pengecekan statistik dan eksplorasi data untuk mengidentifikasi fitur yang berpengaruh terhadap harga apartemen.
2. **Pembersihan Data**: Pembersihan dan pra-pemrosesan data untuk persiapan pemodelan.
3. **Pemodelan**: Pelatihan data menggunakan beberapa model benchmark untuk membandingkan tingkat error dari masing-masing model dan memilih model dengan tingkat error terendah.

## Metrics Evaluation

Metrik evaluasi yang digunakan untuk mengukur performa model machine learning adalah:

- **Root Mean Square Error (RMSE)**: Mengukur kesalahan model regresi dengan menghitung akar kuadrat rata-rata dari perbedaan antara nilai yang diprediksi dan nilai sebenarnya. RMSE memberikan bobot lebih besar pada kesalahan besar.
- **Mean Absolute Error (MAE)**: Mengukur rata-rata dari selisih absolut antara nilai yang diprediksi dan nilai sebenarnya, memberikan bobot yang sama pada semua kesalahan.
- **Mean Absolute Percentage Error (MAPE)**: Mengukur kesalahan model dalam bentuk persentase dari kesalahan relatif terhadap nilai sebenarnya.

Semakin kecil nilai RMSE, MAE, dan MAPE, semakin baik model dalam memprediksi data sebenarnya. MAPE khususnya berguna untuk menginterpretasikan hasil error dalam bentuk persentase, sehingga mudah dipahami.


## Perbandingan dengan Model Rule-Based
Model rule-based adalah pendekatan tradisional yang menggunakan aturan-aturan yang ditentukan secara eksplisit untuk menetapkan harga apartemen. Aturan-aturan ini biasanya berdasarkan pengetahuan domain dan pengalaman praktis agen properti, seperti:

- Harga dasar per meter persegi berdasarkan lokasi.
- Penyesuaian harga berdasarkan jumlah luasan apartment (sqf)
- Pada data Aprtment Daegu diketahui tipe hallway (HallwayType) mempengaruhi median harga,

maka dari itu ditentukan `Size(sqf)` dan `HallwayType` sebagai fitur yang mempengaruhi prediksi harga.


### Perbandingan dengan Model Machine Learning

Model machine learning yang dikembangkan dalam proyek ini diharapkan dapat menangkap kompleksitas data dan menghasilkan prediksi yang lebih akurat dibandingkan dengan model rule-based. Model ini menggunakan berbagai fitur yang relevan dan dapat disesuaikan serta ditingkatkan seiring waktu berdasarkan data baru dan tren pasar.

### Hasil Perbandingan

Setelah melakukan pelatihan dan evaluasi model machine learning, hasilnya akan dibandingkan dengan model rule-based menggunakan metrik evaluasi (RMSE, MAE, dan MAPE). Diharapkan model machine learning akan menunjukkan performa yang lebih baik dengan nilai error yang lebih rendah, memberikan prediksi harga apartemen yang lebih akurat dan dapat diandalkan.

Dengan demikian, agen properti dapat membuat keputusan yang lebih tepat dan kompetitif, meningkatkan kepuasan pelanggan dan mengoptimalkan keuntungan.
