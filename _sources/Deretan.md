# Deretan dan Rekursi
## Deretan (sequence) 

- Deretan adalah suatu urutan atau susunan elemen atau objek yang disusun secara teratur berdasarkan suatu aturan tertentu. Elemen dalam deretan biasanya berupa angka, huruf, simbol, atau objek lainnya, dan urutannya dapat didasarkan pada pola, nilai, atau hubungan tertentu

- Definisi: Sebuah deretan adalah fungsi dari subset suatu himpunan bilangan bulat (biasanya N atau P) ke sebuah himpunan S.

N = {1, 2, 3, 4, … }
S misalnya {2, 4, 6, 8, …},   {1/3, 1/5, 1/7, …},  dsb

Notasi Deretan: {$a_n$}

- Deretan umumnya dinyatakan dalam suatu formula, misalnya:
$a_n = 2n$

$a_n = \frac{1}{n}$

$a_n = 7 - 3n$

Dalam konteks matematika, deretan sering merujuk pada barisan bilangan, yaitu kumpulan bilangan yang disusun dalam suatu pola tertentu.
 Misalnya:
1. Deretan bilangan ganjil: 1,3,5,7,…
2. Deretan bilangan genap: 2,4,6,8,…
3. Deretan bilangan yang membentuk deret aritmetika: 3,6,9,12....

___

-Contoh-contoh deretan dan formulanya:

- Deret Aritmetika
Deret dengan pola kenaikan atau penurunan tetap.
Contoh: 2,5,8,11,14,…
Rumus suku ke-n: $U_n = a + (n - 1) \cdot b$
Di mana:
-$a$: suku pertama
-$b$: beda (selisih antar suku)
-$n$: nomor suku yang dicari

