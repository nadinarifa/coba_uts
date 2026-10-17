# Analisis Masalah Modul A

**Studi Kasus 9: Sistem Pemeriksaan Anggaran Kegiatan Mahasiswa**

## 1. Latar Belakang dan Rumusan Masalah

### 1.1 Latar Belakang

Di pelaksanaan kegiatan mahasiswa, pengeluaran sering tidak sama dengan anggaran yang direncanakan. Perbedaan kedua nilai tersebut perlu diperiksa agar penggunaan dana bisa diketahui secara jelas. Jika pemeriksaan dilakukan secara manual, bendahara bisa salah menghitung persentase atau terlambat menyadari bahwa pengeluarannya melebihi anggaran. Karena itu dibutuhkan program yang bisa memeriksa setiap komponen anggaran secara konsisten dan memberikan status yang jelas.

Modul A berfokus pada pemeriksaan anggaran di setiap komponen, dengan cara membandingkan anggaran rencana dan realisasi pengeluaran. Program menghitung selisih dan persentase penyimpangan, kemudian menentukan status anggaran serta keterangan apabila terjadi kelebihan pengeluaran.

### 1.2 Rumusan Masalah

Berdasarkan latar belakang, masalah yang perlu diselesaikan adalah:

1. Bagaimana membandingkan anggaran rencana dengan realisasi pengeluaran setiap komponen?
2. Bagaimana menghitung selisih dan persentase penyimpangan anggaran?
3. Bagaimana menentukan status anggaran berdasarkan hasil perbandingan?
4. Bagaimana memberikan keterangan ketika pengeluaran melebihi anggaran?
5. Bagaimana menangani input yang tidak valid agar tidak menghasilkan perhitungan yang salah?
6. Bagaimana memeriksa beberapa komponen secara berulang sampai pengguna memilih untuk mengakhiri proses?

## 2. Tujuan dan Pengguna Program

### 2.1 Tujuan Program

Tujuan pembuatan Modul A:

1. Membantu pengguna memeriksa anggaran setiap komponen kegiatan mahasiswa.
2. Menghitung selisih antara anggaran rencana dan realisasi pengeluaran.
3. Menghitung persentase penyimpangan anggaran.
4. Menentukan status anggaran berdasarkan hasil pemeriksaan.
5. Memberikan keterangan tambahan jika terjadi kelebihan anggaran.
6. Memvalidasi input agar data yang tidak sesuai ketentuan tidak diproses.

### 2.2 Pengguna Program

Program ini ditujukan kepada bendahara, panitia kegiatan, atau pihak lain yang bertanggung jawab memeriksa penggunaan anggaran kegiatan mahasiswa.

Program dijalankan melalui terminal atau console dan digunakan dengan memasukkan data setiap komponen secara langsung.

## 3. Ketentuan dan Batasan Program

### 3.1 Ketentuan Program

Ketentuan yang digunakan dalam Modul A adalah:

1. Jika realisasi pengeluaran < anggaran rencana, statusnya adalah **Hemat**.
2. Jika realisasi pengeluaran = anggaran rencana, statusnya adalah **Tepat**.
3. Jika realisasi pengeluaran > anggaran rencana, statusnya adalah **Melebihi Anggaran**.
4. Jika kelebihan anggaran tidak lebih dari 10% dari anggaran rencana, keterangannya adalah **Perlu Evaluasi**.
5. Jika kelebihan anggaran lebih dari 10% dari anggaran rencana, keterangannya adalah **Peringatan**.
6. Anggaran rencana dan realisasi pengeluaran tidak boleh bernilai negatif.
7. Program memproses beberapa komponen menggunakan perulangan.
8. Pengguna dapat memilih untuk memeriksa komponen berikutnya atau mengakhiri proses.

### 3.2 Batasan Program

Batasan dalam pembuatan Modul A:

