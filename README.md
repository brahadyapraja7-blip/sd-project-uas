# Nama Kelompok
Dewa Ngakan Made Rasta Baladika Ak (2501010074)

Wayan Andhika Darma Putra (2501010070)

I Kadek Brahadya Praja Nugraha (2501010093)

# Laporan DSS Dalam pemilihan kost

## BAB I Pendahuluan 

### 1.1 Latar Belakang

Pemilihan tempat kost merupakan salah satu keputusan penting bagi mahasiswa, terutama mahasiswa perantauan. Banyaknya pilihan kost dengan berbagai harga, lokasi, dan fasilitas sering kali membuat calon penghuni kesulitan menentukan kost yang paling sesuai dengan kebutuhan mereka. Oleh karena itu, diperlukan suatu Sistem Pendukung Keputusan (Decision Support System/DSS) yang dapat membantu proses pemilihan kost secara lebih efektif dan terstruktur.

Dalam penelitian ini, digunakan struktur data Directed Graph untuk merepresentasikan hubungan antara pengguna, kriteria pemilihan, dan alternatif kost. Selanjutnya, algoritma Breadth First Search (BFS) digunakan untuk menelusuri graph dan menemukan rekomendasi kost berdasarkan kriteria yang dipilih pengguna. Dengan adanya sistem ini, diharapkan proses pemilihan kost menjadi lebih mudah, cepat, dan akurat serta dapat menunjukkan penerapan nyata struktur data graph dalam pengambilan keputusan.

### 1.2 Rumusan Masalah

1. Bagaimana merancang Sistem Pendukung Keputusan (DSS) untuk membantu mahasiswa dalam memilih kost sesuai kebutuhan dan preferensi?


2. Bagaimana mengimplementasikan struktur data Directed Graph untuk merepresentasikan hubungan antara kriteria pemilihan dan alternatif kost?


3. Bagaimana menerapkan algoritma Breadth First Search (BFS) dalam proses pencarian dan rekomendasi kost?


4. Bagaimana menampilkan hasil rekomendasi kost secara interaktif dan mudah dipahami oleh pengguna?

### 1.3 Tujuan

Adapun tujuan dari pembuatan Sistem Pendukung Keputusan (DSS) Pemilihan Kost ini adalah:
1). Merancang sistem yang dapat membantu pengguna dalam memilih kost sesuai dengan kebutuhan dan preferensi yang diinginkan.
2). Mengimplementasikan struktur data Directed Graph untuk merepresentasikan hubungan antara kriteria dan alternatif kost.
3). Menerapkan algoritma Breadth First Search (BFS) dalam proses pencarian dan rekomendasi kost.
4). Menampilkan hasil rekomendasi kost secara efektif dan mudah dipahami oleh pengguna.

### 1.4 Manfaat

Sistem Pendukung Keputusan (DSS) Pemilihan Kost ini diharapkan dapat membantu pengguna dalam memilih kost yang sesuai dengan kebutuhan dan preferensinya secara lebih cepat, mudah, dan terstruktur. Selain itu, sistem ini menjadi sarana penerapan struktur data Directed Graph dan algoritma Breadth First Search (BFS) dalam menyelesaikan permasalahan nyata, sehingga dapat meningkatkan pemahaman mahasiswa mengenai implementasi graph dalam pengambilan keputusan. Sistem ini juga dapat menjadi dasar pengembangan aplikasi rekomendasi yang lebih kompleks dengan penambahan kriteria, data, maupun fitur pendukung lainnya untuk menghasilkan rekomendasi yang lebih optimal.


## bab 2 Dasar teori

### 2.1 Struktur Data Graph

Graph merupakan salah satu struktur data non-linear yang digunakan untuk merepresentasikan hubungan antar objek. Graph terdiri dari vertex (node) sebagai representasi objek atau entitas dan edge (sisi) sebagai penghubung antar vertex. Struktur data graph banyak digunakan dalam berbagai bidang, seperti jaringan komputer, media sosial, sistem navigasi, dan sistem rekomendasi karena mampu menggambarkan hubungan antar data secara efektif. Berdasarkan arah hubungan antar vertex, graph dibedakan menjadi Undirected Graph (graf tidak berarah) dan Directed Graph (graf berarah), di mana setiap edge pada Directed Graph memiliki arah tertentu dari satu vertex ke vertex lainnya.

Dalam penelitian ini, digunakan Directed Graph untuk merepresentasikan hubungan antara pengguna, kriteria pemilihan kost, dan alternatif kost yang tersedia. Node digunakan untuk menggambarkan pengguna, kriteria, dan kost, sedangkan edge digunakan untuk menunjukkan hubungan antar node tersebut. Dengan model graph ini, proses pencarian dan rekomendasi kost dapat dilakukan secara lebih terstruktur menggunakan algoritma graph, sehingga membantu pengguna dalam memperoleh rekomendasi kost yang sesuai dengan kebutuhan dan preferensinya.

###  2.2 Decision Support System (DSS)

