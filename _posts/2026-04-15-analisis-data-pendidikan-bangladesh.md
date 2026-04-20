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
