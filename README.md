# Travel-Insurance-Claim-Detection

Proyek ini saya kerjakan dalam rangka memenuhi tugas Capstone Project Module 3 di program Job Connector Data Science Purwadhika. Setelah menyelesaikan serangkaian materi dan latihan di modul 3 yang berfokus di Machine Learning,
saya mampu menyelesaikan proyek ini dalam 2 minggu. Proyek ini secara pribadi saya anggap sebagai awal dari lebih banyak lagi proyek pengolahan data yang akan menjadikan saya
lebih mahir dan percaya diri dalam menangani data sebagai data scientist.

Data ini terlebih dahulu dipersiapkan oleh tim pengajar Purwadhika, sehingga bukan data asli. Pertama-tama saya mengeksplorasi data ini, proses bisa ditemukan di file 
[1. Business Comprehension and Pre Processing Data Travel Insurance](https://github.com/Nasyahh/Capstone-Poject-Module-3---Travel-Insurance-Claim-Detection/blob/main/1.%20Business%20Comprehension%20and%20Pre%20Processing%20Data%20Travel%20Insurance.ipynb) dan menemukan bahwa data ini mengklasifikasikan data nasabah ke dalam dua kelas yaitu Claim 'Yes' dan Claim 'No'. Setiap baris memiliki data riwayat nasabah berupa umur, destinasi perjalanan, durasi perjalanan, agensi perjalanan, kanal pembelian,
dan sebagainya. Saya menemukan bahwa di data ini lebih banyak yang tidak klaim asuransi dibandingkan yang klaim asuransi. Sehingga model yang saya buat adalah detektor
yang mendeteksi nasabah yang klaim.
Selanjutnya menemukan model yang sesuai dari skor [cross validation](https://github.com/Nasyahh/Capstone-Poject-Module-3---Travel-Insurance-Claim-Detection/blob/main/2.%20Cross%20Validation%20Base%20Classification%20Model.ipynb)  yang menunjukkan model Decision Tree Classifier yang mampu mendeteksi kelas minoritas yaitu nasabah yang klaim.
Setelah proses Cross Validation, melanjutkan ke proses Imbalance Data Handling yang mencoba lima macam metode penanganan dan dari hasil Evaluation Matrix, ditemukan bahwa metode Random OverSampling
paling tepat digunakan dalam dataset ini. Karena hasil Evaluation Matric menunjukkan model yang overfitting / terlalu menghafal pola kelas 1, maka dilakukan [tuning] untuk memangkas tree/pohon keputusan.

Model deteksi ini tepat digunakan oleh perusahaan asuransi perjalanan dan sejenisnya, dikarenakan model deteksi mampu memprediksi nasabah yang akan klaim atau tidak klaim asuransi sejak nasabah tersebut melengkapi
pembelian produk, pembayaran premi, destinasi perjalanan dan data diri. Jika perusahaan menerapkan model deteksi ini, maka perusahaan akan mendapat support/saran dalam manajemen keuangannya.
Sehingga mampu membuat keputusan kapan dan dalam jumlah berapa perlu menyiapkan cash untuk melayani klaim nasabah atau untuk dijadikan sebagai instrumen investasi dan mendapat capital gain.

Model ini masih bisa diperbaiki lagi dengan data yang lebih merujuk pada klaim asuransi seperti riwayat penyakit, pernah mengajukan klaim atau tidak, besaran premi, jumlah orang yang mendapat proteksi dan sebagainya.
Akhir kata, proyek ini saya kerjakan sebagai pembelajar yang masih baru di bidang Data Science, masukan dapat saya terima melalui email nasyahrike@gmail.com
