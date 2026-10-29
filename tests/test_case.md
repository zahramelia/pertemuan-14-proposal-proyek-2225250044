# Test Case Program Rekap dan Analisis Nilai Matematika Kelas

Dokumen ini berisi rancangan pengujian awal untuk memastikan program dapat memproses data nilai sesuai kebutuhan.

| ID | Kategori | Input/Kondisi | Hasil yang Diharapkan |
|---|---|---|---|
| TC01 | Normal | Nilai 80, 70, 90 | Rata-rata 80, nilai tertinggi 90, nilai terendah 70 |
| TC02 | Batas | Nilai 0 | Diterima sebagai nilai valid |
| TC03 | Batas | Nilai 100 | Diterima sebagai nilai valid |
| TC04 | Invalid | Nilai 105 | Ditolak dengan pesan validasi |
| TC05 | Invalid | File data tidak ditemukan | Kesalahan file ditangani dengan pesan yang sesuai |
| TC06 | Normal | Nilai 80, 70, 90 dengan KKM 60 | Jumlah tuntas 3 dan belum tuntas 0 |
| TC07 | Invalid | File data kosong | Program menampilkan pesan bahwa tidak ada data yang dapat dianalisis |

**Catatan:** Test case ini merupakan rancangan pengujian. Hasil aktual akan diperiksa setelah program diimplementasikan.
