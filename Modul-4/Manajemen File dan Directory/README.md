#D.  IMPLEMENTASI
1.	Membuat dan mengelola file
a.	Membuat directory 
•	Perintah mkdir Modul4
Perintah ini digunakan untuk membuat direktori (folder) baru dengan nama Modul4. Setelah perintah ini dijalankan, direktori Modul4 dibuat di direktori saat ini (home directory pengguna Izzul_Faraby).
•	Perintah ls
Perintah ini digunakan untuk menampilkan daftar file dan direktori yang ada di direktori saat ini. Hasil dari ls menunjukkan berbagai file dan folder, termasuk direktori baru yang baru saja dibuat (Modul4).
 


b.	Membuat file
•	Perintah touch file1.txt
-	Perintah ini digunakan untuk membuat file kosong baru bernama file1.txt di dalam direktori Modul4.
-	touch adalah perintah yang biasanya dipakai untuk Membuat file baru jika file tersebut belum ada.
 

c.	Membuat folder
•	Perintah mkdir folderbaru
mkdir adalah singkatan dari make directory, digunakan untuk membuat direktori/folder baru. Dalam hal ini, kamu membuat direktori bernama folderbaru di dalam direktori Modul4


 

d.	Mengcopy paste file 
•	Perintah cp file1.txt folderbaru
-	cp adalah perintah untuk copy atau menyalin file.
-	Di sini kamu menyalin file1.txt yang berada di direktori Modul4 ke dalam subdirektori folderbaru.
-	Setelah perintah ini dijalankan, akan ada dua salinan dari file1.txt: satu di Modul4 dan satu lagi di Modul4/folderbaru.
•	Perintah cd folderbaru
Kamu masuk ke direktori folderbaru menggunakan cd.
•	Perintah ls
Kamu mengecek isi folder folderbaru, dan hasilnya menunjukkan bahwa file1.txt sudah berada di dalam folder tersebut.

 

e.	Menghapus file dan folder
•	Ls
Menampilkan isi direktori Modul4, terlihat ada:
•	rm filesampah.txt
Perintah ini digunakan untuk menghapus file bernama filesampah.txt. Setelah dijalankan, file tersebut sudah tidak ada lagi di direktori.
•	rmdir foldersampah
Perintah ini digunakan untuk menghapus direktori kosong bernama foldersampah. rmdir hanya bisa digunakan jika folder tersebut kosong.
•	ls lagi
Digunakan untuk mengecek hasil penghapusan.
 

f.	Mengubah nama file
•	Ls
-	Menampilkan isi direktori Modul4.
-	Terdapat file bernama file1.txt dan folder bernama folderbaru.
•	mv file1.txt file2.txt
-	Ini adalah perintah untuk mengganti nama file file1.txt menjadi file2.txt.
-	Perintah mv bisa digunakan untuk memindahkan file ke lokasi lain atau mengganti nama file (seperti dalam contoh ini).

 


g.	Memindahkan file di dalam folder yang sama
•	Ls
Perintah ini digunakan untuk menampilkan isi direktori Modul4. Terlihat terdapat:
•	mv file2.txt folderbaru
Perintah ini berarti:
-	mv = move (memindahkan)
-	file2.txt dipindahkan ke dalam folder folderbaru
•	ls (lagi)
Setelah perintah mv, user mengecek kembali isi direktori Modul4, dan sekarang hanya tersisa:
•	cd folderbaru
Masuk ke dalam folder folderbaru.
•	Ls
Perintah ini menampilkan isi dari folder folderbaru, dan hasilnya adalah:
-	file1.txt (sudah ada sebelumnya)
-	.txt (yang baru saja dipindahkan)

 

h.	Memindahkan file di luar folder yang ingin dipindahkan
•	mv file2.txt /home/Izzul_Faraby/Modul4
Perintah ini memindahkan:
File file2.txt dari direktori saat ini (folderbaru) Ke direktori /home/Izzul_Faraby/Modul4, yaitu folder induk Modul4
•	ls
Menampilkan isi folder saat ini
•	cd ..
berpindah directory satu Langkah ke belakang
•	ls
Menampilkan isi Modul4, sekarang sudah ada:
-	file2.txt (hasil pindahan)
-	folderbaru

 

2.	Mengatur izin akses

a.	Mengubah dengan Symbol
•	chmod u+x file2.txt
Menambahkan izin eksekusi (x) ke pemilik file (user/u).
•	chmod g+x file2.txt
Menambahkan izin eksekusi ke grup (group/g).
•	chmod o+w file2.txt
Menambahkan izin tulis (write) ke others (pengguna lain).
•	chmod ug-x file2.txt
Menghapus izin execute (x) dari user (u) dan group (g).
 

b.	Mengubah dengan Oktal

•	Perintah: chmod 755 file2.txt
Artinya kamu memberikan izin sebagai berikut:
7 (user) = rwx (read, write, execute)
5 (group) = r-x (read, execute)
5 (others) = r-x (read, execute)
•	Perintah chmod 000 file2.txt
Ini akan menghapus semua izin dari semua pihak:
0 (user) = ---
0 (group) = ---
0 (others) = ---

 


3.	Mengubah kepemilikan
a.	Membuat User
•	sudo adduser jumadil
Menjalankan perintah adduser sebagai administrator (sudo) untuk membuat akun baru bernama jumadil.
•	Pembuatan User dan Grup
Sistem membuat:
-	User junadil
-	Grup dengan nama dan ID sama (junadil (1001))
-	Home directory: /home/junadil
-	Menyalin file default dari /etc/skel ke home directory.

•	Password
Sistem meminta untuk membuat password. Meskipun ada peringatan "BAD PASSWORD" (karena kurang dari 8 karakter), password tetap diterima setelah dikonfirmasi dua kali.
•	Informasi Profil
Sistem meminta data tambahan seperti:
-	Nama lengkap (junadil_akhir)
-	Nomor ruangan, telepon, dll (semua dikosongkan)
•	Konfirmasi
Setelah menjawab y (yes), sistem menambahkan user junadil ke grup tambahan users.

 

b.	Mengubah kepemilikan
•	ls -l
Menampilkan detail file dan folder di direktori Modul4.
•	sudo chown jumadil file2.txt
-	Perintah ini mengubah pemilik file file2.txt menjadi jumadil, tapi grup-nya tetap Izzul_Faraby.
-	sudo digunakan karena hanya root atau pemilik file yang bisa mengubah kepemilikan.
•	sudo chown junadil folderbaru
Sama seperti sebelumnya, tapi kali ini diterapkan ke folder folderbaru.
•	ls -l
Untuk melihat detai file dan folder di directory Modul4
Hasil akhir:
-	file2.txt → dimiliki oleh junadil : Izzul_Faraby
-	folderbaru → dimiliki oleh junadil : Izzul_Faraby

 

c.	Mengubah kepemilikan secara menyeluruh dalam satu folder
•	cd ..
untuk mundur selangkah dari directory saat ini
•	ls -l
Untuk melihat detai file dan folder 
•	sudo chown -R junadil:junadil Modul4
digunakan untuk mengubah kepemilikan direktori Modul4 beserta seluruh isinya secara rekursif, di mana sudo menjalankan perintah sebagai administrator, chown adalah perintah untuk mengubah pemilik dan grup file, opsi -R membuat perubahan berlaku ke seluruh isi folder, junadil:junadil menetapkan pemilik dan grup menjadi junadil, dan Modul4 adalah direktori target yang ingin diubah kepemilikannya.
