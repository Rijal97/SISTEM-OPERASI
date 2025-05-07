# Langkah – langkah cek hard di windows

1.	klik windows + E
 
2.	Kemudian klik kanan pada “This pc” 
 
3.	Lalu pilih “properties”
 
4.	Pada bagian ini akan menampilkan halaman "About" (Tentang) dari System Settings di Windows 1:
    •	Komputer ini adalah Asus Vivobook e1404fa
    •	Menggunakan Windows 11 Home Single Language 
    •	Memiliki prosesor AMD Ryzen 5 7520U with radeon graphics
    •	Sistem berjalan dalam arsitektur 64-bit. 
    •	Tidak mendukung layar sentuh atau stylus.
    •	Instalasi Windows dilakukan pada 20 Oktober 2024.
 
# Langkah – langkah melihat memory,core dan theard  pada windows

1.	klik ctrl + shift + esc

2.	Klik garis tiga di kiri atas 

3.	Lalu pilih “performance”

4.	Kemudian pilih “memory”. Pada bagian ini kita akan melihat 
    •	Penggunaan RAM cukup tinggi (51%), yang mungkin menunjukkan bahwa banyak aplikasi sedang berjalan. 
    •	Tersisa 7.5 GB RAM yang belum digunakan, jadi masih ada ruang untuk menjalankan aplikasi tambahan. 
    •	Kecepatan RAM adalah 5500 MHz, yang tergolong standar untuk sistem modern. 
    •	memori yang dikompresi (419 MB), menunjukkan bahwa sistem masih memiliki cukup memori yang tersedia.
                       
5.	Lalu pilih  “CPU”.pada bagian kanan dapat melihat :
    •	Penggunaan CPU sangat rendah (13%), menunjukkan bahwa komputer tidak sedang bekerja keras. 
    •	Kecepatan CPU naik ke 2.39 GHz, menunjukkan bahwa turbo boost aktif. 
    •	Memiliki 4 core dan 8 thread, cukup kuat untuk multitasking. 
    •	Virtualisasi diaktifkan, memungkinkan penggunaan mesin virtual.
    •	Komputer telah menyala selama 76 jam 28 menit 21 detik.

1.	perintah free -h yang digunakan di terminal Linux. Perintah ini digunakan untuk melihat informasi penggunaan memori (RAM) dan swap dalam sistem.
    •  Total: Jumlah total RAM yang tersedia di sistem adalah 3.8 GiB.
    •  Used: RAM yang sedang digunakan adalah 1.0 GiB.
    •  Free: RAM yang tidak digunakan atau kosong adalah 1.7 GiB.
    •  Shared: Memori yang dibagi antar proses adalah 32 MiB.
    •  Buff/Cache: Sebesar 1.4 GiB digunakan untuk menyimpan data buffer dan cache.
    •  Available: RAM yang dapat digunakan untuk proses baru tanpa perlu swap adalah 2.8 GiB.

2.	tampilan htop, yaitu alat pemantauan sistem yang berjalan di terminal Linux.
    •  CPU Usage: Persentase penggunaan CPU saat ini adalah 55.3%.
    •  Memory Usage: Total memori yang digunakan adalah 840 MB dari 3.82 GB.
    •  Swap: Tidak ada swap yang digunakan (0 KB dari total 0 KB).
    •  Tasks: Total 108 tugas berjalan, dengan 341 thread, 79 kernel thread, dan 2 proses aktif/running.
    •  Load Average: Rata-rata beban sistem adalah 0.43, 0.40, dan 0.53 untuk interval waktu tertentu.
    •  Uptime: Sistem telah berjalan selama 28 menit 59 detik.

