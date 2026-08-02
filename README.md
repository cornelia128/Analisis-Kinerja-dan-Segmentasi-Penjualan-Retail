# Analisis Performa Penjualan Ritel dan Tren Perilaku Belanja Konsumen Berdasarkan Demografi

## Business Problem
Perusahaan retail memiliki data transaksi yang mencakup berbagai kategori produk, karakteristik pelanggan, dan informasi penjualan, namun belum dimanfaatkan secara optimal untuk mendukung pengambilan keputusan bisnis. Akibatnya, perusahaan belum mengetahui kategori produk yang paling menguntungkan, karakteristik pelanggan dengan kontribusi pendapatan terbesar, pola penjualan berdasarkan waktu, maupun pengaruh harga terhadap jumlah pembelian. Oleh karena itu, diperlukan analisis data transaksi untuk menghasilkan insight yang dapat mendukung strategi pemasaran, pengelolaan stok, dan penentuan target pelanggan secara lebih efektif guna meningkatkan penjualan dan pendapatan perusahaan.

## Objectives
* Menentukan kategori produk yang memberikan kontribusi pendapatan terbesar dan memiliki volume penjualan tertinggi.
* Menganalisis bagaimana faktor demografi seperti Gender dan Age memengaruhi preferensi pemilihan kategori produk dan total pengeluaran dalam satu transaksi.
* Mengamati pola transaksi berdasarkan Date untuk menemukan periode puncak penjualan (misalnya harian, bulanan, atau musiman) guna membantu perencanaan promosi atau stok barang.
* Mengetahui hubungan antara Price per Unit dengan Quantity yang dibeli untuk melihat apakah harga produk tertentu memengaruhi jumlah barang yang diambil oleh pelanggan.
* Memberikan rekomendasi strategis bagi bisnis dalam menargetkan kelompok usia atau jenis kelamin tertentu berdasarkan data historis transaksi yang paling menguntungkan. 

## Business Questions
* Kategori produk manakah yang menghasilkan total pendapatan tertinggi sepanjang periode transaksi yang tercatat?
* Bagaimana perbandingan total nilai belanja antara pelanggan Male dan Female? Apakah ada kategori produk tertentu yang jauh lebih diminati oleh salah satu gender?
* Apakah terdapat tren tertentu pada kelompok usia misalnya usia 18-30 tahun, dalam frekuensi pembelian produk di pada setiap kategori?
* Pada bulan atau tanggal berapa terjadi puncak penjualan tertinggi, dan apakah terdapat pola musiman dalam aktivitas transaksi pelanggan?
* Berapa rata-rata jumlah barang yang dibeli dalam satu transaksi untuk setiap kategori produk, dan bagaimana hubungannya dengan harga satuan?
  