Decision Support System (DSS) atau Sistem Pendukung Keputusan adalah sistem berbasis komputer yang dirancang untuk membantu pengguna dalam proses pengambilan keputusan dengan memanfaatkan data, model, dan metode tertentu. DSS tidak menggantikan peran pengambil keputusan, melainkan memberikan informasi, analisis, dan rekomendasi yang dapat digunakan sebagai bahan pertimbangan dalam menentukan keputusan yang terbaik. Sistem ini banyak diterapkan dalam berbagai bidang, seperti pendidikan, bisnis, kesehatan, transportasi, dan sistem rekomendasi.

Dalam penelitian ini, DSS digunakan untuk membantu pengguna dalam memilih kost yang sesuai dengan kebutuhan dan preferensinya. Sistem akan mengolah hubungan antara kriteria pemilihan dan alternatif kost yang direpresentasikan dalam bentuk graph, kemudian menghasilkan rekomendasi berdasarkan proses pencarian menggunakan algoritma Breadth First Search (BFS). Dengan adanya DSS ini, proses pemilihan kost menjadi lebih mudah, cepat, dan terstruktur sehingga pengguna dapat mengambil keputusan dengan lebih efektif.

### 2.3 Algoritma Breadth First Search (BFS)

Breadth First Search (BFS) merupakan salah satu algoritma pencarian pada struktur data graph yang bekerja dengan cara menelusuri setiap node secara bertahap berdasarkan tingkat kedekatannya dari node awal. BFS menggunakan struktur data queue (antrian) untuk menyimpan node yang akan dikunjungi sehingga proses pencarian dilakukan secara melebar (level by level) sebelum berpindah ke tingkat berikutnya. Algoritma ini banyak digunakan untuk pencarian jalur, penelusuran graph, dan pencarian solusi dalam berbagai permasalahan yang direpresentasikan menggunakan graph.

Dalam penelitian ini, algoritma BFS digunakan untuk menelusuri hubungan antara kriteria yang dipilih pengguna dengan alternatif kost yang tersedia pada Directed Graph. Proses pencarian dimulai dari node kriteria yang dipilih, kemudian BFS akan mengunjungi node-node yang terhubung hingga menemukan alternatif kost yang sesuai. Penggunaan BFS dipilih karena mampu melakukan pencarian secara sistematis dan efisien pada graph. Secara umum, kompleksitas waktu BFS adalah O(V + E), di mana V merupakan jumlah vertex (node) dan E merupakan jumlah edge (sisi), sedangkan kompleksitas ruangnya adalah O(V). Dengan karakteristik tersebut, BFS sesuai digunakan sebagai algoritma utama dalam Sistem Pendukung Keputusan Pemilihan Kost.

## BAB III Analisis dan perancangan

### 3.1 Analisis Masalah

Pemilihan kost merupakan salah satu permasalahan yang sering dihadapi oleh mahasiswa, terutama mahasiswa perantauan. Banyaknya pilihan kost yang tersedia dengan berbagai harga, lokasi, dan fasilitas membuat proses pemilihan menjadi cukup sulit. Calon penghuni harus mempertimbangkan berbagai kriteria, seperti biaya sewa yang terjangkau, jarak yang dekat dengan kampus, serta fasilitas pendukung seperti WiFi dan area parkir. Jika dilakukan secara manual, proses pencarian dan perbandingan berbagai alternatif kost membutuhkan waktu yang cukup lama dan berpotensi menghasilkan keputusan yang kurang optimal.

Berdasarkan permasalahan tersebut, diperlukan sebuah Sistem Pendukung Keputusan (DSS) yang mampu membantu pengguna dalam menentukan kost yang sesuai dengan kebutuhan dan preferensinya. Pada sistem yang dirancang, hubungan antara pengguna, kriteria pemilihan, dan alternatif kost direpresentasikan menggunakan Directed Graph. Setiap kriteria akan terhubung dengan alternatif kost yang memenuhi kriteria tersebut. Selanjutnya, algoritma Breadth First Search (BFS) digunakan untuk menelusuri graph dan menemukan rekomendasi kost berdasarkan pilihan pengguna. Dengan pendekatan ini, proses pemilihan kost dapat dilakukan secara lebih cepat, terstruktur, dan mudah dipahami sehingga membantu pengguna dalam mengambil keputusan yang lebih tepat.

### 3.2 Desain Graph
Pada sistem yang dirancang, graph digunakan untuk merepresentasikan hubungan antara pengguna, kriteria pemilihan kost, dan alternatif kost yang tersedia. Jenis graph yang digunakan adalah Directed Graph (graf berarah), di mana setiap hubungan memiliki arah tertentu dari satu node ke node lainnya. Node pada graph terdiri dari node pengguna, node kriteria, dan node alternatif kost, sedangkan edge digunakan untuk menunjukkan hubungan antar node tersebut.
Dalam desain graph ini, pengguna dapat memilih satu atau lebih kriteria yang diinginkan, seperti Murah, Dekat Kampus, dan WiFi. Setiap kriteria kemudian dihubungkan dengan alternatif kost yang memenuhi kriteria tersebut.

