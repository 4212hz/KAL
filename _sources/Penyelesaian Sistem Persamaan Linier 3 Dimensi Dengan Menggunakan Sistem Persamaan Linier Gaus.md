---
title: Penyelesaian Sistem Persamaan Linier 3 Dimensi Dengan Menggunakan Sistem Persamaan Linier Gaus

---

# Sistem Persamaan Linear Tiga Dimensi Tanpa Solusi
Sistem persamaan linear tiga dimensi tanpa solusi berarti bahwa tiga bidang yang diwakili oleh persamaan tersebut tidak berpotongan pada suatu titik di ruang tiga dimensi. Hal ini terjadi jika bidang-bidang tersebut sejajar atau bertentangan, sehingga tidak ada titik yang memenuhi semua persamaan sekaligus.

## Contoh sistem persamaan linier tiga dimensi tanpa solusi: 
- x+y+z=4
- x+y+z=6
- x+y+z=8

## Penyelesaian dengan eliminasi gaus : 
Meskipun kita sudah tahu bahwa sistem ini tidak memiliki solusi, kita akan mencoba menyelesaikannya menggunakan eliminasi Gauss untuk memverifikasi. 

Langkah 1: Tulis Matriks Augmented  
Pertama, kita tulis sistem persamaan dalam bentuk matriks augmented:

