1.1	Latar Belakang
NetSpeed Solutions merupakan penyedia layanan internet (ISP) lokal yang tengah berada dalam fase ekspansi strategis. Saat ini, perusahaan melayani ekosistem pelanggan yang terdiri dari 500 pelanggan perumahan dan 50 pelanggan bisnis. Dalam operasional hariannya, NetSpeed Solutions masih mengandalkan mekanisme pencatatan konvensional menggunakan spreadsheet (Excel) serta koordinasi layanan melalui platform WhatsApp.
Ketergantungan pada proses manual ini menjadi hambatan kritikal bagi skalabilitas perusahaan. Seiring dengan meningkatnya kompleksitas layanan, terutama untuk segmen pelanggan bisnis, diperlukan transisi ke arah sistem informasi yang terintegrasi. NetSpeed Hub dirancang sebagai solusi otomatisasi untuk mengonsolidasikan administrasi, manajemen jaringan, dan pelaporan keuangan ke dalam satu platform tunggal yang efisien dan terukur.
1.2	Rumusan Masalah
Analisis operasional mengidentifikasi empat kendala utama (pain points) yang berdampak langsung pada performa bisnis:
-	Ketidakteraturan Data: Kesulitan dalam melacak status pembayaran secara akurat mengakibatkan risiko kesalahan input keuangan dan ketidakpastian arus kas.
-	Manajemen Bandwidth Manual: Konfigurasi teknis untuk upgrade atau downgrade layanan masih dilakukan secara manual oleh tim teknis, yang memicu keterlambatan respons terhadap permintaan pelanggan.
-	Stok Alat Tidak Terpantau: Kurangnya sinkronisasi data inventaris (router, kabel, konektor) sering menyebabkan kegagalan instalasi akibat stok habis yang tidak terdeteksi sebelumnya.
-	Komplain Pelanggan Lambat: Keterbatasan akses pelanggan terhadap rincian tagihan dan status perbaikan jaringan menurunkan tingkat kepuasan layanan secara signifikan.
1.3	Tujuan 
Perancangan sistem NetSpeed Hub ditujukan untuk mencapai target sebagai berikut:
-	Otomatisasi Proses: Mereduksi waktu aktivasi pelanggan baru dari 2 hari menjadi maksimal 2 jam setelah verifikasi pembayaran.
-	Transparansi Pelaporan: Menyediakan grafik keuntungan dan laporan keuangan yang akurat bagi pemilik perusahaan guna mendukung pengambilan keputusan berbasis data.
-	Peningkatan Skalabilitas: Mengoptimalkan infrastruktur administrasi sehingga perusahaan mampu melayani hingga 5.000 pelanggan tanpa penambahan staf yang signifikan.

1.4	Manfaat
Implementasi sistem ini memberikan nilai tambah bagi seluruh pemangku kepentingan:
-	Modul Administrasi & Keuangan: Otomatisasi siklus penagihan dan agregasi laporan pemasukan/pengeluaran (pembelian alat, gaji teknisi).
-	Modul Manajemen Jaringan: Transparansi manajemen bandwidth dan sinkronisasi stok material teknis secara real-time.
-	Portal Pelanggan: Digitalisasi pengalaman pengguna melalui fitur pendaftaran mandiri dan akses informasi layanan 24/7.