1. Program dijalankan melalui terminal atau console.
2. Bahasa pemrograman yang digunakan yaitu C++. Kelompok menggunakan satu bahasa yang sama.
3. Program menggunakan variabel, tipe data, operator, percabangan, dan perulangan.
4. Program berfokus pada pemeriksaan anggaran setiap komponen, bukan rekapitulasi keseluruhan kegiatan.
5. Array, class dan object, database, GUI, framework, serta library eksternal tidak diwajibkan dalam pengerjaan dan tidak digunakan dalam program ini.
6. Program menampilkan hasil pemeriksaan secara terperinci untuk setiap komponen.

### 3.3 Asumsi Program

Untuk memperjelas proses perhitungan, digunakan asumsi berikut:

1. Anggaran rencana harus lebih besar dari nol agar dapat digunakan sebagai pembagi dalam perhitungan persentase penyimpangan.
2. Realisasi pengeluaran sebesar nol diperbolehkan selama nilainya tidak negatif.
3. Kelebihan anggaran tepat 10% termasuk kategori Perlu Evaluasi.
4. Keterangan Perlu Evaluasi atau Peringatan hanya diberikan ketika realisasi pengeluaran melebihi anggaran rencana.
5. Persentase penyimpangan dihitung berdasarkan anggaran rencana setiap komponen.
6. Nama komponen ditulis satu kata tanpa spasi (misalnya Konsumsi atau Sewa_Gedung).
7. Angka anggaran rencana dan realisasi pengeluaran ditulis tanpa titik atau koma pemisah ribuan.

## 4. Analisis Data Modul A

Analisis data digunakan untuk menentukan data yang dimasukkan, proses pengolahan, hasil yang ditampilkan, dan penanganan input tidak valid dalam pemeriksaan anggaran setiap komponen.

### 4.1 Input

Input yang dibutuhkan:

1. **Nama Komponen** adalah nama kebutuhan atau pengeluaran kegiatan mahasiswa yang ditulis satu kata, misalnya konsumsi, dekorasi, perlengkapan, dll.
2. **Anggaran Rencana** adalah jumlah dana yang direncanakan untuk komponen.
3. **Realisasi Pengeluaran** adalah jumlah dana yang dikeluarkan untuk komponen.
4. **Pilihan Lanjut atau Selesai** adalah pilihan pengguna untuk memasukkan komponen berikutnya atau mengakhiri proses pemeriksaan.

### 4.2 Process

Program melakukan proses berikut:

1. Pengguna memasukkan nama komponen.
2. Pengguna memasukkan anggaran rencana.
3. Pengguna memasukkan realisasi pengeluaran.
4. Memeriksa validitas data segera setelah dimasukkan; jika tidak valid, program meminta input ulang sebelum lanjut ke langkah berikutnya.
5. Menghitung selisih antara realisasi pengeluaran dan anggaran rencana.
6. Menghitung persentase penyimpangan berdasarkan anggaran rencana.
7. Menentukan status anggaran berdasarkan perbandingan kedua nilai.
8. Menentukan keterangan tambahan jika realisasi pengeluaran melebihi anggaran.
9. Menampilkan hasil pemeriksaan komponen.
10. Menanyakan apakah pengguna ingin memeriksa komponen berikutnya atau mengakhiri proses.

**Rumus selisih anggaran:**

Selisih = Realisasi Pengeluaran - Anggaran Rencana

**Rumus persentase penyimpangan:**

Persentase Penyimpangan = (Selisih / Anggaran Rencana) x 100%

Hasil persentase dapat bernilai negatif jika pengeluaran lebih kecil daripada anggaran, nol jika pengeluaran sama dengan anggaran, dan positif jika pengeluaran melebihi anggaran.

### 4.3 Ketentuan Penentuan Status

Status anggaran ditentukan berdasarkan hasil perbandingan realisasi pengeluaran dan anggaran rencana.

| Kondisi | Status | Keterangan |
|---|---|---|
| Realisasi lebih kecil daripada anggaran | Hemat | Tidak ada kelebihan anggaran |
| Realisasi sama dengan anggaran | Tepat | Pengeluaran sesuai rencana |
| Realisasi lebih besar daripada anggaran | Melebihi Anggaran | Perlu diperiksa berdasarkan persentase kelebihan |

