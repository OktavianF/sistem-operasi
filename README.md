 **Laporan Praktikum - Instalasi Ubuntu**

1. Pendahuluan
Pada laporan praktikum atau tugas ini, saya akan menginstal Linux Ubuntu dalam Virtualbox.
2. Persiapan Instalasi
Sebelum memulai instalasi, pastikan perangkat memenuhi spesifikasi berikut:

-CPU: 2 core
-RAM: 4 GB
-HDD: 25 GB (dibagi menjadi: / 20GB, /storage 5GB, swap 1.5GB)
-Software: VirtualBox
-File ISO: Ubuntu
3. Langkah-Langkah Instalasi
  3.1 Membuat Virtual Machine di VirtualBox
      Buka VirtualBox, klik New untuk membuat VM baru.
      Masukkan nama dan pilih sistem operasi
      Atur RAM minimal 4096 MB (4 GB).
      Pilih Create a virtual hard disk now, lalu pilih VDI (Virtual Disk Image).
      Atur kapasitas 25 GB, lalu klik Create.
  3.2 Menyiapkan Penyimpanan dan Boot ISO
      Pilih VM, masuk ke Settings → Storage.
      Klik ikon CD di bawah "Controller: IDE" dan pilih Choose a disk file....
      Pilih file ISO Debian/Ubuntu, lalu klik OK.
  3.3 Proses Instalasi OS
      Jalankan VM dan pilih Install atau Graphical Install.
      Ikuti langkah-langkah berikut:
      -Pilih bahasa, zona waktu, dan tata letak keyboard.
      -Masukkan hostname.
      -Buat akun pengguna dan kata sandi.
      -Konfigurasi partisi.
      -Lanjutkan instalasi hingga selesai.
      -Instal bootloader GRUB jika diminta.
  3.4 Menyelesaikan Instalasi
      Setelah instalasi selesai, sistem akan meminta restart.
      Eject file ISO dari pengaturan VirtualBox.
      Boot ulang VM dan masuk ke sistem operasi yang telah terinstal.
**Kesimpulan**
Instalasi Debian atau Ubuntu di VirtualBox dapat dilakukan dengan mudah jika mengikuti langkah-langkah dengan benar. Spesifikasi hardware yang sesuai sangat berpengaruh terhadap performa sistem. Pemahaman tentang partisi juga penting agar sistem berjalan optimal.