1.5	Ruang Lingkup Sistem
Sistem NetSpeed Hub dibatasi pada pengembangan tiga modul utama:
-	Modul Administrasi: Pengelolaan basis data pengguna, manajemen penagihan otomatis, dan akuntansi internal.
-	Manajemen Jaringan & Inventaris: Dashboard teknis untuk pemantauan paket bandwidth dan pelacakan material produksi.
-	Portal Pelanggan: Antarmuka akses mandiri untuk pendaftaran, pelaporan gangguan, dan pengunduhan bukti transaksi.
BAB II ANALISIS SISTEM
2.1	 Deskripsis sistem
NetSpeed Hub adalah platform manajemen ISP berbasis web yang mengintegrasikan fungsi operasional jaringan dan administrasi bisnis. Sistem ini bertindak sebagai jembatan informasi antara pelanggan dan penyedia layanan, memastikan aliran data yang sinkron dari front-end hingga back-end.
2.2	 Analisis Permasalahan
Sistem manual yang ada saat ini gagal memenuhi kebutuhan pelanggan, terutama 50 pelanggan bisnis yang memiliki ekspektasi Service Level Agreement (SLA) lebih ketat dibandingkan pengguna perumahan. Koordinasi melalui WhatsApp sering menyebabkan informasi terfragmentasi, sementara penggunaan Excel untuk 550 pelanggan meningkatkan risiko data redundancy dan inkonsistensi stok alat yang menghambat kinerja teknisi di lapangan.

2.3	 Analisis dan Usulan
Solusi yang diusulkan mencakup tiga pilar fungsi integratif:
-	Modul Administrasi & Keuangan: Otomatisasi siklus penagihan dan agregasi laporan pemasukan/pengeluaran (pembelian alat, gaji teknisi).
-	Modul Manajemen Jaringan: Transparansi manajemen bandwidth dan sinkronisasi stok material teknis secara real-time.
-	Portal Pelanggan: Digitalisasi pengalaman pengguna melalui fitur pendaftaran mandiri dan akses informasi layanan 24/7.



2.4	Stackholder Sistem
Aktor	Peran	Tanggung Jawab
Pelanggan 	Pengguna Layanan	Pendaftaran mandiri, pemilihan paket, pembayaran tagihan, dan pelaporan kendala jaringan.
Administrator	Pengelola Operasional	Pendataan keuangan, pengelolaan data pelanggan, verifikasi pembayaran, dan manajemen stok inventaris.
Teknisi	Pelaksana Lapangan	Pemasangan perangkat, pemeliharaan jaringan, pembaruan status tiket gangguan, dan absensi kerja.
Manajer/Owner		Pengambil Keputusan	Pemantauan dashboard laporan keuangan, grafik keuntungan, dan evaluasi performa operasional.

2.5	Functional Requirements
Sistem memenuhi persyaratan fungsional sebagai berikut:
2.5.1	Pengelolaan data pengguna multifaktor
Sistem harus mampu mengelola data seluruh pengguna berdasarkan hak akses (role) yang dimiliki. Setiap jenis pengguna memiliki menu dan kewenangan yang berbeda sesuai tugasnya.
Fungsi yang harus tersedia:
-	Login dan Logout.
-	Menambah, mengubah, dan menghapus data pengguna.
-	Mengatur hak akses berdasarkan role.
-	Menampilkan dashboard sesuai jenis pengguna.
Hak akses masing-masing:
-	Admin : mengelola seluruh data sistem.
-	Teknisi : melihat daftar pekerjaan, memperbarui status perbaikan, dan mengisi laporan pekerjaan.
-	Customer : melihat tagihan, mengirim bukti pembayaran, membuat laporan gangguan, dan melihat status layanan.

2.5.2	Pencatatan Informasi Keuangan Komprehensif
Sistem harus mampu mencatat seluruh transaksi keuangan perusahaan secara otomatis sehingga kondisi keuangan dapat dipantau dengan mudah.
Data pemasukan meliputi : 
-	Pembayaran tagihan pelanggan.
-	Biaya pemasangan baru.
-	Pendapatan lainnya.
Data pengeluaran lainnya : 
-	Pembelian alat jaringan.
-	Pembelian bahan instalasi.
-	Gaji teknisi.
-	Biaya operasional perusahaan.
Fitur yang tersedia :
-	Menambah transaksi.
-	Mengedit transaksi.
-	Menghapus transaksi.
-	Menghitung total pemasukan dan pengeluaran.
-	Menghitung saldo kas secara otomatis.

