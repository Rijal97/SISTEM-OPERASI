E. Implementasi
1. Docker
a. Cek katalog software terbaru dari server 
- Ketik sudo apt update untuk mengecek katalog software terbaru
 
b. Lakukan instalasi Docker pada Linux dengan: sudo apt install docker.io
 
c. Memulai layanan Docker
- sudo systemctl start docker: Perintah ini digunakan untuk memulai layanan Docker secara langsung pada sistem Linux. Setelah perintah ini dijalankan, Docker akan aktif dan siap digunakan.
- sudo systemctl enable docker: perintah ini digunakan untuk mengatur agar layanan Docker dijalankan secara otomatis setiap kali sistem dinyalakan (booting).
 
d. Cek versi docker menggunakan perintah docker --version
 
e. Setelah Docker berhasil terinstal dan dapat digunakan, gunakan sudo usermod -aG docker $USER untuk menambahkan user ke grup Docker supaya bisa menjalankan Docker tanpa sudo. 
 
f.  Download sistem Ubuntu (versi ringan) agar bisa dijalankan di dalam Docker dengan: docker pull ubuntu. Kemudian gunakan docker images untuk melihat semua image Docker yang sudah di-download.
 
i. Gunakan docker run -it python untuk untuk menjalankan python di dalam Docker. Lalu cobalah untuk mencoba dan menjalankannya.
  
j. -xhost +local:docker	
- Gunakan -xhost +local:docker untuk mengizinkan koneksi local dari user atau grup bernama docker ke server X11 agar bisa menampilkan aplikasi GUI ke layar host pengguna.	
- Gunakan -Xhost untuk menampilkan koneksi yang diizinkan untuk server pengguna yang artinya kontrol akses X11 dan hanya klien yang terotorisasi yang dapat terhubung.

k. Menjalankan aplikasi GUI dari dalam container Docker dan menampilkannya di layar host dengan docker run -it (menjalankan container secara interaktif dan membuka terminal (-i = interactive, -t = terminal)).
 
l. Gunakan perintah apt upt update && apt install -y pyhton3-tk untuk menginstal Tkinter, yaitu pustaka GUI untuk Python agar dapat menjalankan aplikasi GUI berbasis Tkinter dari dalam container dan menampilkannya di layar host.
 
m. Mengunduh paket NumPy dan Matplotlib beserta seluruh dependensi yang dibutuhkan dari Python Package Index (PyPI) dengan: pip install numpy matplotlib
 
n. Cobalah untuk menampilkan grafik dari dalam Docker menggunakan Matplotlib dan NumPy untuk melihat apakah grafik sudah bisa ditampilkan atau tidak, jika berhasil, maka:
- Python, NumPy, dan Matplotlib sudah terinstal dengan benar.
- Tkinter dan X11 GUI dari Docker ke host berfungsi.
- Docker siap untuk menjalankan aplikasi Python berbasis grafik.
  
j. Menampilkan semua container Docker
- docker ps -a: menampilkan semua container; baik yang sedang berjalan maupun berhenti
 
2. Virtualenv
1. Menampilkan grafik dengan library numpy dan matplotlib di dalam Virtualenv
a. Lakukan proses instalasi python3-virtualenv di terminal Linux menggunakan perintah: sudo apt install python3-virtualenv
 
b. Aktifkan Virtualenv dengan: virtualenv env
 
c. Gunakan sorce env//bin/activate untuk mengaktifkan virtual environment Python di Linux.
 
d. Install matplotlib dengan: pip install matplotlib

e. Gunakan sorce/env/bin/activate untuk menjalankan kode python yang telah dibuat serta menampilkan grafiknya di dalam virtualenv.