## Dataset
* Sumber Data: [Kaggle - Retail Sales Dataset](https://www.kaggle.com/datasets/mohammadtalib786/retail-sales-dataset?resource=download)
* Struktur Dataset:
  - Dataset retail_sales_dataset.csv memiliki struktur yang terdiri dari 1.000 baris data transaksi ritel dengan 9 kolom utama.
  - Mencakup transaksi pada tahun 2023 hingga awal 2024.
  - Rincian kolom: data identitas waktu (transaction id, customer id, date), data demografi pelanggan (gender, age), data produk dan nilai transaksi (product category, quantity, price per unit, total amount).
  
## Tools
* Excel
  
## Exploratory Data Analysis
* Menganalisis fluktuasi total belanja harian sepanjang tahun 2023 untuk melihat pola dan lonjakan penjualan.
* Membandingkan total pendapatan tiap kategori produk untuk menentukan kategori paling menguntungkan.
* Membandingkan total belanja Male dan Female pada setiap kategori produk untuk melihat preferensi gender.
* Menganalisis total belanja berdasarkan jumlah unit yang dibeli pada tiap kategori produk.
* Mengelompokkan pelanggan ke dalam rentang usia dan membandingkan total belanja mereka per kategori produk.

## Dashboard Excel
[Dashboard Excel - Retail Sales Performance Dashboard](https://1drv.ms/x/c/33df3e24b33e1e8a/IQDIvAH6RuqbSrRrh2Oj9aJ2AYuBvZxfvnXAbHeLUbi0_Lw?e=aKErDX)

<img src="https://github.com/cornelia128/Analisis-Kinerja-dan-Segmentasi-Penjualan-Retail/blob/main/images/Dashboard%20Excel.png?raw=true" width=500 height=300>

## Business Insights

<img src="https://github.com/cornelia128/Analisis-Kinerja-dan-Segmentasi-Penjualan-Retail/blob/main/images/Distribusi%20Kategori%20Produk.jpg?raw=true" width=500 height=300>

Electronics menghasilkan pendapatan tertinggi ($156.905), namun selisihnya sangat tipis terhadap Clothing ($155.580), hanya sekitar (0,85%). Beauty berada di posisi terakhir ($143.515), namun perbedaannya terhadap dua kategori lain tidak signifikan (<10%). Ketiga kategori berkontribusi hampir merata terhadap total pendapatan ($456.000). Electronics unggul tipis sebagai penyumbang pendapatan tertinggi ($156.905), diikuti Clothing dan Beauty; hampir merata, bukan didominasi satu kategori.

<img src="https://github.com/cornelia128/Analisis-Kinerja-dan-Segmentasi-Penjualan-Retail/blob/main/images/Tren%20Belanja%20Harian%202023.jpg?raw=true" width=500 height=300>

Pola belanja harian sangat fluktuatif dengan lonjakan tajam (spike) di beberapa tanggal tertentu; indikasi adanya event, promo, atau payday effect. Bulan Mei, Oktober, dan Desember tercatat sebagai bulan dengan total pendapatan tertinggi sepanjang 2023, mengindikasikan pola musiman yang bisa dimanfaatkan untuk perencanaan promosi. 

<img src="https://github.com/cornelia128/Analisis-Kinerja-dan-Segmentasi-Penjualan-Retail/blob/main/images/Perbandingan%20Gender.jpg?raw=true" width=500 height=300>

Female mencatat total belanja sedikit lebih tinggi dari Male. Female paling dominan di Clothing ($81.275), sementara Male paling dominan di Electronics ($80.170). Beauty menjadi kategori dengan selisih gender terbesar; Female lebih unggul dibanding Male. Female menyumbang total belanja sedikit lebih besar dari Male; Female dominan di Clothing, Male dominan di Electronics.

<img src="https://github.com/cornelia128/Analisis-Kinerja-dan-Segmentasi-Penjualan-Retail/blob/main/images/Kuantitas%20per%20Kategori.jpg?raw=true" width=500 height=300>

Total belanja meningkat seiring bertambahnya Quantity di hampir semua kategori, dengan pembelian 3–4 unit menyumbang porsi terbesar. Electronics pada Qty 4 mencatat kontribusi tertinggi; mengindikasikan potensi bundling/paket produk elektronik.

<img src="https://github.com/cornelia128/Analisis-Kinerja-dan-Segmentasi-Penjualan-Retail/blob/main/images/Usia%20per%20Kategori.jpg?raw=true" width=500 height=300>

Kelompok usia (18-27) tahun paling dominan di Beauty & Clothing, sejalan dengan gaya hidup dan tren fashion/perawatan diri usia muda. Electronics justru paling diminati kelompok usia (48-57) tahun; bukan usia muda seperti asumsi umum. Kelompok usia (58-67) tahun konsisten menjadi kontributor terendah di semua kategori. Usia muda (18-27) mendominasi Beauty & Clothing, sedangkan Electronics justru paling diminati usia (48-57) tahun.

## Recommendation
* Alokasikan stok dan anggaran promosi lebih besar pada Electronics dan Clothing yang konsisten menjadi kontributor pendapatan tertinggi.
* Tingkatkan stok dan intensitas promosi menjelang bulan Mei, Oktober, dan Desember sebagai periode puncak penjualan historis.
* Jalankan promosi Clothing/Beauty untuk segmen Female, dan promosi Electronics untuk segmen Male guna mengoptimalkan konversi.
* Kembangkan strategi bundling/diskon kuantitas (3-4 unit) khususnya pada kategori Electronics untuk mendorong nilai transaksi lebih tinggi.
* Targetkan kelompok usia 48-57 tahun untuk kampanye Electronics, bukan hanya asumsi usia muda sebagai target utama.
 
## Conclusion
* **Ketegori Produk:** Electronics mencatat pendapatan tertinggi ($156.905), namun selisihnya sangat tipis dengan Clothing ($155.580). Beauty juga berkontribusi cukup besar ($143.515). Artinya, ketiga kategori relatif seimbang dalam kontribusi pendapatan.
* **Gender:** Female sedikit lebih tinggi dalam total belanja dibanding Male. Female dominan di Clothing & Beauty, sementara Male dominan di Electronics.
* **Usia:** Kelompok usia muda (18–27 tahun) mendominasi Beauty & Clothing. Namun, Electronics justru paling diminati kelompok usia 48–57 tahun, bukan usia muda seperti asumsi umum.
* **Pola Waktu:** Penjualan harian fluktuatif dengan lonjakan pada periode tertentu. Bulan Mei, Oktober, dan Desember adalah puncak penjualan, menunjukkan adanya pola musiman yang bisa dimanfaatkan untuk promosi.
* **Harga vs Kuantitas:** Hampir tidak ada korelasi antara harga satuan dan jumlah barang yang dibeli. Pembelian multi-unit (3–4 unit) menyumbang porsi terbesar, terutama Electronics pada Qty 4 ($69.680).