2.5.3	Pemrosesan dan Verifikasi Bukti Pembayaran Pelanggan Secara Digital
Alur Proses : 
-	Customer mengunggah bukti transfer.
-	Sistem menyimpan bukti pembayaran.
-	Admin memverifikasi pembayaran.
-	Jika valid, status tagihan berubah menjadi Lunas.
-	Jika tidak valid, admin dapat menolak dan memberikan alasan.
Manfaat : 
-	Mempercepat proses konfirmasi pembayaran. 
-	Mengurangi kesalahan pencatatan. 
-	Riwayat pembayaran tersimpan secara digital.

2.5.4	Manajemen inventaris alat dan bahan produksi yang tersedia di gudang secara otomatis
Sistem harus mengelola seluruh inventaris yang digunakan dalam proses instalasi maupun perbaikan jaringan.
Data inventari meliputi : 
-	Nama barang. 
-	Kategori barang. 
-	Jumlah stok. 
-	Kondisi barang.
-	Tanggal masuk.
Fungsi sistem : 
-	Menambah barang baru.
-	Mengurangi stok saat barang digunakan.
-	Menambah stok saat pembelian.
-	Memberikan notifikasi apabila stok hampir habis.
-	Menampilkan riwayat penggunaan barang.

2.5.5	Pendataan performa teknis berdasarkan kecepatan penanganan gangguan (SLA)
Sistem harus mencatat seluruh aktivitas penanganan gangguan oleh teknisi berdasarkan standar Service Level Agreement (SLA).
Data yang dicatat : 
-	Waktu laporan gangguan masuk.
-	Teknisi yang menangani.
-	Waktu mulai pengerjaan.
-	Waktu selesai.
-	Durasi penyelesaian.
-	Status penyelesaian.
Tujuan :
-	Mengukur kinerja teknisi.
-	Mengetahui apakah pekerjaan selesai sesuai target SLA.
-	Menjadi dasar evaluasi performa teknisi.

2.5.6	Generasi laporan otomatis untuk keuangan dan performa operasional perusahaan
Sistem harus dapat menghasilkan laporan secara otomatis berdasarkan data yang telah tersimpan di database.
Jenis laporan yang dihasilkan :
Laporan keuangan : 
-	Total pemasukan. 
-	Total pengeluaran. 
-	Saldo kas. 
-	Pembayaran pelanggan. 
-	Piutang pelanggan. 
Laporan Operasional
-	Jumlah pelanggan aktif. 
-	Jumlah gangguan. 
-	Jumlah pekerjaan teknisi. 
-	Tingkat keberhasilan penyelesaian gangguan. 
-	Performa teknisi berdasarkan SLA. 
-	Kondisi stok inventaris. 
Keunggulan fitur ini:
-	Mempercepat pembuatan laporan. 
-	Mengurangi kesalahan perhitungan manual. 
-	Memudahkan pimpinan dalam mengambil keputusan. 
-	Laporan dapat dicetak atau diunduh sesuai kebutuhan.
2.6	Logika system
Data mengalir secara berurutan dimulai dari pendaftaran mandiri oleh pelanggan. Validasi akun oleh Admin memicu kemampuan pelanggan untuk memilih paket layanan yang secara otomatis menggenerasi tagihan. Setelah bukti bayar diverifikasi, sistem mengirimkan notifikasi kerja kepada Teknisi. Teknisi melakukan instalasi dengan mengambil alat dari inventaris (yang secara otomatis mengurangi stok dalam sistem). Seluruh data transaksi dan durasi pengerjaan teknis kemudian diolah menjadi laporan performa dan grafik profitabilitas bagi Manajer.

 BAB III PERANCANGAN SISTEM
