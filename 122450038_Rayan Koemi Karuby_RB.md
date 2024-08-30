# VDI
# 1.	Pendahuluan
Visualisasi data adalah alat yang sangat kuat untuk mengubah data kompleks menjadi representasi visual, agar memudahkan orang untuk memahami informasi tersebut dengan mudah. Seiring dengan berkembangnya zaman, visualisasi data berperan penting untuk memberikan gambaran dan wawasan yang jelas. Visualisasi data telah berkembang pesat dengan bantuan dari berbagai bidang. D3, Vega-Lite, dan Tableau membuat pembuatan dan interaksi visualisasi menjadi lebih mudah dan efisien. Visualisasi data mengikuti proses bertahap, mulai dari mengimpor dan menyiapkan, memetakan dan merendernya menjadi suatu bentuk visual. Selain itu, sistem akan selalu dikembangkan untuk merekomendasikan visualisasi terbaik dalam membantu pengguna.

# 2.	Spesifikasi Visualisasi
## 2.1	Spesifikasi dari Data Visualisasi
- Data, data yang perlu divisualisasikan dan operasi untuk menngubah data.
- Tanda atau petunjuk visual, seperti tipe, ukuran, legenda, dan property lain.
- Pemetaan, yaitu menghubungkan data dengan tanda yang sesuai.

## 2.2	Kategorisasi dari Bahasa Visualisasi Data
Bahasa visualisasi data dapat dikategorikan berdasarkan ekspresivitas dan kemudahan penggunaan. Bahasa dengan tingkatan yang lebih rendah, seperti Prefuse dan D3, memberikan kontrol yang lebih detail namun lebih kompleks. Sebaliknya, bahasa dengan tingkat yang lebih tinggi, seperti ggplot2 dan Vega-Lite, membuat visualisasi lebih sederhana dan dapat mengelola detail secara otomatis, sehingga lebih mudah digunakan.
## 2.3	Aplikasi Visual Berdasarkan GUI
Alat-alat yang berbasis GUI juga digunakan untuk melakukan visualisasi, seperti Excel, Qlik, Tableau, dan Google Sheets. Alat-alat tersebut membantu untuk membuat visualisasi dengan antarmuka yang intuitif, yang mana kurang fleksibel dibandingkan dengan bahasa visualisasi deklaratif. Alat-alat ini penting untuk membuat visualisasi yang efisien.
## 2.4	Spesifikasi yang Tidak Sepenuhnya Jelas
Seringkali pengguna tidak mengetahui seluruh aspek dari data yang digunakan karena ukuran yang besar. Oleh karena itu, sistem visualisasi harus perlu mendukung spesifikasi yang tidak sepenuhnya jelas. Ada beberapa cara untuk ini, yaitu dengan berbasis referensi, kata kunci, dan bahasa alami. Sistem-sistem ini membantu pengguna mendapatkan visualisasi yang relevan tanpa harus memahami detail struktur data secara mendalam.

# 3.	Pendekatan Efisien untuk Visualisasi Data
Pendekatan yang efisien difokuskan kepada bagaimana data diproses dan spesifikasi visualisasinya menghasilkan visualisasi yang interaktif. Ada dua komponen utama, yaitu manipulasi data dan pemetaan.

# 3.1	Visualisasi yang Tepat
Visualisasi yang dihasilkan secara akurat dan cepat merupakan visualisasi yang tepat. Menerjemahkan kueri visualisasi menjadi kueri SQL adalah salah satu cara memanfaatkan system basis data. Sistem seperti DeepEye, Polaris, dan SeeDB juga dapat digunakan. Dengan melakukan pemetaan bahasa visualisasi dengan bahasa SQL, visualisasi dapat dilakukan dengan cepat.

Dengan menerjemahkan kueri ini, ada beberapa kekurangan, seperti adanya fungsi berulang yang akhirnya tidak optimal. Hal ini dapat diatasi dengan melakukan penggabungan antara pengambilan data dan rendering. Penggabungan dapat dilakukan dengan menggunakan Ermac, yaitu suatu system manajemen visualisasi data yang menyediakan beberapa teknik optimasi.
# 3.2	Estimasi Visualisasi
Saat data terlalu besar dan kuerinya kompleks, maka sulit untuk memberikan visualisasi yang tepat. AQP dapat digunakan untuk mengatasi hal ini. AQP membantu pembuatan visualisasi yang interaktif dengan menggunakan subset data yang merepresentasikan dengan jelas.

