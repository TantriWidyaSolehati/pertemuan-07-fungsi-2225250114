# Pertemuan 07 Fungsi Python
- Nama: Tantri Widya Solehati
- NIM: 2225250114
- Kelas: 3F
## Tujuan
Menggunakan fungsi, parameter, return value, dan scope untuk membuat program modular.
## Cara Menjalankan
python3 praktik/utilitas_matematika.py
## Struktur Fungsi
1. Fungsi luas_persegi_panjang(p, l) memiliki dua parameter yaitu p (panjang) dan l (lebar). Fungsi ini mengembalikan nilai hasil perkalian antara panjang dan lebar, sehingga return-nya adalah luas persegi panjang.
2. Fungsi luas_segitiga(a, t) menerima dua parameter yaitu a (alas) dan t (tinggi). Nilai yang dikembalikan adalah hasil perhitungan rumus luas segitiga, yaitu 0.5 * a * t.
3. Fungsi jumlah_n(n) memiliki satu parameter n. Di dalamnya terdapat perulangan untuk menjumlahkan semua bilangan dari 1 sampai n. Nilai yang dikembalikan adalah total, yaitu hasil penjumlahan tersebut.
4. Fungsi faktorial(n) juga memiliki satu parameter n. Fungsi ini menggunakan perulangan untuk menghitung perkalian berurutan dari 1 hingga n. Nilai yang dikembalikan adalah hasil, yaitu nilai faktorial dari n.
5. Fungsi tampilkan_menu() tidak memiliki parameter dan tidak mengembalikan nilai. Fungsinya hanya menampilkan daftar pilihan menu ke layar menggunakan perintah print.
## Hasil Pengujian
| Operasi             | Input    | Hasil yang diharapkan | Hasil Aktual | Status |
|---------------------|----------|-----------------------|--------------|--------|
|Luas persegi panjang | p=8, l=5 | 40                    | 40           | Sesuai |
| Luas segitiga       | a=10, t=6| 30                    | 30           | Sesuai |
| Jumlah 1..n         | n=10     | 55                    | 55           | Sesuai |
| Faktorial           | n=5      | 120                   | 120          | Sesuai |
|Faktorial            | n=0      | 1                     | 1            | Sesuai |
## Refleksi
Bagian program yang menjadi lebih sederhana setelah dipisah menjadi fungsi adalah perhitungan faktorial.
Jika logika faktorial ditulis langsung di dalam blok if, kode akan panjang dan sulit dibaca. Dengan memisahkannya ke fungsi faktorial(n), kita cukup memanggil:

```python
print("Faktorial =", faktorial(n))
```

Tanpa harus menulis ulang loop perkalian setiap kali dibutuhkan.
Hasilnya: kode lebih rapi, mudah diuji, dan bisa dipakai ulang di bagian lain program.