3.1	Use Case Diagram
Sistem memfasilitasi interaksi empat aktor terhadap fungsi inti, mencakup pembagian akses berdasarkan role (peran) yang diterapkan pada sistem login:
-	Admin: mengelola kredensial multi-role, data pelanggan (CRUD), verifikasi pembayaran, inventaris, teknisi/absensi, serta menindaklanjuti tiket kendala.
-	Teknisi: mengakses dashboard dengan kalender absensi (bersifat read-only), melihat dan memperbarui status titik jaringan, serta menerima notifikasi tiket kendala.
-	Customer: mendaftar akun secara mandiri, login untuk melihat dashboard pribadi, memilih paket bandwidth, melihat riwayat tagihan, serta melaporkan kendala jaringan.
-	Manager/Owner: memantau dashboard laporan keuangan, grafik tahunan, dan rincian pengeluaran secara interaktif.
 
3.2	 Flowchart
Flowchart berikut menggambarkan alur proses transaksi pada Sistem Administrasi Pada Penyedia Layanan Jaringan, mulai dari pelanggan melakukan pembelian jasa hingga data transaksi di baca oleh owner.
 
Alur proses transaksi dirancang sebagai berikut:
1.	Customer melakukan registrasi 
-	Calon pelanggan mengisi data diri, memilih paket internet, serta membuat username dan password untuk akun. 
2.	Admin memverifikasi data 
-	Admin memeriksa apakah data pendaftaran valid. 
-	Jika tidak valid, pendaftaran ditolak dan pelanggan harus memperbaiki data. 
-	Jika valid, proses dilanjutkan. 
3.	Sistem membuat akun pelanggan 
-	Setelah disetujui, sistem otomatis membuat akun login dan mengaktifkan data pelanggan sehingga dapat menggunakan sistem. 
4.	Pembuatan tagihan 
-	Pelanggan memilih atau mengonfirmasi paket internet, kemudian Admin membuat tagihan dengan status Belum Bayar. 
5.	Verifikasi pembayaran 
-	Admin memeriksa pembayaran yang dilakukan pelanggan. 
-	Jika belum terverifikasi, tagihan tetap berstatus Belum Bayar. 
-	Jika sudah terverifikasi, proses dilanjutkan. 
6.	Pembayaran dikonfirmasi 
-	Admin mencatat metode pembayaran (Transfer Bank, QRIS, atau Tunai), lalu status tagihan otomatis berubah menjadi Lunas. 
7.	Teknisi melakukan instalasi 
-	Setelah pembayaran lunas, teknisi memasang jaringan di lokasi pelanggan. Peralatan yang digunakan akan otomatis tercatat dan stok inventaris berkurang sesuai pemakaian. 
8.	Penanganan kendala jaringan (jika ada aduan)
-	Jika pelanggan mengalami gangguan, pelanggan membuat laporan kendala. 
-	Teknisi menerima laporan, memperbaiki masalah, lalu memperbarui status jaringan. Setelah selesai, proses kembali ke alur utama. 
9.	Laporan diperbarui otomatis 
-	Seluruh data seperti pembayaran, penggunaan inventaris, dan penanganan kendala akan dihitung secara otomatis dan masuk ke laporan sistem. 
10.	Owner memantau laporan 
-	Manager dapat melihat grafik, statistik, dan rincian laporan untuk memantau kondisi operasional serta keuangan perusahaan. 
11.	Proses selesai 
-	Seluruh aktivitas telah tercatat dalam sistem dan dapat digunakan sebagai bahan monitoring maupun pengambilan keputusan.

Proses dimulai ketika customer melakukan registrasi, lalu memilih paket dan melakukan pembayaran. Kemudian admin mencatat semua hal yg diperlukan untuk operasional seperti data pelanggan, pemasukan dan pengeluaran, dan stok alat dan bahan. Kemudian teknisi akan melakukan pemasangan dan pendistribusian bandwidth, jika ada kendala maka akan di informasikan ke teknisi, lalu manager dapat memantau laporan secara menyeluruh dan melakukan improvisasi jika di perlukan.

