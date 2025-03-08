---
title: Penyelesaian Sistem Persamaan Linier 3 Dimensi Dengan Menggunakan Sistem Persamaan Linier Gaus

---

# Sistem Persamaan Linear Tiga Dimensi Tanpa Solusi
Sistem persamaan linear tiga dimensi tanpa solusi berarti bahwa tiga bidang yang diwakili oleh persamaan tersebut tidak berpotongan pada suatu titik di ruang tiga dimensi. Hal ini terjadi jika bidang-bidang tersebut sejajar atau bertentangan, sehingga tidak ada titik yang memenuhi semua persamaan sekaligus.

## Contoh sistem persamaan linier tiga dimensi tanpa solusi: 
- $x$+$y$+$z$=4
- $x$+$y$+$z$=6
- $x$+$y$+$z$=8

## Penyelesaian dengan eliminasi gaus : 
Meskipun kita sudah tahu bahwa sistem ini tidak memiliki solusi, kita akan mencoba menyelesaikannya menggunakan eliminasi Gauss untuk memverifikasi. 

Langkah 1: Tulis Matriks Augmented  
Pertama, kita tulis sistem persamaan dalam bentuk matriks augmented:
$$
\begin{bmatrix}
1 & 1 & 1 & | 4 \\
1 & 1 & 1 & | 6 \\
1 & 1 & 1 & | 8
\end{bmatrix}
$$


Langkah 2: Eliminasi Gauss  
Kita akan melakukan operasi baris untuk mengubah matriks menjadi bentuk eselon baris.

1. Baris 2 - Baris 1:
$$
\begin{bmatrix}
1 & 1 & 1 & | 4 \\
0 & 0 & 0 & | 2 \\
1 & 1 & 1 & | 8
\end{bmatrix}
$$
2. Baris 3 - Baris 1:
$$
\begin{bmatrix}
1 & 1 & 1 & | 4 \\
0 & 0 & 0 & | 2 \\
0 & 0 & 0 & | 4
\end{bmatrix}
$$
Langkah 3: Analisis Matriks Hasil  
Setelah eliminasi, matriks menjadi:
$$
\begin{bmatrix}
1 & 1 & 1 & | 4 \\
0 & 0 & 0 & | 2 \\
0 & 0 & 0 & | 4
\end{bmatrix}
$$
Pada baris kedua dan ketiga, kita memiliki 0=2 dan 0=4, yang jelas tidak mungkin. Ini menunjukkan bahwa sistem persamaan ini tidak konsisten dan **tidak memiliki solusi**.

## Kesimpulan:
Sistem persamaan linear tiga dimensi ini tidak memiliki solusi karena ketiga persamaan saling bertentangan. Hal ini terlihat jelas baik dari analisis intuitif maupun dari proses eliminasi Gauss.

<iframe src="https://www.geogebra.org/calculator/f7wx5r3k?embed" width="800" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

# Sistem Persamaan Linier Tiga Dimensi Satu Solusi
Sistem persamaan linear tiga dimensi memiliki satu solusi jika ketiga bidang yang diwakili oleh persamaan tersebut saling berpotongan di satu titik. Dalam hal ini, kita akan menyelesaikan sistem persamaan linear berikut dengan menggunakan metode Eliminasi Gauss untuk menemukan solusi dari variabel 
𝑥,𝑦, dan 𝑧.

## Contoh sistem persamaan linier tiga dimensi satu solusi: 
- $x$+$y$+$z$=6
- 2$x$-$y$+3$z$=14
- -$x$+4$y$-$z$=-2