- Deret Geometri
Deret dengan pola kelipatan tetap.
Contoh: 3,6,12,24,48,…
Rumus suku ke-n: $U_n = a \cdot r^{(n-1)}$
Di mana:
-$a$: suku pertama
-$r$: rasio (perbandingan antar suku,
-$n$: nomor suku yang dicari

- Deret Bilangan Kuadrat
Deret dengan pola nilai berupa kuadrat bilangan bulat.
Contoh: 1,4,9,16,25,…
Rumus suku ke-n: $𝑈_𝑛=𝑛^2$

- Deret Bilangan Kubik
Deret dengan pola nilai berupa kubik bilangan bulat.
Contoh: 1,8,27,64,125,…
Rumus suku ke-n: $𝑈_𝑛=𝑛^3$

- Deret Fibonanci
Deret dengan pola di mana setiap suku merupakan jumlah dua suku sebelumnya.
Contoh: 0,1,1,2,3,5,8,…
Rumus suku ke-n(rekursif): $𝐹_𝑛=𝐹_(𝑛−1)+𝐹_(𝑛−2),𝐹_0=0,𝐹_1=1$

___

- String
String adalah deretan berhingga karakter berbentuk
$a_1a_2a_3a_4…a_n$

Panjang string S adalah jumlah karakter di dalam string tersebut
     
Contoh:  informatika adalah string dengan panjang 11 karakter 10100101 adalah string biner dengan panjang 8 bit

String kosong dilambangkan dengan $\lambda$, panjangnya = 0

## Penjumlahan Deretan
Jumlah deretan 
$a_m, a_{m+1}, a_{m+2}, …, a_n$
adalah
$a_m + a_{m+1} + a_{m+2} + … + a_n$
atau dalam notasi sumasi:
$\sum_{k=m}^{n} a_k$ 
$k$ adalah indeks summasi, 
$m$ adalah batas bawah indeks,
$n$ adalah batas atas indeks

Contoh 2: Berapa nilai $\sum_{k=1}^{5} k^2$? 
Jawaban:
$\sum_{k=1}^{5} k^2 = 1^2 + 2^2 + 3^2 + 4^2 + 5^2 = 1 + 4 + 9 + 16 + 25 = 55$

___

Contoh 3:Batas bawah sumasi kadangkala perlu digeser agar dapat dijumlahkan dengan sumasi lain yang memiliki batas bawah berbeda.
Pada Contoh 2 di atas, batas bawah digeser dari 1 menjadi 0, akibatnya:
$\sum_{k=1}^{5} k^2 = \sum_{k=0}^{4} (k+1)^2$

Contoh 4:Sumasi dapat dipecah dengan membagi dua indeksnya, misalnya:
$\sum_{k=1}^{100} k^2$ = $\sum_{k=1}^{49} k^2$ +$ $\sum_{k=50}^{100} k^2$

___
- TUGAS PEMBUKTIAN Dari 3 rumus dibawah Beberapa sumasi sudah ditemukan rumus penjumlahannya sebagai berikut:

| Sum | Closed Form |
| -------- | -------- |
|  $\sum_{k=0}^{n} ar^k =\quad (r \neq 0)$     |$\frac{ar^{n+1} - a}{r - 1}, \quad r \neq 1$    |
|$\sum_{k=1}^{n} k$| $\frac{n(n+1)}{2}$|
|$\sum_{k=1}^{n} k^2$| $\frac{n(n+1)(2n+1)}{6}$
|$\sum_{k=1}^{n} k^3$| $\frac{n^2(n+1)}{4}^2$
|$\sum_{k=0}^{\infty} x^k$,/$x$\ $< 1$ | $\frac{1}{1-x}$
|$\sum_{k=1}^{\infty} kx^{k-1}$ ,/x\ <1 |$\frac{1}{(1-x)^2}$

### Pembuktian Rumus Deret Geometri:
**Langkah 1: Tulis deretnya**  
Mulai dengan bentuk deret geometri:

$$S_n = a + ar + ar^2 + \dots + ar^n$$

**Langkah 2: Kalikan $( S_n )$ dengan rasio $( r )$**  
Kalikan kedua sisi persamaan dengan $( r )$:

$$rS_n = ar + ar^2 + ar^3 + \dots + ar^{n+1}$$

**Langkah 3: Kurangi kedua persamaan**  
Kurangi $( S_n )$ dengan $( rS_n )$:

$$S_n - rS_n = (a + ar + ar^2 + \dots + ar^n) - (ar + ar^2 + \dots + ar^{n+1})$$

Semua suku di kanan akan saling menghilangkan, kecuali $( a )$ dan $( ar^{n+1} )$:

$$S_n (1 - r) = a - ar^{n+1}$$

**Langkah 4: Sederhanakan persamaan**  
Faktor $( S_n )$:

$$S_n = \frac{a(1 - r^{n+1})}{1 - r}, \quad \text{dengan \( r \neq 1 \)}.$$

---

### Hasil Akhir:
Rumus tertutup dari deret geometri adalah:
$$S_n = \frac{a(1 - r^{n+1})}{1 - r}, \quad \text{untuk \( r \neq 1 \)}.$$

Rumus ini sangat berguna dalam banyak aplikasi matematika, termasuk analisis keuangan dan pemodelan data.

---

**Soal :**
Buatlah Pembuktian Rumus Berikut : 

$$\sum_{k=1}^n k$$

**Jawab :**
Rumus yang diberikan adalah jumlah bilangan bulat dari \( k = 1 \) hingga \( n \), yaitu:

$$\sum_{k=1}^n k = 1 + 2 + 3 + \dots + n$$

Rumus ini memiliki bentuk tertutup yang dinyatakan sebagai:

$$\sum_{k=1}^n k = \frac{n(n+1)}{2}$$

Berikut adalah pembuktiannya:

---

### Pembuktian:
**Langkah 1: Tulis deretnya dua kali dengan urutan terbalik**  
Tulis jumlah $( S )$ dua kali, satu dalam urutan asli, dan satu dalam urutan terbalik:

$$S = 1 + 2 + 3 + \dots + n$$

$$S = n + (n-1) + (n-2) + \dots + 1$$

**Langkah 2: Tambahkan kedua persamaan**  
Tambahkan kedua persamaan tersebut secara baris demi baris:

$$2S = (1 + n) + (2 + (n-1)) + (3 + (n-2)) + \dots + (n + 1)$$

Setiap pasangan menghasilkan jumlah $(n + 1)$, dan ada total $( n )$ pasangan:

$$2S = n(n+1)$$

**Langkah 3: Sederhanakan**  
Bagi kedua sisi persamaan dengan 2 untuk mendapatkan $( S )$:

$$S = \frac{n(n+1)}{2}$$

---

### Hasil Akhir:
Rumus jumlah bilangan bulat dari 1 hingga \( n \) adalah:

$$\sum_{k=1}^n k = \frac{n(n+1)}{2}.$$

Rumus ini sering digunakan dalam teori bilangan, kombinatorika, dan aplikasi lainnya.

---
**Soal :**
Buatlah Pembuktian Rumus Berikut

$$\sum_{k=1}^n k^2$$

**Jawab :**
Rumus yang ditampilkan adalah bentuk jumlah kuadrat dari bilangan bulat pertama hingga $(n)$, yaitu:

$$\sum_{k=1}^n k^2$$

Rumus umumnya adalah:

$$\sum_{k=1}^n k^2 = \frac{n(n+1)(2n+1)}{6}.$$

**Pembuktian**
Pembuktian rumus ini dapat dilakukan menggunakan **induksi matematika**.

---

**Langkah 1: Basis Induksi**
Untuk $( n = 1 )$, hitunglah sisi kiri dan sisi kanan.

- Sisi kiri:

$$\sum_{k=1}^1 k^2 = 1^2 = 1.$$

- Sisi kanan:

$$\frac{1(1+1)(2(1)+1)}{6} = \frac{1 \cdot 2 \cdot 3}{6} = 1.$$

Jadi, basis induksi benar.

---

**Langkah 2: Asumsi Induksi**
Misalkan rumus benar untuk $( n = m )$, yaitu:

$$\sum_{k=1}^m k^2 = \frac{m(m+1)(2m+1)}{6}.$$

---

**Langkah 3: Pembuktian untuk $n = m+1$**
Tambahkan suku berikutnya ($(m+1)^2$) pada kedua sisi asumsi induksi:

$$\sum_{k=1}^{m+1} k^2 = \sum_{k=1}^m k^2 + (m+1)^2.$$

Dari asumsi induksi:

$$\sum_{k=1}^{m+1} k^2 = \frac{m(m+1)(2m+1)}{6} + (m+1)^2.$$

Faktor $(m+1)$ dari kedua suku:

$$\sum_{k=1}^{m+1} k^2 = \frac{(m+1) \left[ m(2m+1) + 6(m+1) \right]}{6}.$$

Sederhanakan ekspresi dalam kurung:

$$m(2m+1) + 6(m+1) = 2m^2 + m + 6m + 6 = 2m^2 + 7m + 6.$$

Faktorkan:

$$2m^2 + 7m + 6 = (m+2)(2m+3).$$

Substitusikan kembali:

$$\sum_{k=1}^{m+1} k^2 = \frac{(m+1)(m+2)(2m+3)}{6}.$$

Ini sesuai dengan bentuk rumus untuk $n = m+1$. Maka, langkah induksi terbukti.

## Sumasi ganda
- Di dalam algoritma, kita perlu menghitung berapa kali suatu operasi tertentu dilakukan di dalam sebuah kalang bersarang (nested loop). Penjumlahan semua operasi di dalam kalang bersarang dinyatakan dalam bentuk sumasi ganda.

Contoh: $\sum_{i=1}^{4} \sum_{j=1}^{3} ij$

Untuk menghitung sumasi ganda, mula-mula ekspansi sumasi terdalam, lalu dilanjutkan dengan sumasi terluar:
$\sum_{i=1}^{4} \sum_{j=1}^{3} ij =\sum_{i=1}^{4} \left( i + 2i + 3i\right) = \sum_{i=1}^{4} 6i = 6 +12 + 18 + 24 = 60$

Contoh penggunaan: Berapa kali operasi + dilakukan di dalam algoritma di bawah ini? 
x = 0
for j = 1 to 10 do
    for k = 1 to j do
           x = x + 2
   end for
end for 

Penyelesaian:
Operasi + terdapat di dalam pernyataan x = x + 2 Operasi ini dilakukan satu kali pada setiap pengulangan.

Jumlah seluruh operasi + adalah:

$t = \sum_{j=1}^{10} \sum_{k=1}^{j} 1$ 

$= \sum_{j=1}^{10} (1 + 1 + \dots +1$ sebanyak  j  kali)

$= \sum_{j=1}^{10} j$

$= \frac{10(10+1)}{2} = 55$

___

Latihan:
1. Tentukan nilai $\sum_{k=1}^8 2^k + \sum_{k=2}^8 (-3)^k$

2. Tentukan nilai $\sum_{i=0}^2 \sum_{j=0}^3 (2i + 3j)$

3. Tentukan nilai $\sum_{i=0}^3 \sum_{j=0}^2 i$

Jawab:
1. Tentukan nilai $\sum_{k=1}^8 2^k + \sum_{k=2}^8 (-3)^k$

Untuk $\sum_{k=1}^8 2^k$, kita memiliki deret geometrik dengan rasio $r = 2$, suku pertama $a = 2$, dan jumlah $n = 8$:

$\sum_{k=1}^8 2^k = 2 + 2^2 + 2^3 + \dots + 2^8 = 2 \cdot \frac{2^8 - 1}{2 - 1} = 2(255) = 510$

Untuk $\sum_{k=2}^8 (-3)^k$, ini juga merupakan deret geometrik dengan $r = -3$, suku pertama $a = (-3)^2 = 9$, dan jumlah $n = 7$:

$\sum_{k=2}^8 (-3)^k = (-3)^2 + (-3)^3 + \dots + (-3)^8 = \frac{9(1 - (-3)^7)}{1 - (-3)}$

$= \frac{9(1 + 2187)}{4} = \frac{9 \cdot 2188}{4} = 4923 ]$

