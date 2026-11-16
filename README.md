# proxmox-virtualization
Materi pembelajaran Proxmox VE yang mencakup virtualisasi, pembuatan Virtual Machine (VM), instalasi sistem operasi, dan pengelolaan server.
1. Pengertian Proxmox VE
Proxmox Virtual Environment (Proxmox VE) adalah platform virtualisasi berbasis Linux yang digunakan untuk membuat, menjalankan, dan mengelola mesin virtual (Virtual Machine) serta container. Proxmox memiliki antarmuka berbasis web yang memudahkan administrator dalam mengelola server secara terpusat.
Proxmox bersifat open source sehingga dapat digunakan dan dikembangkan sesuai kebutuhan pengguna.

2. Sejarah Proxmox
Proxmox dikembangkan oleh Proxmox Server Solutions GmbH yang berasal dari Austria. Proxmox Virtual Environment pertama kali dirilis pada tahun 2008.
Sejak pertama kali diperkenalkan, Proxmox terus mengalami perkembangan dengan penambahan fitur virtualisasi, pengelolaan penyimpanan, pencadangan data, dan pengelolaan jaringan.

3. Pengertian Virtualisasi
Virtualisasi adalah teknologi yang memungkinkan satu perangkat komputer fisik menjalankan beberapa lingkungan komputer virtual secara bersamaan.
Setiap lingkungan virtual dapat memiliki sistem operasi, aplikasi, dan sumber daya komputasi sendiri. Teknologi ini membantu penggunaan perangkat keras menjadi lebih efisien.

4. Fungsi dan Manfaat Proxmox
Proxmox memiliki beberapa fungsi dan manfaat, antara lain:

Membuat dan menjalankan Virtual Machine.

Menjalankan beberapa sistem operasi dalam satu server fisik.

Mengelola sumber daya CPU, RAM, dan penyimpanan.

Mengelola jaringan virtual.

Melakukan backup dan restore mesin virtual.

Memudahkan administrasi server melalui antarmuka web.

Mendukung pembelajaran virtualisasi dan administrasi jaringan.

5. Persyaratan Sistem Proxmox

Sebelum melakukan instalasi Proxmox VE, terdapat beberapa persyaratan yang harus diperhatikan:

Komputer atau server yang kompatibel.

Prosesor yang mendukung teknologi virtualisasi.

Kapasitas RAM yang mencukupi.

Media penyimpanan seperti SSD atau HDD.

File ISO Proxmox VE.

USB bootable sebagai media instalasi.

Koneksi jaringan untuk mengakses antarmuka Proxmox.

6. Arsitektur Virtualisasi

Arsitektur virtualisasi merupakan susunan komponen yang memungkinkan beberapa sistem virtual berjalan pada satu perangkat fisik.

Komponen utama dalam arsitektur Proxmox meliputi:

Hardware: Perangkat keras seperti prosesor, RAM, dan media penyimpanan.

Proxmox VE: Platform yang mengelola lingkungan virtualisasi.

Virtual Machine: Komputer virtual yang memiliki sistem operasi sendiri.

Storage: Media untuk menyimpan sistem operasi dan data VM.

Network: Komponen yang mengatur koneksi jaringan mesin virtual.

7. Instalasi Proxmox VE
Instalasi Proxmox VE dilakukan menggunakan file ISO resmi yang dimasukkan ke media USB bootable.

Tahapan umum instalasi Proxmox adalah:

Menyiapkan komputer atau server.

Mengunduh file ISO Proxmox VE dari situs resminya.

Membuat USB bootable.

Melakukan booting melalui media instalasi.

Memilih menu instalasi Proxmox VE.

Menentukan media penyimpanan.

Mengatur lokasi, zona waktu, dan keyboard.

Membuat kata sandi administrator.

Mengatur konfigurasi jaringan.

Menyelesaikan instalasi dan melakukan restart.

8. Pengenalan Dashboard Proxmox
Dashboard Proxmox merupakan tampilan antarmuka berbasis web yang digunakan untuk mengelola server virtualisasi.

Beberapa bagian utama dashboard Proxmox adalah:

Datacenter: Mengelola seluruh lingkungan Proxmox.