3.	Perintah ini digunakan untuk menampilkan informasi detail tentang penggunaan memori di sistem Linux.
    •  MemTotal: Total kapasitas RAM yang tersedia di sistem, yaitu 4.09 juta KB (~4 GB).
    •  MemFree: Jumlah RAM yang sepenuhnya tidak digunakan, yaitu sekitar 799 ribu KB (~799 MB).
    •  MemAvailable: RAM yang tersedia untuk proses baru tanpa memerlukan swap, yaitu sekitar 2.9 juta KB (~2.9 GB).
    •  Buffers: Memori yang digunakan untuk buffering data saat transfer antar perangkat, sebesar 35 ribu KB (~35 MB).
    •  Cached: Memori yang digunakan untuk menyimpan file yang sering diakses, sebesar 2.2 juta KB (~2.2 GB).
    •  SwapTotal dan SwapFree: Swap tidak tersedia pada sistem ini, terlihat dari nilai 0 KB untuk keduanya.

4.	Perintah ini digunakan untuk menampilkan informasi detail tentang prosesor (CPU) di sistem Linux.
    •  processor: Menunjukkan ID prosesor, dalam hal ini prosesor 0.
    •  vendor_id: CPU berasal dari vendor AuthenticAMD.
    •  cpu family: Menyebutkan keluarga prosesor, yaitu 23.
    •  model name: Nama model prosesor adalah AMD Ryzen 5 7520U with Radeon Graphics, yang memberikan gambaran tentang jenis prosesor dan kemampuan grafisnya.
    •  cpu MHz: Kecepatan prosesor adalah sekitar 2794.546 MHz (2.79 GHz), yang menunjukkan kemampuan prosesor dalam eksekusi instruksi.
    •  cache size: Kapasitas cache prosesor adalah 512 KB, yang memengaruhi kecepatan pengambilan data yang sering digunakan.
    •  cpu cores: Jumlah inti yang dimiliki oleh CPU adalah 2 inti.

5.	Perintah ini digunakan untuk menampilkan informasi detail tentang CPU di sistem Linux.
    •  Architecture: Sistem menggunakan arsitektur x86_64, yang berarti mendukung instruksi 64-bit.
    •  CPU op-mode(s): Mendukung mode operasi 32-bit dan 64-bit.
    •  CPU(s): Memiliki 2 CPU atau inti yang terdeteksi.
    •  Model name: Nama model CPU adalah AMD Ryzen 5 7520U with Radeon Graphics.
    •  Core(s) per socket: CPU memiliki 2 core per socket.
    •  Thread(s) per core: Setiap core hanya memiliki 1 thread.
 
6.	perintah ini digunakan untuk menampilkan informasi tentang swap yang sedang digunakan oleh sistem.
    •  Filename: Menampilkan nama file swap yang digunakan, yaitu /swapfile.
    •  Type: Jenis swap yang digunakan adalah file, bukan partisi swap.
    •  Size: Ukuran total swap adalah 1048572 KB atau sekitar 1 GB.
    •  Used: Swap yang sedang digunakan saat ini adalah 0 KB, menunjukkan bahwa swap belum dipakai oleh sistem.
    •  Priority: Prioritas swap adalah -2, yang merupakan nilai default untuk swap file.

7.	Perintah ini digunakan untuk menampilkan statistik sistem dalam format yang lebih mudah dibaca.
    •  Total memory: Total memori sistem adalah 4009636 KB (~4 GB).
    •  Used memory: Memori yang sedang digunakan adalah 1142000 KB (~1.14 GB).
    •  Active memory: Memori aktif (yang digunakan oleh aplikasi dan sering diakses) adalah 1485592 KB (~1.48 GB).
    •  Inactive memory: Memori yang dialokasikan tetapi tidak aktif saat ini adalah 1342992 KB (~1.34 GB).
    •  Free memory: Memori yang sepenuhnya tidak digunakan adalah 755072 KB (~755 MB).
    •  Buffer memory: Memori yang digunakan untuk buffering adalah 36052 KB (~36 MB).
    •  Swap cache: Cache swap yang berisi data yang sebelumnya di-swap adalah 2391820 KB (~2.39 GB).

8.	perintah ini digunakan untuk menampilkan daftar proses yang sedang berjalan di sistem dan mengurutkannya berdasarkan penggunaan memori (%MEM) dari yang terkecil ke terbesar.
    •	 Daftar ini hanya menampilkan proses dengan penggunaan memori paling rendah. 
    •	 Semua proses adalah proses sistem (kernel threads dan worker threads) yang berjalan di latar belakang. 
    •	 Sistem saat ini memiliki beban yang sangat ringan, dengan tidak ada proses yang mengonsumsi banyak memori atau CPU.

