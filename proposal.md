# PROPOSAL PROYEK

## 1. Judul Proyek

**Program Rekap dan Analisis Nilai Matematika Kelas**

## 2. Latar Belakang

Pengolahan nilai siswa merupakan salah satu kegiatan yang dilakukan dalam pembelajaran matematika. Guru perlu mengetahui rata-rata nilai, nilai tertinggi, nilai terendah, serta jumlah siswa yang telah mencapai Kriteria Ketuntasan Minimal (KKM).

Apabila pengolahan nilai dilakukan secara manual, proses perhitungan dan rekapitulasi dapat membutuhkan waktu lebih lama serta berisiko menimbulkan kesalahan. Oleh karena itu, diperlukan program sederhana yang dapat membantu mengolah data nilai siswa secara lebih praktis dan sistematis.

Proyek ini dirancang menggunakan bahasa pemrograman Python untuk membaca data nilai dari file, memvalidasi nilai, menghitung statistik nilai, menentukan ketuntasan berdasarkan KKM, dan menyimpan hasil analisis ke dalam file teks.

## 3. Pengguna dan Tujuan

### Pengguna
Pengguna utama program ini adalah guru matematika yang membutuhkan bantuan untuk merekap dan menganalisis nilai siswa. Program ini juga dapat digunakan oleh mahasiswa untuk mempelajari penerapan algoritma dan pemrograman dalam pengolahan data nilai.

### Tujuan
1. Mempermudah proses rekapitulasi nilai matematika siswa.
2. Memvalidasi nilai agar berada pada rentang 0 sampai 100.
3. Menghitung rata-rata, nilai tertinggi, dan nilai terendah.
4. Menentukan jumlah siswa yang tuntas dan belum tuntas berdasarkan KKM.
5. Menyimpan hasil analisis ke dalam file teks agar mudah dibaca kembali.

## 4. Ruang Lingkup

### Fitur Wajib
1. Membaca data nilai matematika siswa dari file teks.
2. Memvalidasi nilai agar berada pada rentang 0 sampai 100.
3. Menghitung rata-rata nilai siswa.
4. Menentukan nilai tertinggi dan nilai terendah.
5. Menghitung jumlah siswa yang tuntas dan belum tuntas berdasarkan KKM.
6. Menyimpan laporan hasil analisis ke dalam file teks.

### Batasan Proyek
1. Program dijalankan melalui terminal atau command line.
2. Program dibuat menggunakan bahasa pemrograman Python.
3. Nilai siswa harus berada pada rentang 0 sampai 100.
4. KKM awal ditetapkan sebesar 60.
5. Program menggunakan file teks untuk membaca data dan menyimpan laporan.
6. Program tidak menggunakan database, antarmuka grafis (GUI), atau aplikasi berbasis web.

## 5. Kebutuhan

### A. Kebutuhan Fungsional
1. Program dapat membaca data nilai siswa dari file teks.
2. Program dapat memeriksa apakah nilai berada pada rentang 0 sampai 100.
3. Program dapat menghitung rata-rata, nilai tertinggi, dan nilai terendah.
4. Program dapat menentukan jumlah siswa yang tuntas dan belum tuntas berdasarkan KKM.
5. Program dapat menyimpan hasil analisis ke dalam file laporan teks.
6. Program dapat memberikan pesan kesalahan apabila file tidak ditemukan atau data nilai tidak valid.

### B. Kebutuhan Nonfungsional
1. Program menggunakan bahasa pemrograman Python.
2. Program dapat dijalankan melalui terminal di Visual Studio Code.
3. Program memiliki struktur kode yang sederhana dan mudah dipahami.
4. Program menggunakan file teks untuk menyimpan data dan laporan.
5. Program menampilkan hasil perhitungan dengan jelas dan mudah dibaca.

## 6. IPO (Input, Process, Output)

### A. Input
1. File teks yang berisi data nilai matematika siswa.
2. Nilai siswa dalam rentang 0 sampai 100.
3. Nilai KKM yang digunakan untuk menentukan ketuntasan, dengan nilai awal 60.

### B. Process
1. Membaca data nilai dari file teks.
2. Memeriksa ketersediaan file dan validitas data nilai.
3. Memastikan setiap nilai berada pada rentang 0 sampai 100.
4. Menghitung rata-rata, nilai tertinggi, dan nilai terendah.
5. Membandingkan setiap nilai dengan KKM untuk menentukan ketuntasan.
6. Menghitung jumlah siswa yang tuntas dan belum tuntas.
7. Menyusun laporan hasil analisis dan menyimpannya ke file teks.

### C. Output
1. Daftar nilai yang valid.
2. Rata-rata nilai siswa.
3. Nilai tertinggi dan nilai terendah.
4. Jumlah siswa yang tuntas dan belum tuntas.
5. Laporan hasil analisis dalam file teks.

## 7. Algoritma

### Pseudocode

```text
MULAI
    Baca data nilai dari file teks

    JIKA file tidak ditemukan
        Tampilkan pesan kesalahan
        SELESAI
    AKHIR JIKA

    Periksa apakah data nilai tersedia

    JIKA data kosong atau tidak valid
        Tampilkan pesan kesalahan
        SELESAI
    AKHIR JIKA

    Untuk setiap nilai dalam data
        Periksa apakah nilai berada pada rentang 0–100
    AKHIR UNTUK

    Jika terdapat nilai tidak valid
        Tampilkan pesan kesalahan
    SELAIN ITU
        Hitung rata-rata nilai
        Tentukan nilai tertinggi
        Tentukan nilai terendah

        Hitung jumlah siswa yang tuntas
        Hitung jumlah siswa yang belum tuntas

        Susun laporan hasil analisis
        Simpan laporan ke file teks
        Tampilkan laporan
    AKHIR JIKA
SELESAI
```