3.3	DFD (Data Flow Diagram)
3.3.1	Level 0 (Context Diagram)
NetSpeed Hub bertindak sebagai entitas pusat yang berinteraksi dengan empat entitas eksternal. Customer memberikan input data registrasi, pilihan paket, dan laporan kendala; menerima output status tagihan dan update tiket. Teknisi memberikan input absensi (read) dan update titik jaringan; menerima output notifikasi tiket dan status absensi. Admin menginput data master (pelanggan, inventaris, verifikasi bayar, role user); menerima output konfirmasi dan status sistem. Manager menerima output laporan keuangan dan grafik tahunan sebagai hasil akhir.
 
Aliran data antara entitas luar dengan sistem utama :
-	[Customer] (Data Pendaftaran, Bukti Bayar) [Sistem].
-	[ Sistem ] (Rincian Tagihan, Status Perbaikan) [Customer]
-	[Admin/Teknisi] (Data Inventaris, Konfigurasi Bandwidth, Absensi) [Sistem]..
-	[Sistem] (Laporan Keuangan & Performa) [Manager].

3.3.2	DFD Level 1
Berikut adalah rincian lima proses utama dalam sistem:
-	Kelola User 3 Role: memproses autentikasi dan otorisasi untuk peran Admin, Teknisi, dan Customer.
-	2.0 Kelola Pelanggan & Paket: CRUD data pelanggan beserta pemilihan paket bandwidth.
-	3.0 Kelola Tagihan & Pembayaran: generasi tagihan otomatis dan pencatatan metode pembayaran.
-	4.0 Kelola Inventaris & Stok: pelacakan stok barang beserta riwayat transaksi penambahan/pengurangan.
-	5.0 Kelola Teknisi & Absensi: pendataan teknisi dan pencatatan kehadiran harian oleh Admin.
-	6.0 Kelola Jaringan & Titik Peta: manajemen titik lokasi jaringan beserta status interaktifnya pada peta.
-	7.0 Kelola Tiket Kendala: pemrosesan laporan gangguan dari pelanggan hingga status selesai.
-	8.0 Pembuatan Laporan: agregasi seluruh data menjadi laporan dan grafik manajerial.
 
Penjelasan Alur Data : 
1.	Customer Melakukan Registrasi dan Login
Customer mengirim data registrasi ke proses 1.0 Kelola User 3 Role.
Data yang mengalir:
•	Nama 
•	Username 
•	Password 
•	Role Customer 

Kemudian data disimpan ke:
D1 User
Admin dapat mengelola dan memverifikasi data user melalui proses ini.
2. Customer Memilih Paket Internet
Setelah memiliki akun, Customer memilih paket internet melalui proses:
2.0 Kelola Pelanggan & Paket
Data yang diproses:
•	Data pelanggan 
•	Alamat 
•	Nomor HP 
•	Paket bandwidth 
Data kemudian disimpan ke:
D2 Pelanggan
Admin dapat menambah, mengubah, dan menghapus data pelanggan serta paket yang dipilih.

3. Sistem Membuat Tagihan
Berdasarkan paket yang dipilih pelanggan, proses:
3.0 Kelola Tagihan & Pembayaran
akan membuat tagihan.
Data yang tersimpan:
•	ID pelanggan 
•	Nominal tagihan 
•	Status pembayaran 
•	Metode pembayaran 
Data disimpan ke:
D3 Tagihan
Admin melakukan verifikasi pembayaran dan mengubah status menjadi Lunas apabila pembayaran telah diterima.

4. Pengelolaan Inventaris
Saat terjadi pemasangan jaringan atau perbaikan, sistem menggunakan proses:
4.0 Kelola Inventaris & Stok
Data yang dicatat:
•	Nama barang 
•	Jumlah stok 
•	Barang masuk 
•	Barang keluar 
Data disimpan pada:
D4 Barang
Setiap penggunaan alat oleh teknisi akan mengurangi stok secara otomatis.