Sehingga jumlah totalnya:

$\sum_{k=1}^8 2^k + \sum_{k=2}^8 (-3)^k = 510 + 4923 = 5433$

___

2. Tentukan nilai $\sum_{i=0}^2 \sum_{j=0}^3 (2i + 3j)$

Kita akan menghitung:

$\sum_{i=0}^2 \sum_{j=0}^3 (2i + 3j) = \sum_{i=0}^2 \left( \sum_{j=0}^3 2i + \sum_{j=0}^3 3j \right)$

Untuk $\sum_{j=0}^3 2i$, karena $2i$ konstan terhadap $j$, hasilnya:

$\sum_{j=0}^3 2i = 4(2i) = 8i$

Untuk $\sum_{j=0}^3 3j$, ini adalah jumlah deret aritmatika:

$\sum_{j=0}^3 3j = 3(0 + 1 + 2 + 3) = 3 \cdot 6 = 18$

Sehingga:

$\sum_{i=0}^2 \sum_{j=0}^3 (2i + 3j) = \sum_{i=0}^2 (8i + 18) = \sum_{i=0}^2 8i + \sum_{i=0}^2 18$

$\sum_{i=0}^2 8i = 8(0 + 1 + 2) = 8 \cdot 3 = 24$

$\sum_{i=0}^2 18 = 3 \cdot 18 = 54 ]$