9.	menunjukkan sesi terminal di sistem operasi Ubuntu dengan berbagai perintah yang digunakan untuk membuat folder, menulis dan menjalankan skrip Python serta shell, serta mengelola izin eksekusi file
    
1.	Pengguna membuat direktori dan file Python, kemudian menjalankannya tanpa masalah.
   
3.	Pengguna mencoba menjalankan skrip shell tetapi awalnya gagal karena izin eksekusi tidak diberikan.
   
5.	Dengan perintah chmod +x, pengguna memberikan izin eksekusi untuk nuri.sh dan berhasil menjalankannya.
   
7.	Baik file Python (tes.py) maupun skrip shell (nuri.sh) menghasilkan output yang sama, yaitu "halo semua".
    Perintah yang penting dalam sesi ini:
    •	 mkdir → Membuat direktori.
    •	 nano → Mengedit file.
    •	 python3 → Menjalankan skrip Python.
    •	 chmod +x → Memberikan izin eksekusi pada skrip shell.
    •	 ./nama_file.sh → Menjalankan skrip shell.

# Langkah – langkah restart pada ubuntu menggunakan terminal

1.	Buka terminal menggunaka ctrl + alt + t
 
2.	kemudia jalankan perintah pada terminal, lalu ketik “sudo reboot” setelah itu klik enter
 
3.	setelah itu masukan password akun ubuntu kaian lalu klik enter

4.	kemudian tunggu ubuntunya restart 

# Langkah – langkah  shutdown pada ubuntu menggunakan terminal

1.	Buka terminal menggunakan ctrl + alt + t
 
2.	kemudian jalankan perintah pada terminal, lalu ketik “sudo shutdown now” setelah itu klik enter
 
3.	setelah itu masukan password akun ubuntu kaian lalu klik enter
 
4.	kemudian tunggu ubuntunya  loading
 
5.	lalu  akan otomatis menunjukkan tampilan Oracle VM VirtualBox Manager dengan sebuah mesin virtual bernama Ubuntu yang dalam keadaan Powered Off
 
# Langkah – langkah  restart pada waktu yang tertentu di ubuntu menggunakan terminal

1.	Buka terminal menggunaka ctrl + alt + t

2.	kemudian jalankan perintah pada terminal, lalu ketik “sudo shutdwon -r 07: 07” setelah itu klik enter
 
3.	Setelah itu tunggu ubuntunya sampai ada tulisan “Reboot scheduled for tue 2025-03-11 07:07:00 utc,use ‘shutdown -c’ to cancel.
 
4.	kemudian tunggu ubuntunya hingga restart pada waktu yang udah kalian tentukan 

5.	lalu klik nama  
 
6.	kemudian masukan password yang udah kalian buat
 
7.	ubuntu yang udah kalian restart akan otomatis kembali desktop ubuntu
 
8.	Setelah itu tunggu ubuntunya sampai ada tulisan “Reboot scheduled for tue 2025-03-11 07:07:00 utc,use ‘shutdown -c’ to cancel.
 
# Langkah – langkah  shutdown pada waktu yang tertentu di ubuntu menggunakan terminal

1.	Buka terminal menggunaka ctrl + alt + t
 
2.	kemudian jalankan perintah pada terminal, lalu ketik “sudo shutdwon -h 04: 10” setelah itu klik enter dan masukkan paswordnya lalu klik enter

3.	Setelah itu tunggu ubuntunya sampai ada tulisan “Reboot scheduled for tue 2025-03-22 04:10:00 utc,use ‘shutdown -c’ to cancel.
 
4.	kemudian tunggu ubuntunya  loading
 
5.	lalu  akan otomatis menunjukkan tampilan Oracle VM VirtualBox Manager dengan sebuah mesin virtual bernama Ubuntu yang dalam keadaan Powered Off









![Cuplikan layar 2025-05-01 140744](https://github.com/user-attachments/assets/e49088d1-0009-49ff-8141-92a5234f399c)

