5. Pengelolaan Teknisi dan Absensi
Admin mengelola data teknisi melalui:
5.0 Kelola Teknisi & Absensi
Data yang dicatat:
•	Data teknisi 
•	Kehadiran 
•	Status kerja 
Data disimpan ke:
D5 Teknisi
Teknisi dapat melihat data absensinya melalui proses ini.

6. Pengelolaan Jaringan dan Titik Peta
Teknisi melakukan update kondisi jaringan melalui:
6.0 Kelola Jaringan & Titik Peta
Data yang diproses:
•	Lokasi jaringan 
•	Status titik 
•	Informasi gangguan 
Data disimpan pada:
D6 Titik_Jaringan
Teknisi dapat memperbarui status jaringan secara langsung dari lapangan.

7. Penanganan Tiket Kendala
Ketika pelanggan mengalami gangguan, Customer membuat laporan melalui:
7.0 Kelola Tiket Kendala
Data yang dikirim:
•	Keluhan pelanggan 
•	Lokasi gangguan 
•	Deskripsi masalah 
Data disimpan ke:
D7 Tiket
Admin dan Teknisi dapat:
•	Melihat tiket 
•	Memproses tiket 
•	Mengubah status tiket 
•	Menandai tiket selesai 

8. Pembuatan Laporan
Semua data dari proses sebelumnya dikirim ke:
8.0 Pembuatan Laporan
Data yang diambil berasal dari:
•	D2 Pelanggan 
•	D3 Tagihan 
•	D4 Barang 
•	D5 Teknisi 
•	D6 Titik Jaringan 
•	D7 Tiket 
Sistem melakukan:
•	Perhitungan jumlah pelanggan 
•	Perhitungan pendapatan 
•	Perhitungan stok barang 
•	Statistik absensi 
•	Statistik gangguan jaringan 

9. Manager Melihat Hasil Laporan
Hasil proses 8.0 Pembuatan Laporan dikirim ke entitas:
Manager
Dalam bentuk:
•	Dashboard 
•	Grafik 
•	Statistik 
•	Laporan detail 
Manager menggunakan informasi tersebut untuk memantau kondisi operasional ISP.

3.4	 Entity Relationship Diagram (ERD)
Struktur basis data sistem terbagi menjadi dua kelompok entitas utama: entitas jaringan dan entitas operasional/transaksi.
3.4.1	Entitas Utama Jaringan
-	Perangkat (id_Perangkat, Tipe, ip_Address, Lokasi, Status).
-	Kabel/Link (id_Link, Tipe_Kabel, Panjang, Kapasitas, Perangkat_Asal, Perangkat_Tujuan).
-	Pelanggan (id_Pelanggan, Nama, Alamat, No_Telp, Email).
-	Layanan/Paket (id_Paket, Nama_Paket, Kecepatan, Harga, Deskripsi).
-	Langganan (id_Langganan, id_Pelanggan, id_Paket, Tanggal_Mulai, Status).
3.4.2	Entitas Operasional & Transaksi
-	Tiket Laporan (id_Tiket, id_Pelanggan, Deskripsi, Tanggal_Laporan, Status, id_Staff).
-	Staff (id_Staff, Nama, Spesialisasi, No_Telp).
-	Tagihan/Billing (id_Tagihan, id_Langganan, Jumlah, Tanggal_Jatuh_Tempo, Status_Bayar).
 
3.4.3	Relasi Antar Entitas
-	Satu Pelanggan dapat memiliki banyak Langganan (1:N).
-	Satu Langganan terhubung ke satu Layanan/Paket (N:1).
-	Satu Langganan dapat memiliki banyak Tagihan (1:N).
-	Satu Pelanggan dapat membuat banyak Tiket Laporan (1:N).
-	Satu Staff dapat menangani banyak Tiket Laporan (1:N).
-	Setiap Kabel/Link menghubungkan dua Perangkat sebagai titik asal dan tujuan.
 BAB 4 IMPLEMENTASI DAN PENGUJIAN SISTEM
