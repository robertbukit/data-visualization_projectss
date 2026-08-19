# Excel-Sales-Dashboard

### Problem Statement
Sebuah perusahaan ritel global ingin mengembangkan dashboard analisis penjualan mereka. Pendekatan untuk analisis data penjualan saat ini kurang mendalam dan interaktif, memperlambat kinerja untuk mendapat insight dan analisis serta keputusan bisnis mereka. Metode laporan dalam bentuk konvensional/tradisional masih gagal dalam memberikan pandangan komprehensif metrik penjualan. Hal ini memaksakan untuk membuat analisis dashboard untuk membuka boundary dan memaksimalkan potensial penjualan mereka.
### Objective
Membuat dashboard dari rangkaian tabel transaksi penjualan yang terkoneksi untuk memberikan insight yang dinamis dan komprehensif. Menguatkan dan mensupport para decision-makers dengan memprovide data intelligence yang robust. Dashboard ini dirancang dengan cermat untuk memberikan tampilan dan perspektif yang holistik untuk kinerja Perusahaan. Dalam pengembangan ini, insight yang saya berikan pada dashboard meliputi; Analisis kinerja penjualan dari waktu ke waktu, Market/wilayah yang memberikan kontribusi terbesar dalam rentang waktu, Kategori produk yang laris terjual, Analisis segment pelanggan yang paling berkontribusi, Pola belanja disetiap market berdasarkan kategori, dan Analisis ship mode dan order priority yang paling berkontribusi pada sales.
### Key Features:
- Order ID: Kode unik untuk setiap transaksi (*jika ada lebih dari 1 kode unik dalam baris artinya barang-barang dibeli dalam struk belanja yang sama)
- Order date: Tanggal pesanan customer
- Ship date: Tanggal barang mulai dikirim
- Ship mode: Jenis layanan pengiriman (eg. Standard Class, First Class)
- Segment: Tipe customer yang membeli produk (eg. Customer, Corporate, Home Office)
- Market: Wilayah sasaran produk dijual (eg. LATAM, USCA, Europe, Pacific Asia, Africa)
- Category: Kategori barang yang dijual (eg. Technology, Furniture, Office Supplies)
- Sales: Harga/nilai penjualan dari barang tsb

### The Process:
1. Mengumpulkan/mengambil data: Data diperoleh dari website myonlinetraininghub.com, data berisi banyak sub data yang berisi informasi penjualan dari awal tahun 2020 sampai  akhir tahun 2022. Kemudian memindahkan ke power query pada excel dengan menghubungkan banyak subset data tadi dengan satu folder saja dengan "combine & transform".
2. Data Preprocessing: Awalnya data memiliki error yang sangat besar sekitar 90% dari baris data, ini disebabkan kesalahan indentifikasi tipe data pada kolom order date, ship date, dan sales dan saya mengubah masing-masing dari kolom dengan "change type with locale" pada fitur transform power query. Kemudian sisanya ialah teknis prosedural seperti memindahkan baris pertama menjadi header, Renamed kolom, dsb.
3. Membuat pivot table dari data yang di load dari power query tadi untuk agregasi, filter, dan sumarisasi data sesuai dengan objektif yang hendak divisualisasikan.
4. Menggabungkan pivot table yang telah dibuat ke sheet dashboard sales.

### Project Conclusion:
1. Dominasi Pasar Eropa: Pasar Eropa secara konsisten menjadi kontributor pendapatan terbesar, terutama didorong oleh segmen pelanggan Corporate. Ini menunjukkan area kekuatan yang bisa dipertahankan atau direplikasi di pasar lain.
2. Potensi Kategori Teknologi: Kategori produk Technology menunjukkan kinerja yang kuat dan kemungkinan memiliki margin keuntungan yang tinggi, menjadikannya area fokus untuk strategi pemasaran dan penjualan di masa depan.
3. Peluang Peningkatan Logistik: Ditemukan adanya potensi inefisiensi pada waktu pengiriman, khususnya di pasar Amerika Latin (LATAM). Ini adalah insight operasional yang dapat ditindaklanjuti untuk meningkatkan kepuasan pelanggan dan efisiensi biaya.