Sehingga totalnya:

$\sum_{i=0}^2 \sum_{j=0}^3 (2i + 3j) = 24 + 54 = 78$

---

3. Tentukan nilai $\sum_{i=0}^3 \sum_{j=0}^2 i$

Karena $i$ tidak bergantung pada $j$, maka:

$\sum_{i=0}^3 \sum_{j=0}^2 i =\sum_{i=0}^3 \left( \sum_{j=0}^2 i\right) = \sum_{i=0}^3 \left(3i\right)$

\sum_{i=0}^3 3i = 3 \cdot \sum_{i=0}^3 i = 3(0 + 1 + 2 + 3) = 3 \cdot 6 = 18


---

Jawaban akhir:

1. $\sum_{k=1}^8 2^k + \sum_{k=2}^8 (7-3)^k = 5433$


2. $\sum_{i=0}^2 \sum_{j=0}^3 (2i + 3j) = 78$


3. $\sum_{i=0}^3 \sum_{j=0}^2 i = 18$

## Rekursi
-Sebuah objek dikatakan rekursif (recursive) jika ia didefinisikan dalam terminologi dirinya sendiri.

-Proses mendefinisikan objek dalam terminologi dirinya sendiri disebut rekursi (recursion).

-Perhatikan tiga buah gambar pada tiga slide berikut ini.

