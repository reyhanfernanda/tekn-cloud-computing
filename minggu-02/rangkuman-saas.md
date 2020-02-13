## What is the difference between IaaS, SaaS, and PaaS?.


# IaaS - Infrastructure-as-a-Service
  * Layanan cloud yang memungkinkan pengguna mendapatkan akses ke infrastruktur mereka sendiri - komputer, sumber daya jaringan, penyimpanan. Perlu dicatat bahwa ini biasanya sumber daya virtual, tetapi bisa jadi sumber daya nyata, fisik.

# PaaS - Platform-as-a-Service
  * Layanan cloud yang mengabstraksi infrastruktur (pengguna tidak bisa melihat komputer, loadbalancers, dll.) Melainkan menyediakan platform pengembangan perangkat lunak. Dimungkinkan untuk membuat kode dan menjalankan aplikasi pada PaaS dan sistem memastikan bahwa aplikasi memiliki infrastruktur yang diperlukan untuk membuatnya berjalan dan skala.

# SaaS - Software-as-a-Service
  * Layanan cloud yang memberikan pengguna akses ke perangkat lunak dengan layanan mandiri, sesuai permintaan. Ini bisa berupa aplikasi tunggal atau memberikan katalog perangkat lunak yang dapat dipilih pengguna.

[link ke Sumber](https://www.quora.com/What-is-the-difference-between-IaaS-SaaS-and-Paas#)

## SaaS Platform Architecture.

SaaS adalah model pengiriman umum untuk banyak aplikasi bisnis, termasuk perangkat lunak perkantoran dan pesan, perangkat lunak manajemen, virtualisasi dll. Ini adalah bagian dari nomenklatur komputasi awan, bersama dengan infrastruktur sebagai layanan (IaaS), platform sebagai layanan (PaaS) , desktop sebagai layanan (DaaS).

# Arsitektur SAAS:

Dengan model ini, satu versi aplikasi, dengan satu konfigurasi digunakan untuk semua pelanggan. Aplikasi ini diinstal pada banyak mesin untuk mendukung skalabilitas (disebut penskalaan horizontal). Dalam beberapa kasus, versi kedua aplikasi diatur untuk menawarkan kelompok pelanggan tertentu dengan akses ke versi pra-rilis aplikasi untuk tujuan pengujian. Dalam model tradisional ini, setiap versi aplikasi didasarkan pada kode unik. Meskipun pengecualian, beberapa solusi SaaS tidak menggunakan multitenancy, untuk mengelola secara efektif sejumlah besar pelanggan di tempat. Apakah multitenancy merupakan komponen yang diperlukan untuk perangkat lunak-sebagai-layanan adalah topik kontroversi.

# Ada dua varietas utama SaaS:

* SaaS Vertikal
  * Perangkat Lunak yang menjawab kebutuhan industri tertentu (mis. Perangkat lunak untuk kesehatan, pertanian, industri keuangan)

* SaaS Horisontal
  * Produk-produk yang berfokus pada kategori perangkat lunak (pemasaran, penjualan, alat pengembang, SDM) tetapi agnostik industri.

# Manfaat SAAS:

Ini menawarkan peluang besar bagi organisasi dari semua ukuran untuk mengalihkan risiko akuisisi perangkat lunak, dan untuk memindahkan TI dari pusat biaya reaktif menjadi bagian perusahaan yang proaktif dan bernilai tambah. Secara tradisional, menyebarkan sistem perangkat lunak skala besar telah menjadi tugas utama. Menyebarkan sistem ini di perusahaan besar membutuhkan biaya lebih besar. Waktu, staf, dan persyaratan anggaran untuk penyebaran sebesar ini mewakili risiko yang signifikan bagi organisasi dalam ukuran berapa pun, dan sering kali menempatkan perangkat lunak seperti itu di luar jangkauan organisasi yang lebih kecil yang jika tidak dapat diturunkan darinya banyak utilitas. Model pengiriman berdasarkan permintaan mengubah beberapa hal ini. Aplikasi SaaS tidak memerlukan penyebaran infrastruktur besar di lokasi klien.

[link ke Sumber] (https://hackernoon.com/saas-software-as-a-service-platform-architecture-757a432270f5)

## Fitur dan Manfaat Utama dari Platform SaaS

# Kesederhanaan

Aplikasi perangkat lunak yang dirancang sebagai solusi SaaS biasanya diakses melalui web melalui berbagai jenis perangkat. Kemajuan dalam bahasa pemrograman sisi klien seperti JavaScript telah menghasilkan antarmuka web yang lebih intuitif dan dengan demikian, membuat penggunaan aplikasi yang dikirim melalui internet mudah digunakan seperti rekan-rekan desktop mereka.

# Ekonomis

Model pembayaran biaya subskrip bulanan atau tahunan memudahkan bisnis untuk menganggarkan dana, ditambah dengan biaya pemasangan infrastruktur nol, mudah untuk melihat bagaimana memilih menggunakan solusi SaaS dapat menghemat uang bisnis.

# Keamanan

Keamanan adalah aspek penting dari solusi pengembangan perangkat lunak dan platform SaaS tidak berbeda. Sebagai konsumen aplikasi yang dirancang menggunakan SaaS, Anda tidak perlu khawatir dengan bagaimana data Anda dikunci. Itu dipegang dengan aman di awan!

# Kesesuaian

Dengan penginstalan perangkat lunak tradisional, pembaruan dan tambalan terkadang membutuhkan banyak waktu dan uang. Ini terutama benar dalam perusahaan. Selain itu, perbedaan versi antara anggota tim dari tenaga kerja Anda dapat menyebabkan masalah kompatibilitas dan bahkan lebih banyak waktu terbuang. Namun, dengan SaaS, pelanggan dapat log-on ke layanan yang sudah ditingkatkan.

[link ke Sumber] (https://www.devteam.space/blog/saas-software-as-a-service-platform-architecture/)

## How to build a cloud-based SaaS Application.
Mengatur MongoDB untuk aplikasi SaaS
Memulai dengan MongoDB kami memasang instance MongoDB tunggal pada instance AWS EC2

* Sistem antrian
Sistem antrian pesan adalah protokol komunikasi yang tidak sinkron , memungkinkan pengirim dan penerima pesan tidak berinteraksi secara bersamaan.

Juga dikenal sebagai teknologi Antrian Pesan (MSMQ) memungkinkan aplikasi web untuk berjalan pada waktu yang berbeda dan untuk berkomunikasi dengan berbagai integrasi pihak ketiga / API / dan layanan lainnya secara tidak sinkron.

* RabbitMQ
RabbitMQ adalah sistem antrian sumber terbuka yang berjalan pada semua sistem operasi utama.

- menginstal RabbitMQ
Menggunakan server RabbitMQ tunggal , dengan beberapa titik akhir yang memberi makan antrian dengan tugas (tugas berkala serta tugas yang disebabkan oleh tindakan pengguna) serta titik akhir yang memproses tugas-tugas tersebut (mis. Buat tangkapan layar kami yang terlihat bagus).

The konfigurasi optimal akan mencakup server RabbitMQ kedua tawaran replikasi dan mekanisme failover (dengan menyembunyikan mereka di belakang penyeimbang beban).

* AWS & EC2

AWS memungkinkan Anda untuk meng-host dan menjalankan aplikasi web Anda serta melakukan pekerjaan batch berkinerja tinggi. Dengan Elastic Compute Cloud (EC2) AWS menyediakan server virtual yang dapat diskalakan untuk setiap bisnis.

* Mengapa EC2
Amazon EC2 adalah keharusan dan inti dari sistem kami yang menyediakan kapasitas komputasi yang dapat diubah ukurannya.Yang hebat di sini adalah, bahwa server-server EC2 tersebar di seluruh dunia. Bergantung pada kebutuhan Anda untuk mengukur dan pasar geografis mana yang menjadi target pertama, Anda dapat memilih di antara berbagai lokasi EC2 Anda.

* Penyimpanan Web S3

Amazon Simple Storage Service (S3) mudah digunakan, menyimpan dan mengambil data dalam jumlah berapa pun. Anda mungkin bertanya-tanya apakah Amazon S3 hanya dapat digunakan dengan layanan AWS lainnya? Jawaban yang bagus adalah: tidak. Ini juga dapat digunakan sendiri atau dengan repositori dan gateway penyimpanan pihak ke-3 lainnya. Dan tentu saja, ini bekerja sangat baik bersama dengan EC2.

Selain menyimpan data aplikasi web Anda dengan S3, ini juga bisa digunakan untuk cadangan, arsip, atau analitik data besar.

* Jaringan Pengiriman Konten
Sebuah jaringan pengiriman konten (CDN) pada dasarnya adalah sebuah sistem server didistribusikan yang memungkinkan Anda untuk melayani konten dengan pengguna aplikasi Anda dengan kinerja tinggi dan ketersediaan tinggi.

* Rekap: mengatur aplikasi SaaS
Dengan Python, MongoDB - sebagai basis data yang berorientasi pada dokumen, perangkat lunak RabbitMQ sebaiknya dilakukan dengan pengaturan dasar. Namun, ada banyak cara untuk dipikirkan. Dalam posting tindak lanjut kami, kami akan membahas kebutuhan perangkat lunak pemantauan dan analitik yang tepat serta bagaimana prosedur pembayaran dapat berjalan dengan lancar di cloud.

[link ke Sumber] (https://usersnap.com/blog/cloud-based-saas-architecture-fundamentals/)