## Penyelesaian dengan eliminasi gaus : 
Langkah 1: Tulis Matriks Augmented  
Sistem persamaan di atas dapat ditulis dalam bentuk matriks augmented sebagai berikut:
$$
\begin{bmatrix}
1 & 1 & 1 & | 6 \\
2 & -1 & 3 & | 14 \\
-1 & 4 & -1 & | -2
\end{bmatrix}
$$
Langkah 2: Eliminasi Gauss  
Kita akan melakukan operasi baris untuk mengubah matriks menjadi bentuk eselon baris.
Operasi Baris 1: Membuat elemen di bawah a11 menjadi 0
1. Baris 2 - 2 × Baris 1:
$$
\begin{bmatrix}
1 & 1 & 1 & | 6 \\
0 & -3 & 1 & | 2 \\
-1 & 4 & -1 & | -2
\end{bmatrix}
$$
2. Baris 3 + Baris 1:
$$
\begin{bmatrix}
1 & 1 & 1 & | 6 \\
0 & -3 & 1 & | 2 \\
0 & 5 & 0 & | 4
\end{bmatrix}
$$
Operasi Baris 2: Membuat elemen di bawah a22 menjadi 0
1. Baris 3 + 5/3 × Baris 2:
$$
\begin{bmatrix}
1 & 1 & 1 & | 6 \\
0 & -3 & 1 & | 2 \\
0 & 0 & \frac{5}{3} & | \frac{22}{3}
\end{bmatrix}
$$
Langkah 3: Substitusi Balik (Back Substitution)
Setelah eliminasi, matriks berada dalam bentuk eselon baris:
$$
\begin{bmatrix}
1 & 1 & 1 & | 6 \\
0 & -3 & 1 & | 2 \\
0 & 0 & \frac{5}{3} & | \frac{22}{3}
\end{bmatrix}
$$
Langkah 3.1: Selesaikan untuk z
Dari baris ketiga:
$$
\begin{bmatrix}
\frac{5}{3}z = \frac{22}{3}
→ z = \frac{22}{5}
\end{bmatrix}
$$
Langkah 3.2: Selesaikan untuk y
Dari baris kedua:
$$
\begin{bmatrix}
-3y + z - 2 →
-3y + \frac{22}{5} - 2 →
-3y - 2 - \frac{22}{5} 
= -\frac{12}{5}
→ y - \frac{4}{5}
\end{bmatrix}
$$
Langkah 3.3: Selesaikan untuk x
Dari baris pertama:
$$
\begin{bmatrix}
x + y + z = 6 →
x + \frac{4}{5} + \frac{22}{5} = 6 →
x + \frac{26}{5} = 6 →
x = 6 - \frac{26}{5}
 = \frac{4}{5}
\end{bmatrix}
$$
Solusi Sistem Persamaan
Solusi sistem persamaan ini adalah:
$$
\begin{bmatrix}
(x, y, z) = \left( \frac{4}{5}, \frac{4}{5}, \frac{22}{5} \right)
\end{bmatrix}
$$
Verifikasi Solusi
Mari kita verifikasi solusi ini dengan substitusi ke dalam persamaan asli:

1. Persamaan 1:
$$
\begin{bmatrix} 
2x - y + 3z = 2(\ \frac{4}{5} ) - \frac{4}{5} )+3(\frac{22}{5}) 
= \frac{8}{5} - \frac{4}{5} + \frac{66}{5} = \frac{70}{5} = 14 \quad (\text{Benar})
\end{bmatrix}
$$
2. Persamaan 2:
$$
\begin{bmatrix}
2x - y + 3z = 2 \left(\frac{4}{5}\right) - \frac{4}{5} + 3\left(\frac{22}{5}\right)
= \frac{8}{5} - \frac{4}{5} + \frac{66}{5} = \frac{70}{5} = 14 \quad (\text{Benar})
\end{bmatrix}
$$
3. Persamaan 3:
$$
\begin{bmatrix}
-x + 4y - z =
-\left(\frac{4}{5}\right) + 4\left(\frac{4}{5}\right) - \frac{22}{5}
= -\frac{4}{5} + \frac{16}{5} - \frac{22}{5}
= -\frac{10}{5} = -2 \quad (\text{Benar})
\end{bmatrix}
$$
## Kesimpulan
Sistem persamaan linear ini memiliki satu solusi, yaitu:
$$
\begin{bmatrix}
x = \frac{4}{5}, \quad y = \frac{4}{5}, \quad z = \frac{22}{5}
\end{bmatrix}
$$
<iframe src="https://www.geogebra.org/calculator/apeg5wvm?embed" width="800" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

