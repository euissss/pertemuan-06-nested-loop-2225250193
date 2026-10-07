# Pertemuan 06 Nested Loop Python

Nama: Euis Hasanah Ramadani
NIM: 2225250193
Kelas: 3F

## Tujuan

Menggunakan nested loop, pola, akumulasi, dan pencacahan dalam Python.

## Struktur Program

Program terdiri dari empat latihan dan satu tugas utama, yaitu:

1. `01_pasangan_indeks.py`
2. `02_pola_segitiga.py`
3. `03_jumlah_per_baris.py`
4. `04_hitung_pasangan.py`
5. `tabel_perkalian_dan_statistik.py`

## Cara Menjalankan

Program dijalankan melalui terminal VS Code menggunakan perintah:

```bash
python3 latihan/01_pasangan_indeks.py
python3 latihan/02_pola_segitiga.py
python3 latihan/03_jumlah_per_baris.py
python3 latihan/04_hitung_pasangan.py
python3 tugas/tabel_perkalian_dan_statistik.py
```

## Algoritma Tugas 3

Program membaca nilai `n` sebagai bilangan bulat positif. Jika nilai `n` kurang dari atau sama dengan nol, program meminta input kembali sampai mendapatkan nilai positif.

Setelah nilai `n valid`, program menggunakan nested loop. Loop luar menggunakan variabel `i` untuk menentukan baris, sedangkan loop dalam menggunakan variabel `j` untuk menentukan kolom. Pada setiap pasangan `i` dan `j`, program menghitung `hasil = i * j`.

Variabel `total_baris` digunakan untuk menghitung jumlah hasil perkalian pada setiap baris. Variabel tersebut direset pada awal setiap iterasi loop luar. Sementara itu, `total_semua` digunakan untuk menghitung jumlah seluruh hasil perkalian dan `count_genap` digunakan untuk menghitung banyak hasil perkalian yang bernilai genap.

## Hasil Pengujian

| Test Case | Total Seluruh Hasil | Banyak Hasil Genap |
| --------- | ------------------: | -----------------: |
| n = 1     |                   1 |                  0 |
| n = 2     |                   9 |                  3 |
| n = 3     |                  36 |                  5 |

Semua hasil pengujian sesuai dengan hasil yang diharapkan.

## Analisis Efisiensi

Untuk input `n`, loop dalam dijalankan sebanyak `n` kali untuk setiap iterasi loop luar. Oleh karena itu, jumlah eksekusi badan loop dalam adalah `n × n` atau `n²`.

## Refleksi

Pada nested loop, lokasi inisialisasi akumulator sangat penting. `total_baris` harus direset pada setiap awal baris karena digunakan untuk menghitung jumlah pada satu baris. Sebaliknya, `total_semua` tidak boleh direset di dalam loop karena digunakan untuk menghitung seluruh hasil perkalian.

Kesalahan lain yang perlu diperhatikan adalah indentasi. Loop dalam harus berada di dalam loop luar, sedangkan perintah untuk menampilkan jumlah keseluruhan harus berada setelah kedua loop selesai.
