# Algoritma
## Definisi
Algoritma adalah serangkaian instruksi atau langkah-langkah yang jelas dan terperinci untuk menyelesaikan masalah atau menjalankan tugas tertentu. Algoritma dapat diimplementasikan dalam berbagai bahasa pemrograman untuk memecahkan masalah komputasi. Contoh sederhana dari algoritma adalah resep masakan, di mana terdapat langkah-langkah berurutan untuk mencapai hasil akhir.

## Algoritma Sequential Search
Algoritma Sequential Search adalah metode pencarian yang memeriksa setiap elemen dalam daftar satu per satu sampai elemen yang dicari ditemukan atau daftar berakhir. Ini adalah metode pencarian paling sederhana tetapi kurang efisien untuk daftar yang sangat besar.

Contoh Algoritma Sequential Search: Misalkan kita memiliki daftar [5, 3, 8, 4, 2] dan kita mencari elemen 4:
| Index | Elemen | Target | Keterangan             |
|-------|--------|--------|------------------------|
| 0     | 5      | 4      | Tidak cocok            |
| 1     | 3      | 4      | Tidak cocok            |
| 2     | 8      | 4      | Tidak cocok            |
| 3     | 4      | 4      | Cocok, kembalikan index|
| 4     | 2      | 4      | (Tidak dicapai)        |

Contoh kode python:
```python=
def sequentialSearch(arr, target):
    for i in range(len(arr)):
        if arr[i] == target:
            return i
    return -1

# Contoh penggunaan
arr = [5, 3, 8, 4, 2]
target = 4
print(sequentialSearch(arr, target))  # Output: 3

```



## Pseudocode
Pseudocode adalah cara menulis algoritma dengan menggunakan bahasa yang mirip dengan bahasa manusia, namun tetap menggambarkan logika pemrograman. Pseudocode tidak mengikuti aturan sintaksis bahasa pemrograman tertentu, sehingga lebih mudah dipahami oleh siapa saja, baik yang berpengalaman maupun pemula. Pseudocode berfungsi sebagai panduan sebelum menulis kode nyata.

## Algoritma Binary Search
Algoritma Binary Search adalah metode pencarian yang efisien pada daftar yang sudah diurutkan. Algoritma ini membagi daftar menjadi dua bagian, membandingkan elemen tengah dengan target, dan mengulangi proses pada setengah bagian yang relevan. Binary Search lebih cepat dibandingkan Sequential Search untuk daftar yang besar.

Contoh Algoritma Binary Search: Misalkan kita memiliki daftar [2, 3, 4, 5, 8] yang sudah diurutkan, dan kita mencari elemen 4:
| Iterasi | Left | Right | Mid | Elemen Tengah | Target | Keterangan                       |
|---------|------|-------|-----|---------------|--------|----------------------------------|
| 1       | 0    | 4     | 2   | 4             | 4      | Cocok, kembalikan index           |

Contoh kode python:
```python=
def binarySearch(arr, target):
    left, right = 0, len(arr) - 1
    while left <= right:
        mid = (left + right) // 2
        print(f"Iterasi: {arr[left:right+1]}, Left: {left}, Right: {right}, Mid: {mid}, Elemen Tengah: {arr[mid]}")
        if arr[mid] == target:
            return mid
        elif arr[mid] < target:
            left = mid + 1
        else:
            right = mid - 1
    return -1

# Contoh penggunaan
arr = [2, 3, 4, 5, 8]
target = 4
index = binarySearch(arr, target)
print(f"Index dari target {target} adalah {index}")

```
## Big O Algoritma
Big O Notation adalah cara untuk mengukur kompleksitas waktu atau ruang dari sebuah algoritma dalam hal ukuran input. Ini memberikan gambaran seberapa cepat atau lambat algoritma tumbuh seiring dengan peningkatan ukuran input.

Tabel Big O Notation:
| Algoritma             | Kompleksitas Waktu | Kompleksitas Ruang |
|-----------------------|--------------------|--------------------|
| Sequential Search     | $O(n)$             | $O(1)$             |
| Binary Search         | $O(\log n)$        | $O(1)$             |
| Bubble Sort           | $O(n^2)$           | $O(1)$             |
| Merge Sort            | $O(n \log n)$      | $O(n)$             |
| Quick Sort            | $O(n \log n)$      | $O(\log n)$        |

## Hitung Big O dari Algoritma Sequential Search
Algoritma Sequential Search memiliki kompleksitas waktu $O(n)$ karena dalam kasus terburuk, setiap elemen dalam daftar harus diperiksa sekali. Kompleksitas ruangnya adalah $O(1)$ karena tidak membutuhkan ruang tambahan yang bergantung pada ukuran input.

Contoh Penghitungan Big O: Misalkan kita memiliki daftar dengan 10 elemen dan mencari elemen yang berada di posisi terakhir:
| Iterasi | Elemen     | Target | Keterangan     |
|---------|------------|--------|----------------|
| 1       | 5          | 8      | Tidak cocok    |
| 2       | 3          | 8      | Tidak cocok    |
| 3       | 1          | 8      | Tidak cocok    |
| 4       | 4          | 8      | Tidak cocok    |
| 5       | 6          | 8      | Tidak cocok    |
| 6       | 7          | 8      | Tidak cocok    |
| 7       | 2          | 8      | Tidak cocok    |
| 8       | 9          | 8      | Tidak cocok    |
| 9       | 0          | 8      | Tidak cocok    |
| 10      | 8          | 8      | Cocok, selesai |

Contoh kode python:
```python=
def sequentialSearch(arr, target):
    for i in range(len(arr)):
        print(f"Iterasi: {i + 1}, Elemen: {arr[i]}, Target: {target}, Keterangan: {'Cocok, selesai' if arr[i] == target else 'Tidak cocok'}")
        if arr[i] == target:
            return i
    return -1

# Contoh penggunaan
arr = [5, 3, 1, 4, 6, 7, 2, 9, 0, 8]
target = 8
index = sequentialSearch(arr, target)
print(f"Index dari target {target} adalah {index}")

```
Jumlah total perbandingan dalam kasus terburuk adalah 10, sehingga kompleksitas waktunya adalah $O(n)$ dan kompleksitas ruangnya adalah $O(1)$.

## Referensi
Referensi:

Algoritma: Pengertian, Sejarah, Jenis, Fungsi, dan Contohnya. (n.d.). Gramedia Literasi Matematika. Diakses pada 7 Oktober 2024 dari https://www.gramedia.com/literasi/pengertian-algoritma/.

Algoritma: Definisi, Ciri, Jenis, Struktur dan Contohnya. (2021). Tirto.ID. Diakses pada 7 Oktober 2024 dari https://tirto.id/algoritma-definisi-ciri-jenis-struktur-dan-contohnya-gjgn.

Algoritma dan Pemrograman: Buku Bahan Ajar. (2021). Google Books. Diakses pada 7 Oktober 2024 dari https://books.google.com/books?id=2UpEEAAAQBAJ.

Open Library - Buku Algoritma Dan Pemrograman. (n.d.). Telkom University. Diakses pada 7 Oktober 2024 dari https://openlibrary.telkomuniversity.ac.id/home/catalog/id/165210/slug/buku-algoritma-dan-pemrograman.html.