Node: Menampilkan server fisik yang menjalankan Proxmox.

Virtual Machine: Menampilkan daftar mesin virtual.

Storage: Mengelola media penyimpanan.

Network: Mengatur konfigurasi jaringan.

Summary: Menampilkan informasi penggunaan sumber daya server.

9. Pengertian Virtual Machine (VM)
Virtual Machine (VM) adalah komputer virtual yang dibuat menggunakan teknologi virtualisasi. VM dapat menjalankan sistem operasi dan aplikasi secara terpisah dari sistem operasi utama.

Setiap VM memiliki sumber daya virtual seperti CPU, RAM, penyimpanan, dan perangkat jaringan.

Contoh sistem operasi yang dapat dijalankan pada VM adalah:

Debian

Ubuntu

Windows

Linux Mint

10. Pembuatan Virtual Machine
Pembuatan Virtual Machine dilakukan melalui dashboard Proxmox dengan langkah-langkah berikut:

Masuk ke dashboard Proxmox melalui browser.

Pilih node yang akan digunakan.

Klik menu Create VM.

Masukkan VM ID dan nama mesin virtual.

Pilih file ISO sistem operasi.

Tentukan jenis sistem operasi.

Atur kapasitas penyimpanan.

Tentukan jumlah CPU.

Atur kapasitas RAM.

Konfigurasikan jaringan virtual.

Periksa kembali pengaturan.

Klik Finish untuk menyelesaikan pembuatan VM.

11. Instalasi Sistem Operasi pada VM
Setelah Virtual Machine berhasil dibuat, langkah selanjutnya adalah melakukan instalasi sistem operasi.

Tahapan instalasi sistem operasi pada VM meliputi:

Pilih VM yang telah dibuat.

Jalankan mesin virtual dengan menekan tombol Start.

Buka menu Console.

Ikuti petunjuk instalasi sistem operasi.

Atur bahasa dan lokasi.

Tentukan partisi penyimpanan.

Buat akun pengguna.

Selesaikan proses instalasi.

Lakukan restart pada VM.

Pastikan sistem operasi berhasil dijalankan.

12. Pengelolaan Virtual Machine
Proxmox menyediakan berbagai fitur untuk mengelola mesin virtual, di antaranya:

Start: Menjalankan mesin virtual.

Shutdown: Mematikan mesin virtual secara normal.

Reboot: Memulai ulang mesin virtual.

Console: Mengakses tampilan mesin virtual.

Snapshot: Menyimpan kondisi VM pada waktu tertentu.

Backup: Membuat salinan data mesin virtual.

Restore: Mengembalikan VM dari file backup.

Clone: Membuat salinan dari mesin virtual yang sudah ada.

Fitur-fitur tersebut membantu administrator mengelola mesin virtual dengan lebih mudah dan teratur.

13. Perbedaan Virtual Machine dan Container
Virtual Machine dan Container merupakan teknologi yang digunakan untuk menjalankan lingkungan komputasi secara terisolasi. Namun, keduanya memiliki cara kerja yang berbeda.

A. Virtual Machine (VM)

Memiliki sistem operasi sendiri.

Menggunakan sumber daya virtual seperti CPU, RAM, dan penyimpanan.

Dapat menjalankan sistem operasi yang berbeda dari host.

Menggunakan hypervisor untuk menjalankan mesin virtual.

B. Container

Berbagi kernel sistem operasi host.

Memiliki lingkungan aplikasi yang terisolasi.

Umumnya menggunakan sumber daya lebih sedikit dibandingkan VM.

Cocok untuk menjalankan aplikasi dalam lingkungan terpisah.

14. Kesimpulan
Proxmox Virtual Environment merupakan platform virtualisasi yang digunakan untuk membuat, menjalankan, dan mengelola mesin virtual serta container. Dengan mempelajari Proxmox, siswa dapat memahami konsep virtualisasi, instalasi sistem operasi, pembuatan Virtual Machine, pengelolaan sumber daya, dan administrasi server.

Pembelajaran Proxmox memberikan dasar pengetahuan dan keterampilan dalam bidang teknologi informasi, khususnya administrasi server dan jaringan komputer.