Ada visualisasi data yang melakukan pengambilan sampel secara incremental dengan cara kerja system yang menhasilkan visualisasi estimasi berdasarkan data dengan cepat beriringan dengan meningkatkan ukuran sampel guna meningkatkan kualitas visualisasi. Pengguna dapat menghentikan proses jika dirasa kualitas visualisasi sudah cukup.
# 3.3	Visualisasi Progresif
Visualisasi progresif merupakan visualisasi yang dilakukan secara bertahap dan menyempurnakannya seiring dengan beratmbahnya data yang diproses. Visualisasi progresif  cocok digunakan untuk data yang besar agar pengguna dapat melihat hasil sementara menunggu visualisasi akhir.

Visualisasi progresif kadang menggunakan agregasi hierarkis. Agregasi hierarkis mengorganisir data dengan hierarkis sehingga pengguna dapat mengakses data secara lebih terstruktur. imMens merupakan system yang menerapkan agregasi hierarkis, di  mana data dipartisi dan pengguna dapat menjelajahi data dengan tingkat resolusi yang berbeda dengan cara zoom in dan out.
# 4.	Studi Kasus
## 4.1	Kyrix
Kyrix merupakan suatu system yang dapat diskalakan dan dapat menghasilkan spesifikasi visalisasi yang deklaratif di bagian depan dan pemrosesan visualisasi. Pengguna dapat melakukan skala memperbesar dan memperkecil dengan dua opsi, yaitu kanvas dan lompatan. Pada kanvas terdapat visualisasi statis, sedangkan padaa lompatan digunakan untuk memnentukan sumber dan tujuan kanvas dan jenis transisi yang akan digunakan.

Kyrix mempunyai dua elemen penting, yaitu granulitas pengambilan dan pengindeksan. Kyrix membagi data mentah menjadi suatu ubin data statis dengan  ukuran yang tidak berubah. Kyrix menerapkan indeks B-tree pada ID ubin data agar dapat melakukan pengambilan dengan cepat.

## 4.2	Tableau
Mesin data Tableau, yaitu TDE dan Hyper dapat mendukung pembuatan visualisasi yang efisien, berfokus kepada penyimpanan berbasis kolom, kompresi data, dan perhitungan paralel. TDE menggunakan penyimpanan berbasis kolom untuk mengurangi biaya yang tinggi dari basis data. 

Hyper adalah sistem memori yang efisien sebagai sebuah mesin data untuk semua veris dari Tabelau. Hyper membantu dalam melakukan pembaruan, ekstraksi kueri, dan penggabungan basis data.

# 5.	Rekomendasi Visualisasi
Proses visualisasi data merupakan proses yang iteratif,sehingga pengguna harus terus menerus melakukan setiap langkah tidak secara otomatis agar dapat melakukan pembaruan, karena masalah ini, sistem rekomendasi visualisasi yang otomatis berfungsi untuk meringankan pekerjaan pengguna dengan cara menyediakan saran visualisasi.

## 5.1	Spesifikasi Tidak Lengkap
Input dari spesifikasi visualisasi parsial dari pengguna diterima oleh sistem rekomendasi visualisasi. Beberapa contohnya adalah, APT menerima tujuan melihat data dari pengguna sebelum dilakukan rekomendasi, pengguna memilih satu kolom yang diminati sebelum rekomendasi dilakukan di Voyager, DeepEye menerima kata kunci dari pengguna terlebih dahulu sebelum dilakukan rekomendasi.

Solusi berbasis aturan dan solusi pembelajaran mesin merupakan dua pendekatan yang diterapkan dalam rekomendasi visualisasi. Sistem rekomendasi berbasis aturan mengurutkan kandidat visualisasi yang akan digunakan berdasarkan aturan yang sudah ditentukan, seperti suatu grafik pie hanya teriri dari beberapa blok, tidak banyak karena menurut persepsi manusai hal terebut dikatakan kurang bagus. Voyager, Show Me, dan DeepEye mengembangkan aturan dengan persepsi yang lebih beragam dan juga jenis data yang kaya.
## 5.2	Pembelajaran Mesin 
Pembelajaran mesin dan deep learning berkembang dengan pesat, sekarang banyak sistem rekomendasi visualisasi yang berbasis pembelajaran mesin. Sistem ini menggunakan data pelatihan dari crowdsourcing daan web, lalu melatih model ynag didapat. Model tersebut memperlajari fungsi dari data pelatihan sehingga dapat menentukan visualisasi mana yang lebih baik.

Salah satus sistem yang mengekspresikan presferensi menggunakan perangkat lunak adaalah Draco. Draco memiliki bobot yang akan menunjukkan penalty apabila visualisasi melanggar suatu Batasan yang ditentukan. DeepEye menghasilkan Solusi dibantu dengan pembelajaraan mesin yang mengumpulkan pengetahuan desain visualisasi secara otomatis, namun dengan mempertimbangkan atiraan yang sudah ditentukan.
	

	