4.1 Teknologi Yang Digunakan
Sistem NetSpeed Hub diimplementasikan menggunakan arsitektur berbasis web dengan rincian sebagai berikut:
•	Backend: Python dengan framework Flask, dipilih karena sifatnya yang minimal dan mudah dipahami untuk pengembangan bertahap.
•	Database: SQLite, dipilih karena tidak memerlukan instalasi server terpisah dan cukup untuk skala pengujian serta demonstrasi.
•	Frontend: HTML, CSS dengan gaya glassmorphism (efek kaca buram dan gradasi warna biru-ungu), serta JavaScript untuk elemen interaktif.
•	Pustaka Eksternal: Chart.js untuk visualisasi grafik, Leaflet.js untuk peta interaktif, dan Tabler Icons untuk ikonografi antarmuka.
Penggunaan platform web dipilih karena mendukung integrasi terpusat dan aksesibilitas lintas perangkat, yang krusial bagi teknisi di lapangan untuk melakukan sinkronisasi data secara real-time dengan gudang inventaris dan pusat administrasi.

4.2 Struktur Data Base
Struktur tabel database sebagaimana telah diimplementasikan adalah sebagai berikut:
Nama Tabel	Primary Key	Deskripsi Tujuan
admin	id_admin	Menyimpan kredensial akun staf (Admin dan Teknisi), termasuk kolom role dan referensi ke data teknisi.
pelanggan	id_pelanggan	Menyimpan profil pelanggan: nama, nomor HP, paket bandwidth, dan status keaktifan.
user_pelanggan	id_user	Menyimpan kredensial login mandiri milik pelanggan, terhubung ke satu data pelanggan.
tagihan	id_tagihan	Mencatat tagihan per pelanggan: jumlah, jatuh tempo, status bayar, dan metode pembayaran.
teknisi	id_teknisi	Menyimpan data teknisi lapangan: nama, spesialisasi, dan kontak.
absensi	id_absensi	Mencatat kehadiran harian setiap teknisi, diinput oleh Admin.
barang	id_barang	Menyimpan data inventaris alat/bahan beserta jumlah stok dan ambang batas minimum.
riwayat_barang	id_riwayat	Mencatat setiap transaksi penambahan/pengurangan stok sebagai riwayat historis.
titik_jaringan	id_titik	Menyimpan koordinat titik jaringan (terpasang, rusak, area aktif) untuk peta interaktif.
tiket_kendala	id_tiket	Mencatat laporan kendala dari pelanggan beserta status penanganannya.
4.3	Implementasi Sistem Role-Based Access
Salah satu capaian utama implementasi adalah penerapan sistem akses berbasis peran (role-based access control), di mana satu basis data dan satu aplikasi melayani tiga jenis pengguna dengan tampilan dan kewenangan berbeda:
Admin	Teknisi	Customer/Pelanggan
Akses penuh ke seluruh modul sistem	Dashboard, Kalender Absensi (read-only), Peta Jaringan	Dashboard pribadi, Riwayat Tagihan, Lapor Kendala
CRUD Pelanggan, Tagihan, Inventaris, Teknisi	Tambah & ubah status titik jaringan	Tidak dapat melihat data pelanggan lain
Tindak lanjut tiket kendala & verifikasi bayar	Tidak dapat mengabsen diri sendiri (anti penyalahgunaan)	Mendaftar mandiri tanpa perlu login terlebih dahulu

Mekanisme keamanan diterapkan pada setiap route melalui pemeriksaan session berbasis role (contoh: pemeriksaan session.get("role") != "admin" pada modul yang khusus untuk Admin), memastikan Teknisi maupun Customer tidak dapat mengakses halaman di luar kewenangannya meskipun mengetik alamat URL secara langsung. Penghapusan data pelanggan oleh Admin juga dirancang untuk menghapus seluruh data terkait (akun login, tagihan, tiket) guna menjaga integritas referensial basis data.
4.4	Implementasi Antarmuka (Prototype UI)
Antarmuka sistem dirancang dengan tema visual glassmorphism yang konsisten di seluruh halaman, mencakup tiga dashboard utama sesuai peran pengguna, serta halaman login dan pendaftaran mandiri.
Dashboard Admin
  