Untuk komponen dengan status Melebihi Anggaran, keterangan ditentukan sebagai berikut:

| Persentase Kelebihan Anggaran | Keterangan |
|---|---|
| Tidak lebih dari 10% | Perlu Evaluasi |
| Lebih dari 10% | Peringatan |

Persentase kelebihan anggaran untuk menentukan keterangan dihitung dari selisih positif dibandingkan dengan anggaran rencana. Dengan demikian, kelebihan anggaran tepat 10% masuk kategori Perlu Evaluasi.

### 4.4 Output

Hasil pemeriksaan yang ditampilkan untuk setiap komponen adalah:

1. Nama komponen.
2. Anggaran rencana.
3. Realisasi pengeluaran.
4. Selisih anggaran.
5. Persentase penyimpangan.
6. Status anggaran.
7. Keterangan tambahan jika terjadi kelebihan anggaran (ditampilkan tanda "-" jika tidak ada kelebihan).

### 4.5 Penanganan Input Tidak Valid

Program perlu memeriksa input sebelum melakukan perhitungan. Ketentuan penanganannya adalah:

1. Anggaran rencana harus berupa angka yang lebih besar dari nol.
2. Realisasi pengeluaran harus berupa angka yang tidak negatif, dan nilai nol diperbolehkan.
3. Pilihan untuk melanjutkan atau mengakhiri proses harus berupa y atau t.

Jika input tidak valid, program menampilkan pesan kesalahan dan meminta pengguna memasukkan data yang benar sebelum melanjutkan pemeriksaan. Program tidak berhenti secara tidak wajar ketika menerima input yang salah, termasuk ketika yang dimasukkan berupa huruf pada kolom angka.

## 5. Tabel Input-Process-Output (IPO)

| Input | Process | Output |
|---|---|---|
| Nama komponen | Menerima nama komponen yang ditulis satu kata | Nama komponen |
| Anggaran rencana | Memeriksa apakah nilai berupa angka dan lebih besar dari nol | Anggaran rencana yang valid |
| Realisasi pengeluaran | Memeriksa apakah nilai berupa angka dan tidak negatif | Realisasi pengeluaran yang valid |
| Input tidak valid | Menolak data dan meminta pengguna memasukkan ulang | Pesan kesalahan dan permintaan input ulang |
| Anggaran rencana dan realisasi pengeluaran | Menghitung selisih pengeluaran | Selisih anggaran |
| Selisih dan anggaran rencana | Menghitung persentase penyimpangan | Persentase penyimpangan |
| Anggaran rencana dan realisasi pengeluaran | Membandingkan kedua nilai menggunakan percabangan | Status Hemat, Tepat, atau Melebihi Anggaran |
| Persentase kelebihan anggaran | Memeriksa apakah kelebihan tidak lebih dari 10% atau lebih dari 10% | Keterangan Perlu Evaluasi atau Peringatan |
| Pilihan pengguna | Memeriksa apakah pilihan berupa y atau t, lalu menentukan proses berulang atau selesai | Proses berulang atau selesai |

## 6. Tabel Variabel dan Tipe Data

| No. | Nama Variabel | Tipe Data | Nilai Awal | Kegunaan |
|---|---|---|---|---|
| 1 | `namaKomponen` | String | Kosong | Menyimpan nama komponen kegiatan |
| 2 | `anggaranRencana` | Double | 0 | Menyimpan jumlah anggaran yang direncanakan |
| 3 | `realisasi` | Double | 0 | Menyimpan jumlah pengeluaran sebenarnya |
| 4 | `selisih` | Double | 0 | Menyimpan hasil pengurangan realisasi dengan anggaran rencana |
| 5 | `persenPenyimpangan` | Double | 0 | Menyimpan persentase penyimpangan anggaran |
| 6 | `status` | String | Kosong | Menyimpan status anggaran |
| 7 | `keterangan` | String | Kosong | Menyimpan keterangan tambahan jika terjadi kelebihan anggaran |
| 8 | `pilihan` | String | Kosong | Menyimpan pilihan pengguna (y atau t) untuk melanjutkan atau mengakhiri proses |