## 8. Struktur Program

Program dirancang menggunakan beberapa modul agar setiap bagian memiliki tugas yang jelas dan mudah diuji.

### Rancangan Modul dan Fungsi

1. **main.py**
   - Fungsi `main()` untuk mengatur alur utama program dan menampilkan hasil analisis.

2. **data_io.py**
   - Fungsi `baca_nilai()` untuk membaca data nilai dari file teks.
   - Fungsi `simpan_laporan()` untuk menyimpan hasil analisis ke file teks.

3. **analisis.py**
   - Fungsi `validasi_nilai()` untuk memeriksa rentang nilai.
   - Fungsi `hitung_rata_rata()` untuk menghitung rata-rata.
   - Fungsi `cari_nilai_tertinggi()` untuk menentukan nilai tertinggi.
   - Fungsi `cari_nilai_terendah()` untuk menentukan nilai terendah.
   - Fungsi `hitung_ketuntasan()` untuk menghitung jumlah siswa yang tuntas dan belum tuntas.

4. **utilitas.py**
   - Fungsi pendukung untuk menampilkan pesan kesalahan dan membantu proses program.

   ## 9. Struktur Data

Struktur data yang digunakan dalam program ini adalah sebagai berikut.

1. **List**
   
   Digunakan untuk menyimpan kumpulan nilai siswa yang telah dibaca dari file teks.

2. **Float atau Integer**
   
   Digunakan untuk menyimpan nilai siswa dan hasil perhitungan statistik. Nilai dapat berupa bilangan bulat maupun desimal.

3. **String**
   
   Digunakan untuk menyimpan nama file, pesan kesalahan, status ketuntasan, dan isi laporan.

4. **File Teks**
   
   Digunakan sebagai media penyimpanan data nilai dan laporan hasil analisis.

Struktur data tersebut dipilih karena sederhana, sesuai dengan kebutuhan proyek, dan dapat diterapkan menggunakan dasar-dasar pemrograman Python.

## 10. Test Case

Pengujian awal dirancang untuk memastikan program dapat menangani data normal, nilai batas, data tidak valid, dan kondisi file yang bermasalah.

| No. | Kondisi Pengujian | Input | Hasil yang Diharapkan |
|---|---|---|---|
| 1 | Data nilai normal | 80, 70, 90 | Rata-rata 80, nilai tertinggi 90, nilai terendah 70. |
| 2 | Nilai batas bawah | 0 | Nilai diterima karena berada pada rentang 0–100. |
| 3 | Nilai batas atas | 100 | Nilai diterima karena berada pada rentang 0–100. |
| 4 | Nilai di luar rentang | 105 | Program menolak nilai dan menampilkan pesan kesalahan. |
| 5 | File tidak ditemukan | File nilai tidak tersedia | Program menampilkan pesan bahwa file tidak ditemukan. |
| 6 | Seluruh siswa tuntas | 80, 70, 90 dengan KKM 60 | Jumlah siswa tuntas adalah 3 dan belum tuntas adalah 0. |
| 7 | File tanpa data nilai | File kosong | Program menampilkan pesan bahwa data nilai kosong. |

Test case tersebut merupakan rancangan pengujian awal. Hasil aktual akan diperiksa ketika program diimplementasikan dan diuji pada tahap berikutnya.

## 11. Pembagian Tugas

Proyek ini dikerjakan secara individu. Seluruh tahapan perancangan, implementasi, pengujian, dan dokumentasi menjadi tanggung jawab satu orang.

| No. | Tugas | Penanggung Jawab |
|---|---|---|
| 1 | Menyusun rancangan dan proposal proyek | Zahra Amelia |
| 2 | Membuat struktur folder dan program Python | Zahra Amelia |
| 3 | Mengembangkan fungsi pembacaan dan penyimpanan file | Zahra Amelia |
| 4 | Mengembangkan fungsi analisis dan perhitungan nilai | Zahra Amelia |
| 5 | Menyusun dan menjalankan test case serta melakukan debugging | Zahra Amelia |
| 6 | Membuat dokumentasi dan mengelola repository GitHub | Zahra Amelia |

## 12. Jadwal Proyek

| Tahap | Kegiatan | Target |
|---|---|---|
| Pertemuan 14 | Perancangan proyek | Proposal, struktur repository, pseudocode, dan test case selesai. |
| Antara Pertemuan 14–15 | Implementasi awal | Struktur program dan fitur utama mulai dibuat menggunakan Python. |
| Pertemuan 15 | Integrasi, pengujian, dan debugging | Seluruh fitur terintegrasi, test case dijalankan, dan kesalahan diperbaiki. |
| Pertemuan 16 | Presentasi dan evaluasi | Program didemonstrasikan dan hasil proyek dipresentasikan. |

## 13. Repository

Repository proyek akan dibuat di GitHub dengan nama `pertemuan-14-proposal-proyek-2225250044`.

URL Repository: https://github.com/zahramelia/pertemuan-14-proposal-proyek-2225250044
