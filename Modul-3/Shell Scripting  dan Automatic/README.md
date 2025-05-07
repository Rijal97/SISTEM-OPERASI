# Cara menggunakan Variabel di Shell Scripting dan Automasi

1.  Mendeklarasikan dan Menggunakan Variabel
    Variabel  “nama” dan “umur”  disimpan dengan nilai yang bisa dipanggil menggunakan “$nama” atau “$umur”.
    nama=”Rijal” berarti kita membuat variabel bernama nama, lalu mengisinya dengan teks "Rijal".
    Umur=19 artinya kita membuat variabel bernama umur dan mengisinya dengan angka 25.

![image](https://github.com/user-attachments/assets/e139f3ba-f773-4f0c-9029-386900500540)

2.  Mengambil Input dari Pengguna
    “read” digunakan untuk menyimpan input dari pengguna ke dalam variabel.
    echo “masukkan nama anda:” - Skrip menampilkan pesan di layar, meminta pengguna memasukkan nama mereka.
    read nama - Skrip berhenti sejenak, menunggu pengguna mengetik sesuatu. Apapun yang mereka ketik akan disimpan dalam variabel.
    echo “selamat datang $nama.” - Setelah pengguna menekan Enter, skrip akan menggunakan nilai yang mereka masukkan dan menampilkannya kembali.

![image](https://github.com/user-attachments/assets/6ee29395-f3f4-405e-abdd-50c5b1dafbb1)

3.  Operasi Matematika dengan Variabel
    - x=10 → Menyimpan nilai 10 ke dalam variabel x
    - y=5 → Menyimpan nilai 5 ke dalam variabel y
    - hasil=$((x + y)) → Menggunakan (()) untuk melakukan operasi penjumlahan antara x  dan y, lalu menyimpan hasilnya dalam variabel hasil

![image](https://github.com/user-attachments/assets/41d216ad-5ecb-470b-8151-00ba1f71c5f2)

# Cara menggunakan kondisi di shell Scripting dan Automasi

1. Menggunakan If-Else
   Variabel Angka  disimpan dengan nilai 10.
   [$angka -gt 5] → Memeriksa apakah angka lebih besar dari 5 .
   -gt berarti "greater than" atau "lebih besar dari."
   Menjalankan perintah jika kondisi benar (then) Jika  lebih dari 5, maka program akan menampilkan:
   Angka lebih besar dari 5
   Menjalankan perintah jika kondisi salah (else)
   Jika tidak lebih dari 5, maka yang ditampilkan adalah:
   Angka kurang dari atau sama dengan 5
   Menutup blok kondisi dengan fi
   Fi menandai akhir dari blok if.

![image](https://github.com/user-attachments/assets/d1f3fd2a-16ef-48e2-9ebf-188eb0ba938d)

2.  Menggunakan If-Elif-Else
    Deklarasi variabel →  nilai diberi nilai 80. Ini adalah angka yang akan dibandingkan dalam kondisi. 
    Percabangan if  → Memeriksa apakah nilai lebih besar atau sama dengan 90.
    -ge → Operator perbandingan yang berarti "greater than or equal to" (lebih besar atau sama dengan).
    [$nilai -ge 90] → Harus ada spasi antara , (variabel, operator, dan).
    Jika kondisi benar (nilai ≥ 90), maka program akan menampilkan "grade: A".
    Elif (else if) → Jika kondisi pertama salah, program memeriksa kondisi lain: apakah nilai lebih besar atau sama dengan 75.
    Jika nilai ≥ 75 tetapi < 90, program menampilkan "grade: B".
    Kondisi terakhir → Jika tidak memenuhi salah satu kondisi di atas, maka eksekusi masuk ke blok else.
    Jika nilai < 75, program menampilkan "grade: C".
    Menutup blok if → fi menandai bahwa struktur percabangan selesai.

![image](https://github.com/user-attachments/assets/86b7ccfe-f30c-4dfb-97a1-614aa15bd4f7)

# cara menggunakan perulangan di shell scripting

1. Menggunakan  Loop
   Digunakan untuk mengulang sejumlah elemen atau rentang angka.
   Loop for → Mengulang setiap angka dari 1 hingga 5.
   Angka → Nama variabel yang akan berubah setiap iterasi dari 1, 2, 3, 4, hingga 5.
   {1..5} → Menggunakan rentang angka dari 1 sampai 5 untuk iterasi.
   do →  Menandai awal dari blok kode yang akan dieksekusi dalam setiap iterasi.
   Echo “angka saat ini: $angka” →  Menampilkan nilai variabel angka yang berubah setiap iterasi.
   $angka → Digunakan untuk mengambil nilai dari variabel angka saat ini.
   Done →  Menutup blok perulangan dan menandakan akhir dari loop.
   Setelah mencapai angka terakhir (5), perulangan berhenti. 

![image](https://github.com/user-attachments/assets/ff3e8ed8-f6ec-404c-87d8-31ff44b03ec6)

2.  Menggunakan While Loop
    Digunakan untuk mengulang selama kondisi tertentu masih benar.
    angka=1 →  Mendeklarasikan variabel angka dengan nilai awal 1 →  
    Sebagai nilai awal untuk perulangan.
    Nilai ini akan bertambah setiap iterasi hingga mencapai batas.
    While [ $angka -le 5 ] Membuat loop while → Perulangan akan 
    berjalan selama kondisi angka ≤ 5 masih benar.
    -le → Operator perbandingan yang berarti "less than or equal to" (kurang dari atau sama dengan).
    Jika nilai angka lebih besar dari 5, perulangan akan berhenti.
    Do Menandai awal dari blok perulangan → Semua perintah di dalam blok do ... done akan dijalankan setiap iterasi.
    echo “angka saat ini: $angka” Menampilkan nilai angka saat ini → Setiap iterasi akan mencetak teks
    “angka saat ini: X, di mana X adalah nilai variabel angka.
    Output akan berubah sesuai dengan nilai angka.
    angka=$((angka + 1)) Menambah nilai angka setiap iterasi → Agar 
    loop tidak berjalan selamanya (infinite loop), nilai angka harus diperbarui.
    $((angka + 1)) → Perintah ini menjumlahkan angka dengan 1 di setiap iterasi.
    Done Menutup blok while → Menandakan akhir dari perulangan.
    Jika kondisi angka <5 sudah tidak terpenuhi, program keluar dari loop.

![image](https://github.com/user-attachments/assets/da7b7f71-980f-4922-8614-24e9c71e793b)

# Automasi dengan Cron Job. Cron adalah layanan bawaan di Linux yang memungkinkan pengguna untuk menjalankan perintah atau skrip pada jadwal yang telah ditentukan.
1.  Buat Skrip yang Akan Dijalankan
    Buat skrip bernama log_time.sh untuk mencatat waktu eksekusi lalu tekan enter

![image](https://github.com/user-attachments/assets/f25e781c-7a66-4cfb-9b12-7e4fc1610b61)

2.	Isi skrip dengan mengetik seperti gambar dibawah setelah itu Simpan dan keluar (ctrl + o lalu ctrl + x).

![image](https://github.com/user-attachments/assets/ee32d397-fa29-452e-9a4a-5e69463b50ec)

3.	Beri izin eksekusi: dengan mengetik chmod +x  ~/log_time.sh lalu tekan enter

![image](https://github.com/user-attachments/assets/ceaf392b-ea5c-4e23-a38d-f52151525df1)

4.	Menjadwalkan Cron Job
    Buka crontab -e lalu tekan enter untuk mengedit

![image](https://github.com/user-attachments/assets/bddb4c45-a9b7-448e-8c25-470fd51f3fb7)

5.	tambahkan baris ini agar skrip berjalan setiap 1 menit:
    ketik * * * * * ~/log_time.sh lalu simpan dan keluar (ctrl + o dan ctrl + x)

![image](https://github.com/user-attachments/assets/b4600d79-f135-48bd-8022-4c1bf952135c)

6.	Memeriksa Apakah Cron Job Berjalan Lihat daftar cron job aktif:
    Ketik Crontab -l lalu enter

![image](https://github.com/user-attachments/assets/d920f74e-24de-4482-b832-acf0ad2c65a5)

7.	Cek isi file log: ketik cat  ~/log_time.txt lalu tekan enter
    Jika berhasil, file log akan terisi setiap menit dengan timestamp terbaru, menunjukkan bahwa tugas otomatis telah berjalan.

![image](https://github.com/user-attachments/assets/a5f2c5d6-0949-423d-97d1-f486503a9b61)

8.	Jika ada kesalahan seperti ini maka cara mengatasinya ada di nomor berikut

![image](https://github.com/user-attachments/assets/384be7e3-19ff-4864-840f-925e38c45fd0)

9.	Pastikan Skrip log_time.sh Sudah Dibuat dan Bisa Dieksekusi
    Jika skrip belum ada, buatlah dengan cara berikut lalu klik enter

![image](https://github.com/user-attachments/assets/2f538fe7-03ea-4372-943a-3a5aec7e5e6b)

10.  Setelah itu Isi dengan perintah dibawah lalu Simpan (ctrl + o) dan keluar (ctrl + x).

![image](https://github.com/user-attachments/assets/3f7cbcb5-9806-43cb-9492-80b9b84543be)

11.  Beri izin eksekusi, ketik chmod +x  ~/log_time.sh lalu klik enter

![image](https://github.com/user-attachments/assets/fe58ab97-2564-4f65-a194-6c898335f3b1)

12.  cek Apakah Cron Sedang Berjalan
     Pastikan cron aktif dengan mengetik sudo systemctl status cron lalu klik enter 

![image](https://github.com/user-attachments/assets/4ed3bc59-6b3c-4140-96ef-41b7ff7f6083)

13.	 Lalu masukkan password yang telah dibuat di akunnya lalu klik enter

![image](https://github.com/user-attachments/assets/7aa4b620-a9f2-4751-a107-b52ddf95b76b)

14.	 Setelah itu tampilannya akan seperti ini dan berhasil membuat cron job

![image](https://github.com/user-attachments/assets/7006c4e7-1ece-409b-b445-3ce8daa4d746)

# Automasi dengan Systemd timers, Systemd timers menjalankan unit layanan yang berisi perintah atau skrip yang akan dieksekusi.

1.	Buat file layanan (service) dengan cara ketik seperti dibawah lalu klik enter dan masukkan password akunnya lalu klik enter

![image](https://github.com/user-attachments/assets/b12c7aa2-36ce-4bfa-b47a-c0b4079d03df)

2.	Isi seperti gambar dibawah ini Lalu simpan (ctrl + o) dan keluar (ctrl + x)

![image](https://github.com/user-attachments/assets/d4112542-3908-42d6-be79-51ea5006d156)

3.	Buat file Timer (timer)
    Systemd timers mengontrol kapan layanan (service) dijalankan.
    Ketik seperti gambar dibawah lalu ketik enter

![image](https://github.com/user-attachments/assets/3c9bb81c-ac11-4f17-a34e-37928d2e8854)

4.	Isi seperti gambar dibawah ini Lalu simpan (ctrl + o) dan keluar (ctrl + x)

![image](https://github.com/user-attachments/assets/f01d34d4-8d70-41f7-9d7f-2bb8501cfbb4)

5.	Aktifkan Timer, Jalankan perintah berikut untuk mengaktifkan timer lalu klik enter

![image](https://github.com/user-attachments/assets/64e1e344-e1a9-4b58-92b2-296dcdd190fd)

6.	Periksa Status Timer Untuk melihat apakah timer aktif, gunakan perintah digambar ini lalu klik enter

![image](https://github.com/user-attachments/assets/9270e7fa-fe94-48da-88e0-af0180acd54a)

7.	Jika berhasil, kamu akan melihat hasil seperti berikut:

![image](https://github.com/user-attachments/assets/94631a73-b389-4af7-adaf-ebbc74f2931c)

# debugging dan logging menggunakan journalctl dan dmesg
1.  Debugging dengan journalctl (Systemd Logs) 
    Journalctl digunakan untuk melihat log dari layanan yang dikelola oleh        
    systemd, seperti cron, network, dan aplikasi lain.
    Cara Menggunakan journalctl
    - Melihat Semua Log Sistem dengan cara ketik seperti dibawah ini lalu klik enter

![image](https://github.com/user-attachments/assets/a3668561-88ed-447d-bd1f-03d9b493cb51)

2.  melihat Filter Log Berdasarkan Waktu dengan cara mengetik 
    Journalctl –since “30 minutes ago” lalu klik enter

![image](https://github.com/user-attachments/assets/8f660863-95ae-487c-8488-7553fb6eab88)

3.   Melihat Log dari Layanan Tertentu Misalnya, melihat log dari layanan cron:
     Ketik journalctl -u cron –No.-pager –since “10 minutes ago” lalu klik enter  
     maka tampilannya akan seperti ini

![image](https://github.com/user-attachments/assets/8bdbdfae-fa14-4315-9caa-48935390d0e6)

4.   Melihat Log Booting Terakhir dengan cara mengetik journalctl -b -1 lalu klik enter maka tampilannya akan seperti ini

![image](https://github.com/user-attachments/assets/153949b5-8f71-4176-a94d-c2f551856b7b)

5.   Menampilkan Log Secara Real-Time (Live Monitoring) dengan cara mengetik Journalctl -f lalu klik enter maka tampilannya akan seperti ini

![image](https://github.com/user-attachments/assets/8ed98259-ee09-4353-8cc4-f1aba38bf7a5)

6.  Debugging dengan dmesg (Kernel Logs)
    Dmesg digunakan untuk melihat log kernel yang mencatat informasi tentang hardware, driver, dan error sistem.
    Cara Menggunakan dmesg :
    Ketik sudo journalctl -k untuk menampilkan log kernel yang mencakup Informasi seperti :
    - Versi kernel yang digunakan (linux version 6.11.0-19-generic).
    - Command line yang digunakan saat booting.
    - CPU yang didukung oleh kernel (Intel, AMD, Hygon, Centaur, zhaoxin).
    - Firmware Bug terkait dengan frekuensi TSC (Time Stamp Counter).
    - BIOS-provided physical RAM map, yang menunjukkan area memori yang dapat digunakan.

![image](https://github.com/user-attachments/assets/9cd17871-bf01-4baa-82c0-768ca9d33bc5)