![Capture](https://hackmd.io/_uploads/HJcpYcesyx.png)

Langkah 2: Eliminasi Gauss  
Kita akan melakukan operasi baris untuk mengubah matriks menjadi bentuk eselon baris.

1. Baris 2 - Baris 1:

![Capture1](https://hackmd.io/_uploads/HJH059xiyx.png)

2. Baris 3 - Baris 1:

![Capture2](https://hackmd.io/_uploads/HyJkj5loyl.png)

Langkah 3: Analisis Matriks Hasil  
Setelah eliminasi, matriks menjadi:

![Capture3](https://hackmd.io/_uploads/SJQmsqej1x.png)

Pada baris kedua dan ketiga, kita memiliki 0=2 dan 0=4, yang jelas tidak mungkin. Ini menunjukkan bahwa sistem persamaan ini tidak konsisten dan **tidak memiliki solusi**.

## Kesimpulan:
Sistem persamaan linear tiga dimensi ini tidak memiliki solusi karena ketiga persamaan saling bertentangan. Hal ini terlihat jelas baik dari analisis intuitif maupun dari proses eliminasi Gauss.

<iframe src="https://www.geogebra.org/calculator/f7wx5r3k?embed" width="800" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

# Sistem Persamaan Linier Tiga Dimensi Satu Solusi
Sistem persamaan linear tiga dimensi memiliki satu solusi jika ketiga bidang yang diwakili oleh persamaan tersebut saling berpotongan di satu titik. Dalam hal ini, kita akan menyelesaikan sistem persamaan linear berikut dengan menggunakan metode Eliminasi Gauss untuk menemukan solusi dari variabel 
𝑥,𝑦, dan 𝑧.

## Contoh sistem persamaan linier tiga dimensi satu solusi: 
- x+y+z=6
- 2x-y+3z=14
- -x+4y-z=-2

## Penyelesaian dengan eliminasi gaus : 
Langkah 1: Tulis Matriks Augmented  
Sistem persamaan di atas dapat ditulis dalam bentuk matriks augmented sebagai berikut:

![Capture4](https://hackmd.io/_uploads/Hy8Dgseoye.png)

Langkah 2: Eliminasi Gauss  
Kita akan melakukan operasi baris untuk mengubah matriks menjadi bentuk eselon baris.
Operasi Baris 1: Membuat elemen di bawah a11 menjadi 0
1. Baris 2 - 2 × Baris 1:

![Capture5](https://hackmd.io/_uploads/ByHgZigo1l.png)

2. Baris 3 + Baris 1:

![Capture6](https://hackmd.io/_uploads/H1wVWoesyg.png)

Operasi Baris 2: Membuat elemen di bawah a22 menjadi 0
1. Baris 3 + 5/3 × Baris 2:

![Capture7](https://hackmd.io/_uploads/r1qnZsxokg.png)

Langkah 3: Substitusi Balik (Back Substitution)
Setelah eliminasi, matriks berada dalam bentuk eselon baris:

![Capture8](https://hackmd.io/_uploads/ryifMixsyx.png)

Langkah 3.1: Selesaikan untuk z
Dari baris ketiga:

![Capture9](https://hackmd.io/_uploads/HJ4Dzseikx.png)

Langkah 3.2: Selesaikan untuk y
Dari baris kedua:

![Capture10](https://hackmd.io/_uploads/rJBnMses1g.png)

Langkah 3.3: Selesaikan untuk x
Dari baris pertama:

![Capture11](https://hackmd.io/_uploads/HkpZXslsJl.png)

Solusi Sistem Persamaan
Solusi sistem persamaan ini adalah:

![Capture12](https://hackmd.io/_uploads/rktHmogjJg.png)

Verifikasi Solusi
Mari kita verifikasi solusi ini dengan substitusi ke dalam persamaan asli:

1. Persamaan 1:

![Capture13](https://hackmd.io/_uploads/rkQjQigjJg.png)

2. Persamaan 2:

![Capture14](https://hackmd.io/_uploads/SyiyEjeoke.png)

3. Persamaan 3:

![Capture15](https://hackmd.io/_uploads/rydSNoliye.png)

## Kesimpulan
Sistem persamaan linear ini memiliki satu solusi, yaitu:

![Capture16](https://hackmd.io/_uploads/rJi54olske.png)


<iframe src="https://www.geogebra.org/calculator/apeg5wvm?embed" width="800" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

# Sistem Persamaan Linear Tiga Dimensi Solusi Tak Hingga
Sistem persamaan linear tiga dimensi dapat memiliki solusi tak hingga jika ketiga persamaan tersebut mewakili tiga bidang yang saling sejajar, sehingga mereka tidak berpotongan pada satu titik, tetapi membentuk satu garis atau ruang yang lebih besar dengan solusi tak hingga. Dalam kasus ini, kita akan memiliki solusi tak hingga jika ketiga persamaan tersebut tidak independen satu sama lain, dan dapat digambarkan sebagai bidang yang sejajar.

## Contoh sistem persamaan linier tiga dimensi solusi tak hingga: 
- x+y+z=6
- x+2y+2z=12
- x+3y+3z=18

## Penyelesaian dengan eliminasi gaus : 
Langkah 1: Tulis Matriks Augmented
Sistem persamaan di atas dapat ditulis dalam bentuk matriks augmented sebagai berikut:

![Capture17](https://hackmd.io/_uploads/rkN_Kjgikg.png)

Langkah 2: Eliminasi Gauss
Kita akan melakukan operasi baris untuk mengubah matriks menjadi bentuk eselon baris.

Operasi Baris 1: Membuat elemen di bawah a11 menjadi 0

1. Baris 2 - 2 × Baris 1:

![Capture18](https://hackmd.io/_uploads/r1u1qoloyg.png)

2. Baris 3 - 3 × Baris 1:

![Capture19](https://hackmd.io/_uploads/Hk5Xcigi1e.png)

Langkah 3: Analisis Matriks Hasil
Setelah eliminasi, matriks menjadi:

![Capture20](https://hackmd.io/_uploads/B149coloJg.png)

- Baris kedua dan ketiga semuanya adalah 0=0, yang menunjukkan bahwa persamaan-persamaan ini redundan (tidak memberikan informasi baru).
- Hanya satu persamaan yang independen, yaitu x+y+z=6.

Langkah 4: Tentukan Solusi
Karena hanya ada satu persamaan independen, sistem ini memiliki solusi tak hingga. Solusi umumnya dapat dinyatakan dalam bentuk parameter.

Langkah 4.1: Tentukan Variabel Bebas
Misalkan y dan z adalah variabel bebas. Kita dapat menyatakan x dalam bentuk y dan z:

![Capture21](https://hackmd.io/_uploads/rJkKjolskl.png)

Langkah 4.2: Tulis Solusi Umum
Solusi umum sistem persamaan ini adalah:

![Capture22](https://hackmd.io/_uploads/ryjnssei1g.png)

Di mana y dan z dapat mengambil nilai berapa pun.

## Kesimpulan
Sistem persamaan linear ini memiliki solusi tak hingga. Solusi umumnya dapat dinyatakan sebagai:

![Capture23](https://hackmd.io/_uploads/rk9zhseskl.png)

di mana y dan z adalah parameter bebas.

<iframe src="https://www.geogebra.org/calculator/vzt9k8ce?embed" width="800" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>