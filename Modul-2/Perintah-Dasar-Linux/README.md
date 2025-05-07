# Langkah – langkah cek hard di windows

1.	klik windows + E

![image](https://github.com/user-attachments/assets/00133ce8-6174-47e8-a24a-4a0f82980e03)
 
2.	Kemudian klik kanan pada “This pc” 

![image](https://github.com/user-attachments/assets/bf4be296-e87e-4c84-9177-a8cbe80ebaf1)
 
3.	Lalu pilih “properties”

![image](https://github.com/user-attachments/assets/cf6fbc0a-23eb-4bbc-b671-cd7a97e7e06e)
 
4.	Pada bagian ini akan menampilkan halaman "About" (Tentang) dari System Settings di Windows 1:
    •	Komputer ini adalah Asus Vivobook e1404fa
    •	Menggunakan Windows 11 Home Single Language 
    •	Memiliki prosesor AMD Ryzen 5 7520U with radeon graphics
    •	Sistem berjalan dalam arsitektur 64-bit. 
    •	Tidak mendukung layar sentuh atau stylus.
    •	Instalasi Windows dilakukan pada 20 Oktober 2024.

![image](https://github.com/user-attachments/assets/932240ef-c83c-41af-a681-12584f4d815b)
 
# Langkah – langkah melihat memory,core dan theard  pada windows

1.	klik ctrl + shift + esc

![image](https://github.com/user-attachments/assets/31dcf419-662a-46f9-9027-33b88d7569a0)

2.	Klik garis tiga di kiri atas 

![image](https://github.com/user-attachments/assets/15fdb468-bbfb-4738-af18-9e554f545a3a)

3.	Lalu pilih “performance”

![image](https://github.com/user-attachments/assets/036b1c22-9568-4f89-ae43-66ff0a469e3c)

4.	Kemudian pilih “memory”. Pada bagian ini kita akan melihat 
    •	Penggunaan RAM cukup tinggi (51%), yang mungkin menunjukkan bahwa banyak aplikasi sedang berjalan. 
    •	Tersisa 7.5 GB RAM yang belum digunakan, jadi masih ada ruang untuk menjalankan aplikasi tambahan. 
    •	Kecepatan RAM adalah 5500 MHz, yang tergolong standar untuk sistem modern. 
    •	memori yang dikompresi (419 MB), menunjukkan bahwa sistem masih memiliki cukup memori yang tersedia.

![image](https://github.com/user-attachments/assets/d68fa056-5420-49f9-8825-ac3a84e7b5bb)
                       
5.	Lalu pilih  “CPU”.pada bagian kanan dapat melihat :
    •	Penggunaan CPU sangat rendah (13%), menunjukkan bahwa komputer tidak sedang bekerja keras. 
    •	Kecepatan CPU naik ke 2.39 GHz, menunjukkan bahwa turbo boost aktif. 
    •	Memiliki 4 core dan 8 thread, cukup kuat untuk multitasking. 
    •	Virtualisasi diaktifkan, memungkinkan penggunaan mesin virtual.
    •	Komputer telah menyala selama 76 jam 28 menit 21 detik.

![image](https://github.com/user-attachments/assets/8e0f4e16-12aa-41a4-b966-4637c27cdabe)

1.	perintah free -h yang digunakan di terminal Linux. Perintah ini digunakan untuk melihat informasi penggunaan memori (RAM) dan swap dalam sistem.
    •  Total: Jumlah total RAM yang tersedia di sistem adalah 3.8 GiB.
    •  Used: RAM yang sedang digunakan adalah 1.0 GiB.
    •  Free: RAM yang tidak digunakan atau kosong adalah 1.7 GiB.
    •  Shared: Memori yang dibagi antar proses adalah 32 MiB.
    •  Buff/Cache: Sebesar 1.4 GiB digunakan untuk menyimpan data buffer dan cache.
    •  Available: RAM yang dapat digunakan untuk proses baru tanpa perlu swap adalah 2.8 GiB.

![image](https://github.com/user-attachments/assets/cdaf33d1-415a-4151-963e-52261119f26d)

2.	tampilan htop, yaitu alat pemantauan sistem yang berjalan di terminal Linux.
    •  CPU Usage: Persentase penggunaan CPU saat ini adalah 55.3%.
    •  Memory Usage: Total memori yang digunakan adalah 840 MB dari 3.82 GB.
    •  Swap: Tidak ada swap yang digunakan (0 KB dari total 0 KB).
    •  Tasks: Total 108 tugas berjalan, dengan 341 thread, 79 kernel thread, dan 2 proses aktif/running.
    •  Load Average: Rata-rata beban sistem adalah 0.43, 0.40, dan 0.53 untuk interval waktu tertentu.
    •  Uptime: Sistem telah berjalan selama 28 menit 59 detik.

![image](https://github.com/user-attachments/assets/35f237b9-6b57-4fc4-8a21-43732d2e0686)

3.	Perintah ini digunakan untuk menampilkan informasi detail tentang penggunaan memori di sistem Linux.
    •  MemTotal: Total kapasitas RAM yang tersedia di sistem, yaitu 4.09 juta KB (~4 GB).
    •  MemFree: Jumlah RAM yang sepenuhnya tidak digunakan, yaitu sekitar 799 ribu KB (~799 MB).
    •  MemAvailable: RAM yang tersedia untuk proses baru tanpa memerlukan swap, yaitu sekitar 2.9 juta KB (~2.9 GB).
    •  Buffers: Memori yang digunakan untuk buffering data saat transfer antar perangkat, sebesar 35 ribu KB (~35 MB).
    •  Cached: Memori yang digunakan untuk menyimpan file yang sering diakses, sebesar 2.2 juta KB (~2.2 GB).
    •  SwapTotal dan SwapFree: Swap tidak tersedia pada sistem ini, terlihat dari nilai 0 KB untuk keduanya.

![image](https://github.com/user-attachments/assets/49faddd4-6738-40e3-8a37-c142375186ba)

4.	Perintah ini digunakan untuk menampilkan informasi detail tentang prosesor (CPU) di sistem Linux.
    •  processor: Menunjukkan ID prosesor, dalam hal ini prosesor 0.
    •  vendor_id: CPU berasal dari vendor AuthenticAMD.
    •  cpu family: Menyebutkan keluarga prosesor, yaitu 23.
    •  model name: Nama model prosesor adalah AMD Ryzen 5 7520U with Radeon Graphics, yang memberikan gambaran tentang jenis prosesor dan kemampuan grafisnya.
    •  cpu MHz: Kecepatan prosesor adalah sekitar 2794.546 MHz (2.79 GHz), yang menunjukkan kemampuan prosesor dalam eksekusi instruksi.
    •  cache size: Kapasitas cache prosesor adalah 512 KB, yang memengaruhi kecepatan pengambilan data yang sering digunakan.
    •  cpu cores: Jumlah inti yang dimiliki oleh CPU adalah 2 inti.

![image](https://github.com/user-attachments/assets/e1e51c06-9e81-463b-a639-6f21e567822a)

5.	Perintah ini digunakan untuk menampilkan informasi detail tentang CPU di sistem Linux.
    •  Architecture: Sistem menggunakan arsitektur x86_64, yang berarti mendukung instruksi 64-bit.
    •  CPU op-mode(s): Mendukung mode operasi 32-bit dan 64-bit.
    •  CPU(s): Memiliki 2 CPU atau inti yang terdeteksi.
    •  Model name: Nama model CPU adalah AMD Ryzen 5 7520U with Radeon Graphics.
    •  Core(s) per socket: CPU memiliki 2 core per socket.
    •  Thread(s) per core: Setiap core hanya memiliki 1 thread.

![image](https://github.com/user-attachments/assets/25c466e1-03d7-4410-97d9-748d891c33b2)
 
6.	perintah ini digunakan untuk menampilkan informasi tentang swap yang sedang digunakan oleh sistem.
    •  Filename: Menampilkan nama file swap yang digunakan, yaitu /swapfile.
    •  Type: Jenis swap yang digunakan adalah file, bukan partisi swap.
    •  Size: Ukuran total swap adalah 1048572 KB atau sekitar 1 GB.
    •  Used: Swap yang sedang digunakan saat ini adalah 0 KB, menunjukkan bahwa swap belum dipakai oleh sistem.
    •  Priority: Prioritas swap adalah -2, yang merupakan nilai default untuk swap file.

![image](https://github.com/user-attachments/assets/5246b51d-1cb5-4981-8356-7d45694e6a51)

7.	Perintah ini digunakan untuk menampilkan statistik sistem dalam format yang lebih mudah dibaca.
    •  Total memory: Total memori sistem adalah 4009636 KB (~4 GB).
    •  Used memory: Memori yang sedang digunakan adalah 1142000 KB (~1.14 GB).
    •  Active memory: Memori aktif (yang digunakan oleh aplikasi dan sering diakses) adalah 1485592 KB (~1.48 GB).
    •  Inactive memory: Memori yang dialokasikan tetapi tidak aktif saat ini adalah 1342992 KB (~1.34 GB).
    •  Free memory: Memori yang sepenuhnya tidak digunakan adalah 755072 KB (~755 MB).
    •  Buffer memory: Memori yang digunakan untuk buffering adalah 36052 KB (~36 MB).
    •  Swap cache: Cache swap yang berisi data yang sebelumnya di-swap adalah 2391820 KB (~2.39 GB).

![image](https://github.com/user-attachments/assets/ecb5785b-97f0-4cde-9847-09ab1266e795)

8.	perintah ini digunakan untuk menampilkan daftar proses yang sedang berjalan di sistem dan mengurutkannya berdasarkan penggunaan memori (%MEM) dari yang terkecil ke terbesar.
    •	 Daftar ini hanya menampilkan proses dengan penggunaan memori paling rendah. 
    •	 Semua proses adalah proses sistem (kernel threads dan worker threads) yang berjalan di latar belakang. 
    •	 Sistem saat ini memiliki beban yang sangat ringan, dengan tidak ada proses yang mengonsumsi banyak memori atau CPU.

![image](https://github.com/user-attachments/assets/73f0159d-f631-412b-a71e-9c0da84c94ae)

9.	menunjukkan sesi terminal di sistem operasi Ubuntu dengan berbagai perintah yang digunakan untuk membuat folder, menulis dan menjalankan skrip Python serta shell, serta mengelola izin eksekusi file
    1.	Pengguna membuat direktori dan file Python, kemudian menjalankannya tanpa masalah.
    2.	Pengguna mencoba menjalankan skrip shell tetapi awalnya gagal karena izin eksekusi tidak diberikan.
    3.	Dengan perintah chmod +x, pengguna memberikan izin eksekusi untuk nuri.sh dan berhasil menjalankannya.
    4.	Baik file Python (tes.py) maupun skrip shell (nuri.sh) menghasilkan output yang sama, yaitu "halo semua".
       Perintah yang penting dalam sesi ini:
       •	mkdir → Membuat direktori.
       •	nano → Mengedit file.
       •	python3 → Menjalankan skrip Python.
       •	chmod +x → Memberikan izin eksekusi pada skrip shell.
       •	./nama_file.sh → Menjalankan skrip shell.

![image](https://github.com/user-attachments/assets/c2b306a6-71ad-4ba4-bfca-26607347f5c3)

# Langkah – langkah  restart pada ubuntu menggunakan terminal

1.	Buka terminal menggunaka ctrl + alt + t
 
![image](https://github.com/user-attachments/assets/fdf5c66b-788e-4494-b7c7-20bb2ccfb028)

2.	kemudian jalankan perintah pada terminal, lalu ketik “sudo reboot” setelah itu klik enter
 
![image](https://github.com/user-attachments/assets/11730148-4e67-4d8c-853f-6fa9c8e2270a)

3.	setelah itu masukan password akun ubuntu kalian lalu klik enter
 
![image](https://github.com/user-attachments/assets/43a6c6a4-9b7f-4ba9-9654-98aef4cf924d)

4.	kemudian tunggu ubuntunya restart 
 
![image](https://github.com/user-attachments/assets/1b24db6a-779f-427d-829d-1a1140bd8524)

# Langkah – langkah  shutdown pada ubuntu menggunakan terminal

1.	Buka terminal menggunakan ctrl + alt + t
 
![image](https://github.com/user-attachments/assets/34c1b357-138b-4694-abdb-01d21388af79)

2.	kemudian jalankan perintah pada terminal, lalu ketik “sudo shutdown now” setelah itu klik enter
 
![image](https://github.com/user-attachments/assets/89edcac9-5293-49e8-99d1-d2185a85ce4b)

3.	setelah itu masukan password akun ubuntu kaian lalu klik enter
 
![image](https://github.com/user-attachments/assets/d9e1b2b5-5ba3-4c53-b011-9cbb814ea58b)

4.	kemudian tunggu ubuntunya  loading
 
![image](https://github.com/user-attachments/assets/10797b61-940a-40c8-a201-defc08034328)

5.	lalu  akan otomatis menunjukkan tampilan Oracle VM VirtualBox Manager dengan sebuah mesin virtual bernama Ubuntu yang dalam keadaan Powered Off
 
![image](https://github.com/user-attachments/assets/4d40f6a5-c6f6-41c9-95f6-14b1c128b768)

# Langkah – langkah  restart pada waktu yang tertentu di ubuntu menggunakan terminal

1.	Buka terminal menggunaka ctrl + alt + t
 
![image](https://github.com/user-attachments/assets/666b7d21-d788-4f6d-9e34-171b66f10438)

2.	 kemudian jalankan perintah pada terminal, lalu ketik “sudo shutdwon -r 07: 07” setelah itu klik enter

![image](https://github.com/user-attachments/assets/d745b6d6-8301-425a-a77d-237cafb819bb)
 
3.	Setelah itu tunggu ubuntunya sampai ada tulisan “Reboot scheduled for tue 2025-03-11 07:07:00 utc,use ‘shutdown -c’ to cancel.
 
![image](https://github.com/user-attachments/assets/2f8acf59-84f3-4a66-bdbe-3ace5878a8df)

4.	kemudian tunggu ubuntunya hingga restart pada waktu yang udah kalian tentukan 
 
![image](https://github.com/user-attachments/assets/c8f752fc-6c81-417f-8ee1-5ec741224a51)

5.	lalu klik nama  
 
![image](https://github.com/user-attachments/assets/633313df-e118-434d-86dd-9ba692fbea6a)

6.	kemudian masukan password yang udah kalian buat
 
![image](https://github.com/user-attachments/assets/1c8125e2-045a-4a70-ae15-90cd2755e5fd)

7.	ubuntu yang udah kalian restart akan otomatis kembali desktop ubuntu
 
![image](https://github.com/user-attachments/assets/a862cee7-47aa-4051-942e-9fecf783b194)

# Langkah – langkah  shutdown pada waktu yang tertentu di ubuntu menggunakan terminal

1.	Buka terminal menggunaka ctrl + alt + t
 
![image](https://github.com/user-attachments/assets/78a4e5f5-ddd0-4a95-9fc3-c719b88d0e91)

2.	kemudian jalankan perintah pada terminal, lalu ketik “sudo shutdwon -h 04: 10” setelah itu klik enter dan masukkan paswordnya lalu klik enter

![image](https://github.com/user-attachments/assets/e160b382-b841-4fde-8306-e5051869dfa7)

3.	Setelah itu tunggu ubuntunya sampai ada tulisan “Reboot scheduled for tue 2025-03-22 04:10:00 utc,use ‘shutdown -c’ to cancel.
 
![image](https://github.com/user-attachments/assets/c44982c5-d016-44a7-ad68-cab7c4e518e4)

4.	kemudian tunggu ubuntunya  loading
 
![image](https://github.com/user-attachments/assets/957ba823-a24b-4a9b-8e71-211eaa3d8817)

5.	lalu  akan otomatis menunjukkan tampilan Oracle VM VirtualBox Manager dengan sebuah mesin virtual bernama Ubuntu yang dalam keadaan Powered Off

![image](https://github.com/user-attachments/assets/237b9c04-bbf2-4c5c-9a1e-b5b00ff03154)
