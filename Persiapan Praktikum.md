# Tugas Pendahuluan - Instalasi Ubuntu

## 1. Pendahuluan
Pada laporan praktikum atau tugas ini, saya akan menginstal Linux Ubuntu dalam VirtualBox.

## 2. Persiapan Instalasi
Sebelum memulai instalasi, pastikan perangkat memenuhi spesifikasi berikut:

- **CPU**: 2 core  
- **RAM**: 4 GB  
- **HDD**: 25 GB (dibagi menjadi: `/` 20GB, `/storage` 5GB, `swap` 1.5GB)  
- **Software**: VirtualBox  
- **File ISO**: Ubuntu  

## 3. Langkah-Langkah Instalasi

### 3.1 Membuat Virtual Machine di VirtualBox
1. Buka **VirtualBox**, klik **New** untuk membuat VM baru.  
2. Masukkan **nama** dan pilih **sistem operasi**.  
3. Atur **RAM** minimal **4096 MB (4 GB)**.  
4. Pilih **Create a virtual hard disk now**, lalu pilih **VDI (Virtual Disk Image)**.  
5. Atur kapasitas **25 GB**, lalu klik **Create**.  

### 3.2 Menyiapkan Penyimpanan dan Boot ISO
1. Pilih **VM**, masuk ke **Settings → Storage**.  
2. Klik ikon **CD** di bawah "Controller: IDE" dan pilih **Choose a disk file...".  
3. Pilih file **ISO Debian/Ubuntu**, lalu klik **OK**.  

### 3.3 Proses Instalasi OS
1. Jalankan **VM** dan pilih **Install** atau **Graphical Install**.  
2. Ikuti langkah-langkah berikut:
   - Pilih **bahasa**, **zona waktu**, dan **tata letak keyboard**.  
   - Masukkan **hostname**.  
   - Buat **akun pengguna** dan **kata sandi**.  
   - Konfigurasi **partisi**.  
   - Lanjutkan **instalasi** hingga selesai.  
   - Instal **bootloader GRUB** jika diminta.  

### 3.4 Menyelesaikan Instalasi
1. Setelah instalasi selesai, sistem akan meminta **restart**.  
2. **Eject file ISO** dari pengaturan VirtualBox.  
3. Boot ulang **VM** dan masuk ke sistem operasi yang telah terinstal.  

## Kesimpulan
Instalasi Debian atau Ubuntu di VirtualBox dapat dilakukan dengan mudah jika mengikuti langkah-langkah dengan benar. Spesifikasi hardware yang sesuai sangat berpengaruh terhadap performa sistem. Pemahaman tentang partisi juga penting agar sistem berjalan optimal.


# Tugas Pendahuluan - Perbedaan Debian 12 (Bookworm) dengan Debian 11 (Bullseye)

## 1. Perbedaan Versi Kernel
| Debian Version | Kernel Version |
|---------------|---------------|
| Debian 11 (Bullseye) | 5.10 LTS |
| Debian 12 (Bookworm) | 6.1 LTS |

## 2. Kebutuhan Sistem
| Debian Versionn | Minimum RAM | Minimum Storage |
|---------------|------------|----------------|
| Debian 11 (Bullseye) | 512 MB | 10 GB |
| Debian 12 (Bookworm) | 1 GB | 20 GB |

## 3. Penerapan Systemd
Debian 12 menggunakan systemd versi lebih baru dibandingkan Debian 11, yang memberikan peningkatan dalam manajemen layanan dan proses booting yang lebih cepat.

## 4. Perbedaan Paket dan Perubahan Software
| Perubahan | Debian 11 (Bullseye) | Debian 12 (Bookworm) |
|-----------|----------------------|----------------------|
| Versi GCC | 10 | 12 |
| Python | 3.9 | 3.11 |
| LibreOffice | 7.0 | 7.4 |
| GNOME | 3.38 | 43 |
| KDE Plasma | 5.20 | 5.27 |

## Kesimpulan
Debian 12 membawa banyak peningkatan dibandingkan Debian 11, termasuk kernel yang lebih baru, peningkatan kebutuhan sistem, versi software yang lebih mutakhir, serta peningkatan performa melalui systemd terbaru. Jika menginginkan stabilitas dengan software terbaru, Debian 12 adalah pilihan yang lebih baik dibandingkan Debian 11.


# Tugas Pendahuluan - Cek Environment dengan CPU-Z
### Langkah-langkah:
1. **Download dan install CPU-Z** dari [CPU-Z Official](https://www.cpuid.com/softwares/cpu-z.html).
2. **Menjalankan CPU-Z**
   - **CPU**: Model, jumlah core, clock speed.
   - **Memory (RAM)**: Kapasitas, tipe, dan frekuensi.
   - **Motherboard**: Merk, model, dan chipset.
   - **Graphics**: Jenis GPU dan kapasitas VRAM.

### Hasil Pengujian:
| Komponen | Spesifikasi |
|----------|-------------|
| CPU | 2 core |
| RAM | 4GB |

### Kesimpulan:
Dengan CPU-Z, saya dapat dengan mudah mendapatkan informasi mendetail mengenai spesifikasi perangkat keras yang digunakan, membantu dalam troubleshooting dan optimalisasi sistem.


# Tugas Pendahuluan - Mencari Info Aplikasi dari Hardware Menggunakan Shell
### Perintah yang digunakan:
- **Melihat daftar perangkat keras:**
  ```bash
  lshw -short
  ```
- **Cek driver perangkat keras:**
  ```bash
  lspci -k
  ```
- **Melihat perangkat USB yang terhubung:**
  ```bash
  lsusb
  ```
- **Menampilkan modul kernel yang digunakan:**
  ```bash
  lsmod
  ```
- **Menampilkan aplikasi terkait firmware/hardware:**
  ```bash
  dpkg --list | grep -i firmware
  ```

### Hasil Pengujian:
| Perintah | Output |
|----------|--------|
| `lshw -short` | Menampilkan daftar perangkat keras yang terdeteksi. |
| `lspci -k` | Menunjukkan perangkat PCI dan driver yang digunakan. |
| `lsusb` | Daftar perangkat USB yang terhubung. |
| `lsmod` | Modul kernel yang sedang aktif. |
| `dpkg --list | grep -i firmware` | Menampilkan daftar paket firmware yang terinstal. |

## Kesimpulan:
Dengan menggunakan perintah shell di Linux, kita dapat memperoleh informasi detail mengenai perangkat keras dan aplikasi terkait tanpa perlu menggunakan GUI, sehingga lebih efisien untuk troubleshooting dan administrasi sistem.

# Kesimpulan Akhir
Debian 12 membawa banyak peningkatan dibandingkan Debian 11, termasuk kernel terbaru, perubahan pada software, serta sistem yang lebih optimal. Selain itu, pemahaman tentang spesifikasi perangkat keras menggunakan CPU-Z dan perintah shell membantu dalam menganalisis serta mengelola sistem lebih efektif.

