# **Data Public Transportation Transaction Transjakarta**

## **Latar Belakang**
TransJakarta adalah salah satu operator layanan transportasi publik terkemuka di Jakarta, yang mengoperasikan sistem Bus Rapid Transit (BRT). Dalam upaya untuk meningkatkan pendapatan dari pemasangan iklan di tiap halte, TransJakarta ingin merekrut seorang data analyst. Data analyst ini akan bertugas untuk menganalisis, dan menyajikan data terkait dengan persebaran penumpang serta penggunaan kartu berdasarkan corridor,gender,dan range Age.

## **Pernyataan Masalah**

Perusahaan Transjakarta ingin mengetahui persebaran banyaknya penumpang berdasarkan rute dan waktu melalui data yang ada pada bulan April. Informasi ini akan membantu perusahaan untuk **meningkatkan pendapatan melalui pemasangan iklan**

Sebagai seorang *data analyst*, kita akan mencoba menjawab pertanyaan berikut:

**Bagaimana hubungan data penumpang dengan penggunaan kartu bank dalam meningkatkan pendapatan dari pemasangan iklan di setiap halte TransJakarta**

Dataset bersumber dari kaggle dan dapat diunduh pada Link : https://www.kaggle.com/datasets/dikisahkan/transjakarta-transportation-transaction?select=dfTransjakarta.csv.

Data set ini berisi informasi terkait tentang Corridor,Jurusan,dan Card pembayaran yang digunakan oleh penumpang Transjakarta yang nanti dapat kita analisa untuk melihat persebaran Card pembayaran dari berbagai jurusan dan Corridor.  
Terdapat 22 kolom pada dataset Transjakarta ini yaitu :

- transID: ID unik transaksi untuk setiap transaksi.
- payCardID: Identifikasi utama pelanggan. Kartu yang digunakan pelanggan sebagai tiket masuk dan keluar.
- payCardBank: Nama penerbit bank kartu pelanggan.
- payCardName: Nama pelanggan yang terdapat di dalam kartu.
- payCardSex: Jenis kelamin pelanggan yang terdapat di dalam kartu.
- payCardBirthDate: Tahun kelahiran pelanggan.
- corridorID: ID Koridor / ID Rute sebagai kunci untuk pengelompokan rute.
- corridorName: Nama Koridor / Nama Rute yang berisi titik awal dan akhir untuk setiap rute.
- direction: 0 untuk Pergi, 1 untuk Kembali. Arah rute.
- tapInStops: ID Titik Tap In (masuk) untuk mengidentifikasi nama halte.
- tapInStopsName: Nama Halte Titik Tap In di mana pelanggan melakukan tap masuk.
- tapInStopsLat: Garis lintang Halte Titik Tap In.
- tapInStopsLon: Garis bujur Halte Titik Tap In.
- stopStartSeq: Urutan berhenti, mulai dari yang pertama, kedua, dst. Terkait dengan arah.
- tapInTime: Waktu tap masuk. Tanggal dan waktu.
- tapOutStops: ID Titik Tap Out (keluar) untuk mengidentifikasi nama halte.
- tapOutStopsName: Nama Halte Titik Tap Out di mana pelanggan melakukan tap keluar.
- tapOutStopsLat: Garis lintang Halte Titik Tap Out.
- tapOutStopsLon: Garis bujur Halte Titik Tap Out.
- stopEndSeq: Urutan berhenti, mulai dari yang pertama, kedua, dst. Terkait dengan arah.
- tapOutTime: Waktu tap keluar. Tanggal dan waktu.
- payAmount: Jumlah yang dibayar oleh pelanggan. Beberapa gratis. Beberapa tidak.

Setelah kita melakukan data cleaning dan telah melakukan suatu analisa berdasarkan Kartu bank yang digunakan,Age Group,tapInDay,dan Gender kita mendapatkan suatu kesimpulan dan dapat memberikan rekomendasi action pada setiap Bank.

## **Conclusion and Recommendations**

### **Conclusion**

Dari Hasil analisa diatas kita dapat menyumpulkan bahwa : 
* Mayoritas pengguna Transjakarta memakai kartu bank DKI dan Pengguna Transjakarta terbanyak adalah Perempuan.
* Transjakarta banyak digunakan oleh kalangan pelajar dan pekerja dengan Range Usia 18-60 tahun.
* Dari hasil analisa diatas berdasarkan tapInDay dapat disimpulkan bahwa untuk setiap corridor memiliki kepadatan pada saat hari Senin - Jumat (Weekday).

Persebaran Berdasarkan Mayoritas Kartu yang digunakan pada setiap corridor :  

* Untuk corridor yang menggunakan kartu bank **DKI** sebagai kartu bank yang mayoritas ada pada corridor 3B, 8C, 11P, JAK.06, JAK.42, 2, 1T, JAK.08 dengan proporsi gender terbanyaknya adalah Female.
* Untuk corridor yang menggunakan kartu bank **emoney** sebagai kartu bank yang mayoritas ada pada corridor 6H, JAK.64, JAK.49, T11, 6D, JAK.72, 13, S31, 5D, JAK.39 dengan rata-rata gender terbanyaknya adalah Female.
* Untuk corridor yang menggunakan kartu bank **brizzi** sebagai kartu bank yang mayoritas ada pada corridor M7B, 10K, 1H, 1F, 5B, S11, 3H, JAK.28 dengan rata-rata gender terbanyaknya adalah Female.
* Untuk corridor yang menggunakan kartu bank **flazz** sebagai kartu bank yang mayoritas ada pada corridor 10D, JAK.48B, JAK.106, B11, 8M, 7Q, 10B, 9F dengan rata-rata gender terbanyaknya adalah Female.
* Untuk corridor yang menggunakan kartu bank **BNI** sebagai kartu bank yang mayoritas ada pada corridor S21, 2F, JAK.60, JAK.04 dengan rata-rata gender terbanyaknya adalah Female.

### **Recommendations**

* Transjakarta dapat bekerja sama dengan bank DKI,Mandiri,BCA,BNI,BRI untuk memberikan Informasi dari hasil analisa diatas kepada setiap bank untuk merekomendasi berupa pemasangan iklan di beberapa corridor yang telah dianalisa berdasarkan mayortias penggunaan bank di setiap corridornya,dengan segment market berdasarkan Gender,Hari dan Usia,Oleh karena itu Transjakarta dapat meningkatkan pendapatan dari setiap bank untuk pemasangan iklan di setiap corridornya.


  Untuk Data Visualisasi dapat di akses lewat link dibawah ini :
  https://public.tableau.com/app/profile/adlan.muammar.s/viz/Transjakarta_Analysis_16984081321400/Transjakarta?publish=yes
