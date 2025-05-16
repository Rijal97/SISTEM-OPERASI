D.    Implementasi
1.	Konfigurasi (mengatur) Jaringan VirtualBox
a.	Menggunakan NAT (Networl Address Translation)
Buka Settings (pengaturan) lalu pilih tab Network (jaringan). Attached to 
diatur ke NAT setelah itu tekan "ok”.

b.	Menggunakan Bridged Adapter
Kembali ke pengaturan Network, ubah Attached to menjadi Bridged Adapter setelah itu tekan "ok”. 
c.	Menggunakan Host-Only Adapter
Kembali ke pengaturan Network, ubah Attached to menjadi Host-Only Adapter setelah itu tekan "ok”.
 

2.	Menganalisis Konektivitas Jaringan
a.	Perintah ip a dan ping 
1)	Jaringan NAT 
-	Ketik ip a untuk lihat alamat IP di bagian 2: enp0s3: inet 10.0.2.15/24 
-	Ketik ping 8.8.8.8 untuk memastikan sistem terhubung ke internet dan dapat menjangkau jaringan luar.









2)	  Jaringan Bridged Adapter:
-	Ketik ip a untuk lihat alamat IP di bagian 2: enp0s3: inet 172.16.45.105/24 
-	Ketik ping 8.8.8.8 untuk memastikan sistem terhubung ke internet dan dapat menjangkau jaringan luar.

3)	Jaringan Host-Only Adapter
-	Ketik ip a untuk lihat alamat IP di bagian 2: enp0s3: 
inet 192.168.56.101/24 



-	Ketik ping 8.8.8.8 untuk memastikan sistem terhubung ke internet dan dapat menjangkau jaringan luar.
-	Jika menggunakan Host-Only,maka gunakan ping ke IP host

3.	Mengakses Sistem Linux dengan SSH dan Transfer File
a.	Mengaktifkan SSH
-	Menginstall OpenSSH Server : sudo apt install openssh-server. 
 
-	Jika sudah diinstall, aktifkan dengan sudo systemctl enable ssh dan jalankan layanan dengan sudo systemctl start ssh.
 



b.	Akses dari Host ke VM
Gunakan perintah ssh username@ip_vm dari host. Misalnya: 
ssh bibul@192.168.100.213



c.	Transfer File dengan SCP
Kirim file dari host ke VM: 
1)	Siapkan file yang akan dikirim
-	ls 
-	echo “modul 5 cok” > file_scp.txt
2)	lakukan transfer file dengan scp
-	scp tugas5.txt bibul@192.168.100.213
File tugas5.txt dikirim dari VM1 ke user bibul di VM2 (192.168.100.213) ditempatkan di direktori /home/vboxuser/
-	Setelah menekan “Enter” masukkan password user bibul di VM2 lalu “Enter”.
-	Verifikasi file sudah diterima di VM2, login ke VM2 lalu cek file-nya dan cat tugas5.txt untuk melihat isi file

4.	Melakukan Koneksi Antar-PC di Jaringan Lokal
a.	Pastikan kedua VM dalam Jaringan yang sama, gunakan Host-Only Adapter pada dua VM. Cek IP dengan ip a. IP harus berada dalam subnet yang sama, misal 192.168.56.101 dan 192.168.56.101.
-	Cek ip a dari VM 1
-	Cek ip a dari VM 2

b.	Coba Ping Antar Mesin
Dari VM1 ketik  ping 192.168.56.101 Jika berhasil, berarti koneksi antar mesin sudah aktif.


c.	Mengelola Firewall Menggunakan UFW 
a.	Mengaktifkan dan Mengatur UFW
Mengaktifkan firewall untuk melindungi sistem dari akses luar yang tidak diinginkan, UFW digunakan untuk mengatur izin atau larangan akses jaringan ke sistem
-	Instal UFW jika belum ada : sudo apt install ufw
-	Aktifkan		                : sudo ufw enable (mengaktifkan 
				     firewall)
-	Izinkan SSH	                : sudo ufw allow 22 (buka akses 
				     SSH)
-	Lihat status                        	  : sudo ufw status (menampilkan 
				    aturan firewall)

b.	Menutup dan Membuka Port
-	Blokir SSH        : sudo ufw deny 22
-	Buka kembali : sudo ufw allow 22
 
d.	Mengelola User dan Grup
a.	Membuat User Baru
-	sudo adduser cuy	(menambah user baru)
-	sudo deluser cuy	(menghapus user)
-	cat /etc/passwd	(lihat daftar user)
		          Ikuti instruksi untuk membuat password dan informasi profil.


b.	Membuat Grup Baru
-	sudo groupadd modul5		(menambah grup baru)
-	sudo delgroup modul5		(menghapus grup)
-	cat /etc/group 			(lihat daftar grup)
-	sudo usermod -aG Modul5 cuy	(tambahkan user ke grup)
 
 
c.	Mengubah Kepemilikan File
-	Sudo chown cuy tugas.txt		  (ubah owner)
-	sudo chown cuy:modul5 tugas.txt (ubah owner:group)
-	ls -l				     (lihat detail file atau folder)


d.	Mengatur Hak Akses
-	chmod 700 tugas.txt : hanya pemilik yang bisa baca, tulis, dan eksekusi
-	chmod 750 tugas.txt        :  pemilik full akses, grup bisa baca & eksekusi
