---
layout: post
title: "Menganalisis Faktor-Faktor yang Memengaruhi Hasil Akademik Siswa (SSC dan HSC)"
date: "2026-04-15"
language: "ID"
---

Halo semua, kali ini saya akan menganalisis dataset "Student Performance Dataset" yang dapat anda lihat di [sini](https://www.kaggle.com/datasets/ihasan88/student-performance-dataset). Dataset tersebut berisi 1000 data siswa-siswi di Bangladesh dengan variabel-variabel terkait sejumlah 14 kolom. Dari dataset berikut diharapkan dapat ditemukan keterkaitan antara satu variabel dengan variabel lainnya yang dapat mempengaruhi hasil akademik dari siswa dan siswi di Bangladesh. Terdapat dua kelompok variabel dalam data yang saya gunakan.

### Variable Numerik

Variabel numerik adalah variabel yang memiliki nilai berupa angka dan dapat dilakukan operasi matematis. Disini ditemukan 8 variabel yang dapat dikategorikan sebagai variabel numerik seperti yang ada pada tabel berikut:

| Variabel             | Deskripsi                       |
| -------------------- | ------------------------------- |
| Student_ID           | ID unik untuk setiap siswa      |
| Age                  | Usia siswa (tahun)              |
| Study_Hours_per_Week | Jumlah jam belajar per minggu   |
| Attendance           | Persentase kehadiran siswa (%)  |
| Family_Income_BDT    | Pendapatan keluarga (dalam BDT) |
| Previous_GPA         | Nilai GPA sebelumnya            |
| SSC_Result           | Nilai ujian SSC                 |
| HSC_Result           | Nilai ujian HSC                 |

### Variabel Kategorikal

Variabel numerik adalah variabel yang berisi kategori atau tabel tertentu. Disini terdapat 6 variabel yang dapat dikategorikan sebagai variabel numerik seperti yang ada pada tabel berikut:

| Variabel         | Deskripsi                       | Contoh Nilai                 |
| ---------------- | ------------------------------- | ---------------------------- |
| Gender           | Jenis kelamin siswa             | Male, Female                 |
| District         | Wilayah tempat tinggal siswa    | Rangpur, Dhaka, dll          |
| School_Type      | Jenis sekolah                   | Private, Public              |
| Parent_Education | Tingkat pendidikan orang tua    | Graduate, Undergraduate, dll |
| Internet_Access  | Akses internet di rumah         | Yes, No                      |
| Private_Tuition  | Mengikuti les privat atau tidak | Yes, No                      |

## Statistik Dasar

Disini statistik dasar dari dataset utamanya variabel numerik akan diuraikan satu demi satu.

### Jam Belajar Per Minggu

**🔢 Ukuran Pemusatan**

- Rata-rata (mean) nilai HSC: 17,102
- Median nilai HSC: 17
- Nilai mean yang sangat dekat dengan median menunjukkan bahwa distribusi data cenderung simetris.

**📉 Ukuran Penyebaran**

- Standar deviasi: 7,295
- Hal ini menunjukkan bahwa terdapat variasi nilai yang cukup besar antar siswa, sehingga nilai tidak terlalu terpusat di sekitar rata-rata.

**📌 Nilai Ekstrem**

- Nilai minimum: 5
- Nilai maksimum: 29
- Rentang nilai yang cukup lebar (24 poin) mengindikasikan adanya perbedaan performa yang signifikan antar siswa.

### Kehadiran

**🔢 Ukuran Pemusatan**

- Rata-rata kehadiran: 79,40%
- Median kehadiran: 79%
- Nilai mean yang sangat dekat dengan median menunjukkan bahwa distribusi data cenderung simetris.

**📉 Ukuran Penyebaran**

- Standar deviasi: 11,48
- Hal ini menunjukkan bahwa terdapat variasi kehadiran yang cukup besar antar siswa, sehingga data tidak terlalu terpusat di sekitar rata-rata.

**📌 Nilai Ekstrem**

- Nilai minimum: 60%
- Nilai maksimum: 99%
- Rentang nilai yang cukup lebar (39 poin persentase) mengindikasikan adanya perbedaan tingkat kehadiran yang signifikan antar siswa.

### Pendapatan Keluarga (BDT)

**🔢 Ukuran Pemusatan**

- Rata-rata pendapatan: 34.888 BDT
- Median pendapatan: 34.847 BDT
- Nilai mean yang sangat dekat dengan median menunjukkan bahwa distribusi pendapatan cenderung simetris, tanpa kemencengan yang signifikan.

**📉 Ukuran Penyebaran**

- Standar deviasi: 14.523 BDT
- Hal ini menunjukkan bahwa terdapat variasi pendapatan yang cukup besar antar keluarga siswa, sehingga data tidak terlalu terpusat di sekitar rata-rata.

**📌 Nilai Ekstrem**

- Pendapatan minimum: 10.016 BDT
- Pendapatan maksimum: 59.767 BDT
- Rentang pendapatan yang cukup lebar (49.751 BDT) mengindikasikan adanya kesenjangan ekonomi yang signifikan antar keluarga siswa.

### GPA (Grade Point Average)

**🔢 Ukuran Pemusatan**

- Rata-rata GPA: 3,99
- Median GPA: 4,0
- Nilai mean yang sangat dekat dengan median menunjukkan bahwa distribusi GPA cenderung simetris, tanpa kemencengan yang signifikan.

**📉 Ukuran Penyebaran**

- Standar deviasi: 0,58
- Hal ini menunjukkan bahwa terdapat variasi nilai GPA yang kecil hingga moderat, sehingga sebagian besar nilai relatif terkonsentrasi di sekitar rata-rata.

**📌 Nilai Ekstrem**

- GPA minimum: 3,0
- GPA maksimum: 5,0
- Rentang nilai (2,0 poin) menunjukkan adanya perbedaan tingkat prestasi akademik, namun masih dalam batas skala penilaian yang wajar.

### SSC (Secondary School Certificate)

**🔢 Ukuran Pemusatan**

- Rata-rata nilai SSC: 4,25
- Median nilai SSC: 4,26
- Nilai mean yang sangat dekat dengan median menunjukkan bahwa distribusi nilai SSC cenderung simetris, tanpa kemencengan yang signifikan.

**📉 Ukuran Penyebaran**

- Standar deviasi: 0,42
- Hal ini menunjukkan bahwa terdapat variasi nilai yang kecil, sehingga sebagian besar nilai relatif terkonsentrasi di sekitar rata-rata.

**📌 Nilai Ekstrem**

- Nilai minimum: 3,5
- Nilai maksimum: 5,0
- Rentang nilai (1,5 poin) menunjukkan adanya perbedaan tingkat prestasi akademik, namun masih dalam batas skala penilaian yang wajar.

### HSC (Higher Secondary Certificate)

**🔢 Ukuran Pemusatan**

- Rata-rata nilai HSC: 4,01
- Median nilai HSC: 4,01
- Nilai mean yang sama dengan median menunjukkan bahwa distribusi nilai HSC sangat simetris, tanpa kemencengan yang signifikan.

**📉 Ukuran Penyebaran**

- Standar deviasi: 0,58
- Hal ini menunjukkan bahwa terdapat variasi nilai yang kecil hingga moderat, sehingga sebagian besar nilai relatif terkonsentrasi di sekitar rata-rata.

**📌 Nilai Ekstrem**

- Nilai minimum: 3,0
- Nilai maksimum: 5,0
- Rentang nilai (2,0 poin) menunjukkan adanya perbedaan tingkat prestasi akademik, namun masih dalam batas skala penilaian yang wajar.
