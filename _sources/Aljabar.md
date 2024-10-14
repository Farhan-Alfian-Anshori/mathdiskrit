# Aljabar Boolean dan Gerbang Logika
## Aljabar Boolean
Pengertian Aljabar Boolean: Aljabar Boolean adalah cabang matematika yang berkaitan dengan operasi logika dan variabel biner. Variabel biner ini hanya memiliki dua nilai, yaitu 1 (benar) dan 0 (salah). Aljabar Boolean digunakan untuk menyederhanakan dan menganalisis rangkaian logika.

## Tujuan
Tujuan utama Aljabar Boolean adalah untuk menyediakan metode matematika dalam mendesain dan menganalisis sirkuit digital. Hal ini memungkinkan insinyur untuk menyederhanakan fungsi logika dan meminimalkan penggunaan gerbang logika dalam rangkaian elektronik.

## Operator Biner & Uner:

### Operator Biner:

AND ($\cdot$ atau ∗): Menghasilkan 1 jika kedua operannya 1. $$A \cdot B = C$$

Contoh:
|$A$|$B$|$A \cdot B$|
|---|---|-----------|
| 0 | 0 |    0      |
| 0 | 1 |    0      |
| 1 | 0 |    0      |
| 1 | 1 |    1      |



OR (+): Menghasilkan 1 jika salah satu atau kedua operannya 1. $$A + B = C$$

Contoh:
|$A$|$B$|$A + B$ |
|---|---|--------|
| 0 | 0 |   0    |
| 0 | 1 |   1    |
| 1 | 0 |   1    |
| 1 | 1 |   1    |


XOR ($\oplus$): Menghasilkan 1 jika kedua operan berbeda. $$A \oplus B = C$$

Contoh:
| $A$ |$B$ | $A \oplus B$ |
|-----|----|--------------|
| 0   | 0  |   0          |
| 0   | 1  |   1          |
| 1   | 0  |   1          |
| 1   | 1  |   0          |


### Operator Uner:

NOT ($\overline{A}$ atau $\neg A$): Menghasilkan kebalikan dari nilai operan. $$\overline{A} = A'$$

Contoh: 
| $A$ | $\overline{A}$ |
|-----|----------------|
| 0   |      1         |
| 1   |      0         |



## Manfaat
Aljabar Boolean sangat berguna dalam pemrograman, terutama dalam pengambilan keputusan dan pernyataan kondisional. Contoh penggunaan termasuk:

-Mengontrol alur program dengan pernyataan if-else.

-Meningkatkan efisiensi kode dengan menyederhanakan ekspresi logika.

-Memvalidasi kondisi tertentu dalam algoritma pencarian dan pengurutan.

## Gerbang Logika (Logic Gates)
Gerbang logika adalah blok dasar dari rangkaian digital yang melakukan operasi logika pada satu atau lebih sinyal input biner dan menghasilkan sinyal output biner. Gerbang logika digunakan untuk membangun sirkuit digital yang dapat melakukan berbagai fungsi komputasi.

## Jenis-Jenis Logic Gates:

Gerbang AND: Menghasilkan output 1 hanya jika semua inputnya 1.
| $A$ | $B$ | $A \cdot B$ |
|-----|-----|-------------|
| 0   | 0   |    0        |
| 0   | 1   |    0        |
| 1   | 0   |    0        |
| 1   | 1   |    1        |


Gerbang OR: Menghasilkan output 1 jika salah satu atau semua inputnya 1.
|$A$|$B$|$A + B$ |
|---|---|--------|
| 0 | 0 |   0    |
| 0 | 1 |   1    |
| 1 | 0 |   1    |
| 1 | 1 |   1    |


Gerbang NOT:
| $A$ | $\overline{A}$ |
|-----|--------------  |
| 0   |      1         |
| 1   |      0         |



Gerbang NAND: Menghasilkan output 0 hanya jika semua inputnya 1.
| $A$ | $B$ | $\overline{A \cdot B}$ |
|-----|-----|------------------------|
| 0   | 0   |          1             |
| 0   | 1   |          1             |
| 1   | 0   |          1             |
| 1   | 1   |          0             |



Gerbang NOR: Menghasilkan output 0 jika salah satu atau semua inputnya 1.
| $A$ | $B$ | $\overline{A + B}$ |
|-----|-----|--------------------|
| 0   | 0   |        1           |
| 0   | 1   |        0           |
| 1   | 0   |        0           |
| 1   | 1   |        0           |



Gerbang XOR: Menghasilkan output 1 jika inputnya berbeda. 
| $A$ | $B$ | $A \oplus B$ |
|-----|-----|--------------|
| 0   | 0   |     0        |
| 0   | 1   |     1        |
| 1   | 0   |     1        |
| 1   | 1   |     0        |


Gerbang XNOR: Menghasilkan output 1 jika inputnya sama. 
| $A$ | $B$ | $\overline{A \oplus B}$ |
|-----|-----|-------------------------|
| 0   | 0   |          1              |
| 0   | 1   |          0              |
| 1   | 0   |          0              |
| 1   | 1   |          1              |


## Referensi
Aljabar Boolean - Pengertian, Hukum, dan Contoh Soal1
. (2019). Webstudi. Diakses pada 14 Oktober 2024 dari https://www.webstudi.site/2019/02/aljabar-boolean.html1
.

Gerbang Logika: Pengertian, Jenis dan Simbolnya1
. (n.d.). Teknik Elektronik. Diakses pada 14 Oktober 2024 dari https://teknikece.com/gerbang-logika/1
.

Pengertian Gerbang Logika: Fondasi Sistem Digital Modern1
. (n.d.). Wiki Elektronika. Diakses pada 14 Oktober 2024 dari https://wikielektronika.com/pengertian-gerbang-logika/1
.