# Sistem Persamaan Linear Tiga Dimensi Solusi Tak Hingga
Sistem persamaan linear tiga dimensi dapat memiliki solusi tak hingga jika ketiga persamaan tersebut mewakili tiga bidang yang saling sejajar, sehingga mereka tidak berpotongan pada satu titik, tetapi membentuk satu garis atau ruang yang lebih besar dengan solusi tak hingga. Dalam kasus ini, kita akan memiliki solusi tak hingga jika ketiga persamaan tersebut tidak independen satu sama lain, dan dapat digambarkan sebagai bidang yang sejajar.

## Contoh sistem persamaan linier tiga dimensi solusi tak hingga: 

- $x$+$y$+$z$=6
- $x$+2$y$+2$z$=12
- $x$+3$y$+3$z$=18

## Penyelesaian dengan eliminasi gaus : 
Langkah 1: Tulis Matriks Augmented
Sistem persamaan di atas dapat ditulis dalam bentuk matriks augmented sebagai berikut:
$$
\begin{bmatrix}
1 & 1 & 1 & | 6 \\
2 & 2 & 2 & | 12 \\
3 & 3 & 3 & | 18
\end{bmatrix}
$$
Langkah 2: Eliminasi Gauss
Kita akan melakukan operasi baris untuk mengubah matriks menjadi bentuk eselon baris.

Operasi Baris 1: Membuat elemen di bawah a11 menjadi 0

1. Baris 2 - 2 × Baris 1:
$$
\begin{bmatrix}
1 & 1 & 1 & | 6 \\
0 & 0 & 0 & | 0 \\
3 & 3 & 3 & | 18
\end{bmatrix}
$$
2. Baris 3 - 3 × Baris 1:
$$
\begin{bmatrix}
1 & 1 & 1 & | 6 \\
0 & 0 & 0 & | 0 \\
0 & 0 & 0 & | 0
\end{bmatrix}
$$
Langkah 3: Analisis Matriks Hasil
Setelah eliminasi, matriks menjadi:
$$
\begin{bmatrix}
1 & 1 & 1 & | 6 \\
0 & 0 & 0 & | 0 \\
0 & 0 & 0 & | 0
\end{bmatrix}
$$
- Baris kedua dan ketiga semuanya adalah 0=0, yang menunjukkan bahwa persamaan-persamaan ini redundan (tidak memberikan informasi baru).
- Hanya satu persamaan yang independen, yaitu x+y+z=6.

Langkah 4: Tentukan Solusi
Karena hanya ada satu persamaan independen, sistem ini memiliki solusi tak hingga. Solusi umumnya dapat dinyatakan dalam bentuk parameter.

Langkah 4.1: Tentukan Variabel Bebas
Misalkan y dan z adalah variabel bebas. Kita dapat menyatakan x dalam bentuk y dan z:
$$
\begin{bmatrix}
x = 6 - y - z
\end{bmatrix}
$$
Langkah 4.2: Tulis Solusi Umum
Solusi umum sistem persamaan ini adalah:
$$
\begin{cases}
x = 6 - y - z \\
y = y \quad \text{(variabel bebas)} \\
z = z \quad \text{(variabel bebas)}
\end{cases}
$$
Di mana y dan z dapat mengambil nilai berapa pun.

## Kesimpulan
Sistem persamaan linear ini memiliki solusi tak hingga. Solusi umumnya dapat dinyatakan sebagai:
$$
\begin{bmatrix}
(x, y, z) = (6 - y - z, y, z)
\end{bmatrix}
$$
di mana y dan z adalah parameter bebas.

<iframe src="https://www.geogebra.org/calculator/vzt9k8ce?embed" width="800" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>