# Tugas Pengolahan Citra Digital

## Deskripsi
Repositori ini berisi tugas mata kuliah Pengolahan Citra Digital menggunakan bahasa pemrograman Python dan Google Colab.

Tugas ini bertujuan untuk mempelajari cara mengolah gambar digital dengan mengubah foto berwarna menjadi gambar grayscale (keabuan). Melalui praktik ini, kita dapat memahami bahwa gambar digital dapat diproses oleh komputer menggunakan program.

## Teknologi yang Digunakan
- **Python**: Bahasa pemrograman yang digunakan untuk mengolah gambar.
- **Google Colab**: Platform online untuk menulis dan menjalankan kode Python.
- **Pillow (PIL)**: Library untuk membuka, mengolah, dan menyimpan gambar.
- **Matplotlib**: Library untuk menampilkan dan membandingkan gambar.

## Metode Pengolahan Citra: Grayscale
Grayscale adalah metode pengolahan citra yang mengubah gambar berwarna menjadi gambar dengan tingkat keabuan.

Gambar berwarna memiliki beberapa komponen warna, seperti merah (Red), hijau (Green), dan biru (Blue). Dengan metode grayscale, gambar diubah menjadi representasi satu tingkat intensitas keabuan untuk setiap piksel.

Nilai intensitas grayscale berkisar dari:
- **0**: Hitam.
- **255**: Putih.
- **1–254**: Berbagai tingkat keabuan.

## Penjelasan Kode Program

### 1. Mengimpor Library
```python
from PIL import Image
import matplotlib.pyplot as plt
```
Kode ini mengimpor library yang digunakan. `PIL` berfungsi untuk membuka dan mengolah gambar, sedangkan `matplotlib.pyplot` digunakan untuk menampilkan gambar.

### 2. Membuka Foto
```python
foto = Image.open("foto.jpg")
```
Kode ini digunakan untuk membuka gambar bernama `foto.jpg`. File gambar harus tersedia di lokasi yang dapat diakses oleh program.

### 3. Mengubah Foto Menjadi Grayscale
```python
foto_gray = foto.convert("L")
```
Kode ini mengubah foto berwarna menjadi grayscale. Mode `"L"` menunjukkan bahwa gambar menggunakan tingkat kecerahan keabuan dengan nilai intensitas 0–255.

### 4. Menampilkan Foto Asli dan Grayscale
```python
plt.figure(figsize=(10, 5))

plt.subplot(1, 2, 1)
plt.imshow(foto)
plt.title("Foto Asli")
plt.axis("off")

plt.subplot(1, 2, 2)
plt.imshow(foto_gray, cmap="gray")
plt.title("Foto Grayscale")
plt.axis("off")

plt.show()
```
Bagian ini digunakan untuk menampilkan dua gambar secara berdampingan, yaitu foto asli dan foto yang sudah diubah menjadi grayscale.

- `plt.figure(figsize=(10, 5))`: Mengatur ukuran tampilan gambar.
- `plt.subplot(1, 2, 1)`: Menyiapkan posisi gambar pertama.
- `plt.imshow(foto)`: Menampilkan foto asli.
- `plt.title("Foto Asli")`: Memberikan judul pada foto asli.
- `plt.axis("off")`: Menghilangkan sumbu pada tampilan gambar.
- `plt.subplot(1, 2, 2)`: Menyiapkan posisi gambar kedua.
- `plt.imshow(foto_gray, cmap="gray")`: Menampilkan hasil grayscale menggunakan warna keabuan.
- `plt.title("Foto Grayscale")`: Memberikan judul pada gambar grayscale.
- `plt.show()`: Menampilkan kedua gambar.

### 5. Menyimpan Hasil Grayscale
```python
foto_gray.save("foto_grayscale.png")
```
Kode ini menyimpan gambar hasil grayscale dengan nama `foto_grayscale.png`, sehingga hasil pengolahan dapat digunakan kembali.

### 6. Menampilkan Pesan
```python
print("Foto berhasil diubah menjadi grayscale!")
print("Hasil disimpan sebagai foto_grayscale.png")
```
Kode ini menampilkan pesan bahwa proses pengubahan gambar telah selesai dan hasilnya disimpan.

## Hasil Praktik
Program menghasilkan dua tampilan gambar, yaitu foto asli dan foto grayscale. Foto grayscale juga disimpan dalam format PNG dengan nama `foto_grayscale.png`.

Praktik ini menunjukkan bahwa gambar digital dapat dibaca, diubah, ditampilkan, dan disimpan kembali menggunakan program Python.

## Kesimpulan
Melalui tugas ini, saya mempelajari cara melakukan pengolahan citra digital menggunakan Python dengan library Pillow dan Matplotlib. Metode grayscale digunakan untuk mengubah foto berwarna menjadi gambar keabuan.

Pengolahan ini merupakan salah satu dasar dalam pemrosesan citra digital. Namun, kode yang digunakan belum menampilkan nilai numerik setiap piksel secara langsung, sehingga pembuktian bahwa citra digital tersusun dari angka masih dapat dikembangkan lebih lanjut.
