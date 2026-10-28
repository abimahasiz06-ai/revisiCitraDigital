# Tugas Pengolahan Citra Digital

## Deskripsi
Repositori ini berisi tugas mata kuliah Pengolahan Citra Digital yang dikerjakan menggunakan Python melalui Google Colab.

Tujuan tugas ini adalah membuktikan bahwa citra digital merupakan susunan angka yang direpresentasikan dalam bentuk piksel. Setiap piksel memiliki nilai numerik yang menentukan warna atau tingkat kecerahan pada gambar.

## Teknologi yang Digunakan
- **Python** — bahasa pemrograman untuk mengolah citra.
- **Google Colab** — lingkungan untuk menulis dan menjalankan kode Python secara online.
- **Pillow** — library untuk membaca dan memproses gambar.
- **NumPy** — library untuk merepresentasikan gambar sebagai array atau susunan angka.
- **Matplotlib** — library untuk menampilkan gambar dan hasil pengolahan citra.

## Metode Pengolahan Citra: Grayscale
Metode yang digunakan dalam tugas ini adalah *grayscale*, yaitu mengubah gambar berwarna menjadi gambar dengan tingkat keabuan.

Pada gambar berwarna, setiap piksel umumnya memiliki tiga komponen warna, yaitu Red (R), Green (G), dan Blue (B). Setelah diubah menjadi grayscale, setiap piksel direpresentasikan oleh satu nilai intensitas keabuan.

Rentang nilai intensitas tersebut adalah:
- **0** = hitam
- **255** = putih
- **1–254** = berbagai tingkat keabuan

## Tahapan Pengerjaan
1. Menyiapkan gambar sebagai citra masukan.
2. Membaca gambar menggunakan Python.
3. Mengubah gambar berwarna menjadi grayscale.
4. Menampilkan gambar asli dan hasil grayscale untuk dibandingkan.
5. Mengubah data gambar menjadi array menggunakan NumPy.
6. Menampilkan nilai numerik beberapa piksel untuk membuktikan bahwa citra digital tersusun dari angka.
7. Menyimpan hasil pengolahan citra.

## Struktur Repositori
- `Citra-digital.ipynb` — notebook Google Colab yang berisi kode program dan proses pengolahan citra.
- `pas foto.jpeg` — gambar yang digunakan sebagai citra masukan.

## Hasil dan Pembahasan
Melalui proses grayscale, gambar berwarna diubah menjadi gambar dengan tingkat keabuan. Data gambar juga dapat ditampilkan dalam bentuk array numerik menggunakan NumPy.

Hasil tersebut menunjukkan bahwa gambar digital tidak hanya berupa tampilan visual, tetapi juga memiliki representasi data berupa angka yang menyusun setiap pikselnya.

## Kesimpulan
Berdasarkan praktik yang dilakukan, citra digital dapat direpresentasikan sebagai susunan angka dalam bentuk array atau matriks piksel. Dengan menggunakan Python dan Google Colab, gambar dapat dibaca, diolah menjadi grayscale, dan ditampilkan nilai numerik pikselnya.

Praktik ini membantu memahami hubungan antara gambar yang terlihat oleh mata dan data numerik yang diproses oleh komputer.
