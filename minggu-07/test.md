# Get Starter - Docker

# Uji versi Docker 
Setelah berhasil menginstal Docker Desktop, buka terminal dan jalankan docker --version untuk memeriksa versi Docker yang diinstal pada mesin
[image](https://github.com/reyhanfernanda/tekn-cloud-computing/blob/master/minggu-07/gambar-06.png)

# Instalasi Docker Test

1. Uji apakah instalasi Anda berfungsi dengan menjalankan image Docker hello-world :
[image](https://github.com/reyhanfernanda/tekn-cloud-computing/blob/master/minggu-07/gambar-07.png)

2. untuk melihat image yang sedang berjalan bisa menggunakan perintah docker image ls
[image](https://github.com/reyhanfernanda/tekn-cloud-computing/blob/master/minggu-07/gambar-08.png)

# Build and run  image

1. kita melakukan clone/pull terhadap repository git yang didalamnya terdapat beberapa image docker dan berpindah ke direktori dengan mengetikkan perintah cd
[image](https://github.com/reyhanfernanda/tekn-cloud-computing/blob/master/minggu-07/gambar-12.png)

2. lalu image bulletinboard yang sudah di clone sebelumnya kita build
[image](https://github.com/reyhanfernanda/tekn-cloud-computing/blob/master/minggu-07/gambar-13.png)
[image](https://github.com/reyhanfernanda/tekn-cloud-computing/blob/master/minggu-07/gambar-14.png)

3. Setelah melakukan build dan Success, selanjutnya dilakukan run images dengan docker run --publish 8000:808 --detcah --name bb bulletinboard:1.0
[image](https://github.com/reyhanfernanda/tekn-cloud-computing/blob/master/minggu-07/gambar-15.png)

4. buka browser kemudian ketikan localhost:8000 maka akan muncul sebuah tampilan dari image dockerbulletin board
[image](https://github.com/reyhanfernanda/tekn-cloud-computing/blob/master/minggu-07/gambar-17.png)

5. Setelah menjalankan image, kemudian untuk menghentikan container sebelum melakukan stop container yang berjalan dilakukan pengecekan terlebih dahulu dengan mengetikkan perintah docker -ps a kemudian akan dimunculkan daftar container yang sedang berjalan
[image](https://github.com/reyhanfernanda/tekn-cloud-computing/blob/master/minggu-07/gambar-16.png)

6. dan untuk Memberhentikan container yang sedang jalan, dan menghapusnya dari list container dapat dilakukan dengan perintah docker rm --force bb
[image](https://github.com/reyhanfernanda/tekn-cloud-computing/blob/master/minggu-07/gambar-18.png)

# Share images on Docker Hub
Jika kita belum memiliki ID Docker, maka melakukan langkah-langkah ini 

1. Kunjungi halaman mendaftar Docker Hub, https://hub.docker.com/signup .
2. Isi formulir dan kirim untuk membuat ID Docker Anda.
[image](https://github.com/reyhanfernanda/tekn-cloud-computing/blob/master/minggu-07/gambar-18.png)
3. Verifikasi alamat email kita untuk menyelesaikan proses pendaftaran.
4. setlah itu login menggunakan ID Docker dan kata sandi kita yang baru. Setelah kita berhasil mengautentikasi, maka docker sudah siap digunakan

# Create a Docker Hub repository and push image

1. Klik ikon Docker di bagian menu , lalau buat repositori baru.

2. Isi nama repositori yaitu bulletinboard. lalu seting visibility repsitory tersebut, bisa public atau private lalu klik create
[image](https://github.com/reyhanfernanda/tekn-cloud-computing/blob/master/minggu-07/gambar-19.png)

3. untuk melakukan push image ke dokerhub kita harus memiliki akun dokerhub dan tempmembuatat repository untuk meletakan image tersebut
[image](https://github.com/reyhanfernanda/tekn-cloud-computing/blob/master/minggu-07/gambar-20.png)

4. lalu memberikan nama image sesuai dengan persyaratan share di dokerhub dan push image kedalam repository dengan perintah push
[image](https://github.com/reyhanfernanda/tekn-cloud-computing/blob/master/minggu-07/gambar-21.png)

5. setelah proses push ke respository dokerhub berhasil maka hasilnya dapat dilihat seperti gambar dibawah ini
[image](https://github.com/reyhanfernanda/tekn-cloud-computing/blob/master/minggu-07/gambar-22.png)
[image](https://github.com/reyhanfernanda/tekn-cloud-computing/blob/master/minggu-07/gambar-23.png)