___
Objek fraktal adalah contoh rekursif. 

![1000122502](https://hackmd.io/_uploads/HkhHupg7ke.jpg)

## Fungsi Rekursif

Fungsi rekursif didefinisikan oleh dua bagian: 
(i) Basis
1. Bagian yang berisi nilai fungsi yang terdefinisi secara eksplisit. 2. Bagian ini juga sekaligus menghentikan rekursif (dan memberikan sebuah nilai yang terdefinisi pada fungsi rekursif). (ii) Rekurens
1. Bagian ini mendefinisikan fungsi dalam terminologi dirinya sendiri 2. Berisi kaidah untuk menemukan nilai fungsi pada suatu input dari nilai-nilai lainnya pada input yang lebih kecil.

___

Contoh 6: Misalkan f didefinsikan secara rekusif sbb

$f(n) =
\begin{cases} 
3, & \text{jika } n = 0 \\ 
2f(n-1) + 4, & \text{jika } n > 0
\end{cases}$

Tentukan nilai $f$(4)!

Solusi:      
f(4) = 2f(3) + 4 
	 =  2(2f(2) + 4) + 4
	 =  2(2(2f(1) + 4) + 4) + 4
	 =  2(2(2(2f(0) + 4) + 4) + 4) + 4
	 =  2(2(2(2.3 + 4) + 4) + 4) + 4	
	 =  2(2(2(10) + 4) + 4) + 4
	 =  2(2(24) + 4) + 4
	 =  2(52) + 4
	 = 108	

Cara lain menghitungnya:
f(0) = 3
f(1) = 2f(0) + 4 = 2 . 3 + 4 = 10
f(2) = 2f(1) + 4 = 2 . 10 + 4 = 24
f(3) = 2f(2) + 4 = 2 . 24 + 4 = 52
f(4) = 2f(3) + 4 = 2 . 52 + 4 = 108
		
Jadi, f(4) = 108.

___

Contoh 7: Nyatakan n! dalam definisi rekursif

Solusi: $n! = 1 \times 2 \times 3 \times \ldots \times (n-1) \times n = (n-1)! \times n$

Misalkan f(n) = n!, maka  
$n! =
\begin{cases} 
1, & \text{jika } n = 0 \\ 
n \cdot (n-1)!, & \text{jika } n > 0
\end{cases}$

Menghitung 5! secara rekursif adalah:
5! = 5 . 4! = 5 . 4 . 3! = 5 . 4 . 3 . 2! = 5 . 4 . 3 . 2 . 1! = 5 . 4 . 3 . 2 . 1 . 0!	=  5 . 4 . 3 . 2 . 1 . 1 = 120

___

Algoritma menghitung faktorial:

function Faktorial (input  n :integer)integer
{ mengembalikan nilai n!;
  basis   : jika n = 0, maka 0! = 1
  rekurens: jika n > 0, maka n! = n  (n-1)!
}
DEKLARASI
      -
ALGORITMA:
    if n = 0 then
       return 1		              { basis }
    else
       return  n * Faktorial(n – 1)	{ rekurens }
    end
    
___

Contoh 8: Barisan Fibonacci  0, 1, 1, 2, 3, 5, 8, 11, 19, …. Dapat dinyatakan secara rekursif sebagai berikut:

$t_n = \begin{cases} 
0 & \text{jika } n = 0 \\
1 & \text{jika } n = 1 \\
t_{n-1} + t_{n-2} & \text{jika } n > 1 
\end{cases}$

___

Contoh 9: Fungsi (polinom) Chebyshev dinyatakan sebagai

$I(n, x) = 
\begin{cases} 
1 & \text{jika } n = 0 \\
x & \text{jika } n = 1 \\
2x \cdot I(n-1, x) - I(n-2, x) & \text{jika } n > 1 
\end{cases}$

Contoh 10: Sumasi$\sum_{k=0}^{n} a_k$ didefinisikan secara rekursif sebagai  berikut:

$\sum_{k=0}^{n} a_k = a_0 + a_1 + a_2 + \ldots + a_{n-1} + a_n$

$= (a_0 + a_1 + a_2 + \ldots + a_{n-1}) + a_n$

$= \left( \sum_{k=0}^{n-1} a_k \right) + a_n$

Sehingga $\sum_{k=0}^{n} a_k = 
\begin{cases} 
a_0, & \text{jika } n = 0 \\
\left( \sum_{k=0}^{n-1} a_k \right) + a_n, & \text{jika } n > 0
\end{cases}$

___

Latihan
1. Definisikan an secara rekursif , yang dalam hal ini a adalah  sebilangan riil tidak-nol dan n adalah bilangan bulat tidak-negatif.

2. Nyatakan a . b secara rekursif, yang dalam hal ini a dan b adalah bilangan bulat positif.

Solusi:

$a^n = a \cdot a \cdot a \cdot \ldots \cdot a \quad \text{(n kali)}$

$a^{n-1} = a \cdot a \cdot a \cdot \ldots \cdot a \quad \text{(n-1 kali)}$

Sehingga $a^n = 
\begin{cases} 
1, & \text{jika } n = 0 \\
a \cdot a^{n-1}, & \text{jika } n > 0 
\end{cases}$

2. $\begin{align*}
a \cdot b &= b + b + \ldots + b \quad \text{(a kali)} \\
&= b + b + \ldots + b \\
&= b + (a - 1)b \\ &\Rightarrow a \cdot b = \begin{cases} b & , \text{jika } a = 1\\b + (a - 1)b & , \text{jika } a > 1\end{cases}\end{align*}$

## Struktur Rekursif
Struktur data yang penting dalam komputer adalah pohon biner (binary tree).

![1000122546](https://hackmd.io/_uploads/rybwfReX1e.jpg)

- Simpul (node) pada pohon biner mempunyai paling banyak dua buah anak.

- Jumlah anak pada setiap simpul bisa 1, 2, atau 0.

- Simpul yang mempunyai anak disebut simpul cabang (branch node) atau simpul dalam (internal node)

- Simpul yang tidak mempunyai anak disebut simpul daun (leave).

___
Pohon biner adalah struktur yang rekursif, sebab setiap simpul mempunyai cabang yang juga berupa pohon. Setiap cabang disebut  upapohon (subtree).

![1000122554](https://hackmd.io/_uploads/rJY0f0lmkl.jpg)

___
Oleh karena itu, pohon dapat didefinisikan secara rekursif sebagari berikut:

(i) Basis: kosong adalah pohon biner
(ii) Rekurens: Jika T1 dan T2 adalah pohon biner, maka adalah pohon biner

___
Proses pembuatan pohon biner secara rekursif

![1000122558](https://hackmd.io/_uploads/r1zoE0em1e.jpg)
