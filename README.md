# Analisis Pola Penyewaan Sepeda di Seoul

## Repository Outline
1. `README.md` - Berisi gambaran umum dan penjelasan project.
2. `notebook.ipynb` - Notebook yang berisi proses pengolahan, analisis dan visualisasi data menggunakan Python.
3. `SeoulBikeData.csv` - Dataset asli Seoul Bike Sharing Demand.
4. `Seoul_Bike_Dataset_Clean.csv` - Dataset yang telah dibersihkan dan difilter berdasarkan hari operasional.

## Problem Background
Penyewaan sepeda adalah salah satu alternatif transportasi yang dapat membantu masyarakat dalam melakukan perjalanan. Namun, jumlah penyewaan sepeda di Seoul tidak selalu sama karena dapat berubah berdasarkan waktu, musim, kondisi cuaca dan hari libur. Perubahan tersebut dapat menyulitkan penyedia layanan sewa sepeda dalam menentukan jumlah sepeda yang harus disiapkan pada waktu tertentu.

Oleh karena itu, project ini dilakukan untuk menganalisis karakteristik dan pola penyewaan sepeda berdasarkan jam, bulan, musim, hari libur dan kondisi hujan / salju. Jadi nantinya hasil analisis ini dapat digunakan untuk membantu pengelola layanan sewa sepeda dalam menentukan waktu yang tepat untuk menyediakan jumlah sepeda pada waktu ramai.

## Project Output
Output dari project ini adalah hasil analisis statistik deskriptif dan inferensial, visualisasi data menggunakan Python dan dashboard interaktif menggunakan Tableau.

Hasil analisis menunjukkan waktu, bulan, musim dan kondisi cuaca yang memiliki jumlah penyewaan sepeda tertinggi.

## Data
Data yang digunakan adalah dataset Seoul Bike Sharing Demand dari UCI Machine Learning Repository. Dataset ini data penyewaan sepeda setiap jam di Seoul selama 1 Desember 2017 sampai 30 November 2018.

Dataset awal berisi 8.760 baris dan 14 kolom dan tidak memiliki missing values. Datanya berisi informasi jumlah penyewaan sepeda, tanggal, jam, suhu, kelembapan, kecepatan angin, jarak pandang, suhu titik embun, radiasi matahari, curah hujan, salju, musim, hari libur dan status operasional layanan sewa sepeda.

Setelah data difilter, jadi hanya mengambil data saat layanan sewa sepeda beroperasi saja. Maka jumlah datanya berkurang menjadi 8.465 baris.

## Method
Metode yang digunakan dalam project ini :

1. Data Cleaning = Membersihkan nama kolom, Mengubah tipe data tanggal, memeriksa missing values dan filter data berdasarkan status operasional.
2. Analisis statistik deskriptif untuk mengetahui mean, median, modus, standar deviasi, variance, range, quartile, IQR, skewness dan kurtosis.
3. Visualisasi menggunakan Histogram, Boxplot dan Line Chart untuk mengetahui distribusi dan tren penyewaan sepeda.
4. Pengujian One-Way ANOVA dengan tingkat signifikansi 5% untuk mengetahui apakah terdapat perbedaan rata - rata jumlah penyewaan sepeda yang signifikan antar musim.
5. Pembuatan Dashboard Interaktif menggunakan Tableau.

## Stacks
-> Bahasa Pemrograman yang dipakai : Python.

-> Tools yang digunakan : Jupyter Notebook dan Tableau.

-> Library yang digunakan : Pandas, Numpy, Scipy, Matplotlib dan Seaborn.

## Reference
-> Dataset Seoul Bike Sharing Demand : https://archive.ics.uci.edu/dataset/560/seoul%2Bbike%2Bsharing%2Bdemand

-> Dashboard Tableau : https://public.tableau.com/views/DistribusiJumlahPenyewaanSepedapadaHariLiburdanHaribukanLibur/Dashboard1?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link

-> Statistical Analysis Tableau : https://public.tableau.com/views/DistribusiJumlahPenyewaanSepedapadaHariLiburdanHaribukanLibur/StatisticalAnalysis?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link

---