### 3.3 Flowchart
<img width="1024" height="1536" alt="WhatsApp Image 2026-06-05 at 12 31 57" src="https://github.com/user-attachments/assets/22eaaec1-6d8d-429d-90af-7afb0bcf9993" />


### 3.4 use case
<img width="1536" height="1024" alt="WhatsApp Image 2026-06-05 at 12 31 57" src="https://github.com/user-attachments/assets/8adb5baa-978f-4a6c-a7de-f8e1ea7a490a" />

### 3.5 Struktur Node dan Edge

Pada Sistem Pendukung Keputusan (DSS) Pemilihan Kost, struktur graph dibangun menggunakan node (vertex) dan edge (sisi) untuk merepresentasikan hubungan antara pengguna, kriteria pemilihan kost, dan alternatif kost yang tersedia. Node yang digunakan terdiri dari User, Murah, Dekat Kampus, WiFi, Kost A, Kost B, Kost C, dan Kost D. Node User merepresentasikan pengguna sistem, node Murah, Dekat Kampus, dan WiFi merepresentasikan kriteria yang dapat dipilih pengguna, sedangkan Kost A, Kost B, Kost C, dan Kost D merupakan alternatif kost yang direkomendasikan oleh sistem.

Hubungan antar node direpresentasikan menggunakan edge yang bersifat berarah (directed). Node User terhubung ke node Murah, Dekat Kampus, dan WiFi sebagai kriteria yang dapat dipilih. Selanjutnya, node Murah terhubung ke Kost A dan Kost C, node Dekat Kampus terhubung ke Kost B dan Kost C, serta node WiFi terhubung ke Kost A dan Kost D. Dengan total 8 node dan 9 edge, struktur Directed Graph ini memungkinkan algoritma Breadth First Search (BFS) melakukan penelusuran hubungan antar node secara sistematis untuk menghasilkan rekomendasi kost yang sesuai dengan kebutuhan dan preferensi pengguna.

## BAB IV Implementasi 

### 4.1 Implementasi Program

Implementasi program dilakukan menggunakan bahasa pemrograman Python dengan framework Streamlit sebagai antarmuka pengguna. Sistem ini dirancang sebagai Decision Support System (DSS) untuk membantu pengguna dalam memilih kost berdasarkan kriteria tertentu. Hubungan antara pengguna, kriteria, dan alternatif kost direpresentasikan menggunakan Directed Graph, sehingga data dapat diorganisasikan dan dikelola secara terstruktur.

Dalam proses penggunaannya, pengguna dapat memilih satu atau lebih kriteria yang tersedia, seperti Murah, Dekat Kampus, dan WiFi. Setelah kriteria dipilih, sistem akan menjalankan algoritma Breadth First Search (BFS) untuk menelusuri node-node yang terhubung pada graph. Hasil penelusuran tersebut digunakan untuk menemukan dan menampilkan alternatif kost yang sesuai dengan kebutuhan serta preferensi pengguna.

Selain menghasilkan rekomendasi kost, sistem juga menampilkan visualisasi Directed Graph menggunakan library NetworkX dan Matplotlib. Visualisasi ini membantu pengguna memahami hubungan antara node kriteria dan alternatif kost yang tersedia. Dengan menggabungkan konsep DSS, struktur data graph, dan algoritma BFS, sistem mampu memberikan rekomendasi kost secara lebih cepat, efektif, dan mudah dipahami oleh pengguna.

### 4.2 Penjelasan Kode

Program DSS Pemilihan Kost dibangun menggunakan bahasa pemrograman Python dengan memanfaatkan beberapa library, yaitu Streamlit untuk membuat antarmuka pengguna, NetworkX untuk membangun dan mengelola graph, Matplotlib untuk menampilkan visualisasi graph, serta collections.deque untuk mendukung implementasi algoritma Breadth First Search (BFS). Pada tahap awal program, dibuat struktur Directed Graph yang berisi hubungan antara node pengguna, kriteria pemilihan kost, dan alternatif kost yang tersedia.

Selanjutnya, program mengimplementasikan algoritma Breadth First Search (BFS) melalui sebuah fungsi yang bertugas menelusuri graph dari node awal yang dipilih pengguna. Algoritma BFS bekerja menggunakan struktur data queue (antrian) untuk mengunjungi node secara bertahap berdasarkan tingkat kedekatannya. Selama proses pencarian, sistem menyimpan node yang telah dikunjungi agar tidak terjadi pengulangan penelusuran. Hasil dari proses BFS berupa daftar alternatif kost yang memenuhi kriteria serta jalur penelusuran yang dilakukan oleh algoritma.

Pada bagian antarmuka, pengguna dapat memilih kriteria kost yang diinginkan melalui fitur yang disediakan oleh Streamlit. Setelah pengguna menjalankan proses pencarian, sistem akan menampilkan rekomendasi kost berdasarkan hasil BFS, jalur penelusuran algoritma, serta visualisasi Directed Graph yang menggambarkan hubungan antar node. Dengan demikian, pengguna tidak hanya memperoleh rekomendasi kost, tetapi juga dapat memahami proses pencarian yang dilakukan oleh sistem secara lebih jelas dan interaktif.

4.3 Tampilan Sistem