Dashboard Teknisi
 




Login dan Pendaftaran Mandiri
 
Dashboard Pelanggan
 

4.4.1	User Flow
-	Admin: Login → Dashboard → Akses modul (Pelanggan/Tagihan/Inventaris/Teknisi/Jaringan) → Update database → Notifikasi otomatis pada sidebar.

-	Customer: Pendaftaran mandiri → Verifikasi Admin → Login → Pilih paket → Akses tagihan dan pelaporan gangguan → Notifikasi saat status tiket berubah.

-	Teknisi: Login → Dashboard (kalender absensi & notifikasi tiket) → Akses Jaringan → Update status titik atau tambah titik baru.


4.5	Pengujian Sistem
Verifikasi fungsionalitas dilakukan melalui metode black-box testing untuk memastikan seluruh kebutuhan fungsional (FR-1 hingga FR-6) terpenuhi. Pengujian dilakukan secara menyeluruh terhadap setiap peran pengguna, dengan hasil sebagai berikut:
-	Autentikasi: pengujian akses langsung tanpa login pada seluruh halaman terlindungi berhasil ditolak dan dialihkan ke halaman login.
-	Isolasi Akses Peran: akun Teknisi dan Customer yang mencoba mengakses alamat URL modul Admin secara langsung berhasil ditolak sistem.
-	Integritas Data: penghapusan data pelanggan oleh Admin terbukti turut menghapus akun login dan data terkait tanpa meninggalkan data yatim.
-	Akurasi Inventaris: pengurangan dan penambahan stok terbukti akurat serta tercatat pada riwayat transaksi sesuai jumlah yang diinput.
-	Sinkronisasi Notifikasi: perubahan status tiket oleh Admin terbukti secara konsisten memperbarui angka notifikasi pada sisi Teknisi maupun Customer.

BAB 5 PENUTUP
5.1	Kesimpulan
NetSpeed Hub merupakan solusi arsitektural yang komprehensif bagi NetSpeed Solutions dalam mengatasi inefisiensi akibat manajemen manual. Dengan mengotomatisasi siklus administrasi dan manajemen jaringan, sistem ini mampu mempercepat waktu aktivasi layanan hingga 90% (dari 2 hari menjadi 2 jam). Digitalisasi data ini tidak hanya menyelesaikan masalah ketidakteraturan informasi, tetapi juga memberikan transparansi finansial yang fundamental bagi pemilik perusahaan melalui pelaporan otomatis.
Lebih lanjut, penerapan sistem role-based access control dengan tiga peran (Admin, Teknisi, Customer) membuktikan bahwa satu platform terpadu dapat melayani kebutuhan yang berbeda-beda secara aman dan terisolasi, tanpa memerlukan tiga aplikasi terpisah. Penambahan fitur pendukung seperti peta interaktif untuk monitoring jaringan, kalender absensi, dan sistem notifikasi berbasis status turut memperkuat posisi sistem ini sebagai solusi yang siap digunakan dalam skala operasional nyata.

5.2	Saran
Untuk pengembangan tahap selanjutnya, disarankan beberapa hal sebagai berikut:
-	Pengintegrasian API langsung dengan perangkat router untuk otomatisasi manajemen bandwidth secara programatik.
-	Penguatan lapisan keamanan data, termasuk hashing password dan validasi input yang lebih ketat pada seluruh form.
-	Optimalisasi database secara berkala guna mendukung skalabilitas yang melampaui target awal 5.000 pelanggan.
-	Integrasi payment gateway sungguhan untuk mendukung pembayaran daring secara langsung pada tahap produksi.
-	Pengembangan aplikasi mobile khusus untuk Teknisi guna mempermudah input data di lapangan tanpa memerlukan koneksi desktop.





