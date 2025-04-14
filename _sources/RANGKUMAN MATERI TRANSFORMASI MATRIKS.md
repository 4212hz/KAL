---
title: RANGKUMAN MATERI TRANSFORMASI MATRIKS

---

# RANGKUMAN MATERI TRANSFORMASI MATRIKS

Pada bab ini, kita mempelajari konsep dasar dari transformasi matriks, yaitu suatu aturan yang mengubah vektor menjadi vektor lain melalui operasi perkalian matriks. Transformasi ini merupakan alat penting yang banyak digunakan dalam berbagai bidang seperti matematika, ilmu fisika, dan rekayasa teknik karena kemampuannya dalam memodelkan perubahan posisi, arah, atau bentuk dari suatu objek dalam ruang.

## Transformasi Matriks

Sebuah transformasi matriks adalah fungsi linear $T: \mathbb{R}^n \rightarrow \mathbb{R}^m$ yang didefinisikan oleh:

$T(\vec{x}) = A\vec{x}$

di mana $A$ adalah matriks berukuran $m \times n$ dan $\vec{x}$ adalah vektor kolom berdimensi $n$ di $\mathbb{R}^n$.

Transformasi matriks bersifat linear, yang berarti memenuhi dua sifat berikut:

$T(\vec{u} + \vec{v}) = T(\vec{u}) + T(\vec{v})$
$T(c\vec{u}) = cT(\vec{u})$, untuk setiap skalar $c$

Contoh :

Misalkan kita memiliki transformasi $T: \mathbb{R}^2 \rightarrow \mathbb{R}^2$ yang didefinisikan oleh matriks:

$
A = \begin{bmatrix} 2 & 3 \\ -1 & 4 \end{bmatrix}
$ 
dan dua vektor:

$$
\vec{u} = \begin{bmatrix} 1 \\ 2 \end{bmatrix}
\vec{v} = \begin{bmatrix} -1 \\ 0 \end{bmatrix}
$$
c = 5

Hitung $T(\vec{u})$, $T(\vec{v})$, $T(\vec{u} + \vec{v})$, dan $T(c\vec{u})$:

$$
T(\vec{u}) = A\vec{u} = \begin{bmatrix} 2 & 3 \\ -1 & 4 \end{bmatrix} 
\begin{bmatrix} 1 \\ 2 \end{bmatrix} = 
\begin{bmatrix} 2(1) + 3(2) \\ -1(1) + 4(2) \end{bmatrix} = 
\begin{bmatrix} 8 \\ 7 \end{bmatrix}
$$

$$
T(\vec{v}) = A\vec{v} = \begin{bmatrix} 2 & 3 \\ -1 & 4 \end{bmatrix}
\begin{bmatrix} -1 \\ 0 \end{bmatrix} =
\begin{bmatrix} 2(-1) + 3(0) \\ -1(-1) + 4(0) \end{bmatrix} =
\begin{bmatrix} -2 \\ 1 \end{bmatrix}
$$

$$
\vec{u} + \vec{v} = \begin{bmatrix} 1 + (-1) \\ 2 + 0 \end{bmatrix} = 
\begin{bmatrix} 0 \\ 2 \end{bmatrix}
\Rightarrow T(\vec{u} + \vec{v}) = A \begin{bmatrix} 0 \\ 2 \end{bmatrix} =
\begin{bmatrix} 6 \\ 8 \end{bmatrix}
$$

$$
T(\vec{u}) + T(\vec{v}) = \begin{bmatrix} 8 \\ 7 \end{bmatrix} + \begin{bmatrix} -2 \\ 1 \end{bmatrix} = 
\begin{bmatrix} 6 \\ 8 \end{bmatrix}
\Rightarrow T(\vec{u} + \vec{v}) = T(\vec{u}) + T(\vec{v})
$$

$$
T(c\vec{u}) = A(c\vec{u}) = A \begin{bmatrix} 5 \\ 10 \end{bmatrix} = 
\begin{bmatrix} 2(5) + 3(10) \\ -1(5) + 4(10) \end{bmatrix} =
\begin{bmatrix} 40 \\ 35 \end{bmatrix}
$$

$$
cT(\vec{u}) = 5 \begin{bmatrix} 8 \\ 7 \end{bmatrix} = 
\begin{bmatrix} 40 \\ 35 \end{bmatrix}
\Rightarrow T(c\vec{u}) = cT(\vec{u})
$$

Kesimpulan

Transformasi $T(\vec{x}) = A\vec{x}$ dengan $A = \begin{bmatrix} 2 & 3 \\ -1 & 4 \end{bmatrix}$ merupakan transformasi linear karena memenuhi:

$T(\vec{u} + \vec{v}) = T(\vec{u}) + T(\vec{v})$
$T(c\vec{u}) = cT(\vec{u})$

---

## Matriks dan Perkalian Vektor

Untuk mempermudah visualisasi, kita membatasi pembahasan pada vektor di $\mathbb{R}^2$. Untuk mendapatkan hasil vektor 2D dari perkalian matriks, kita gunakan matriks $2 \times 2$.

Misalkan:

$$
A = \begin{bmatrix} 2 & -1 \\ 0 & 3 \end{bmatrix}
\vec{x} = \begin{bmatrix} 1 \\ 2 \end{bmatrix}
\vec{y} = \begin{bmatrix} -2 \\ 1 \end{bmatrix}
\vec{z} = \begin{bmatrix} 0 \\ -1 \end{bmatrix}
$$

Maka hasil transformasinya:

$$
A\vec{x} = \begin{bmatrix} 2(1) + (-1)(2) \\ 0(1) + 3(2) \end{bmatrix}
= \begin{bmatrix} 0 \\ 6 \end{bmatrix}
$$

$$
A\vec{y} = \begin{bmatrix} 2(-2) + (-1)(1) \\ 0(-2) + 3(1) \end{bmatrix}
= \begin{bmatrix} -5 \\ 3 \end{bmatrix}
$$

$$
A\vec{z} = \begin{bmatrix} 2(0) + (-1)(-1) \\ 0(0) + 3(-1) \end{bmatrix}
= \begin{bmatrix} 1 \\ -3 \end{bmatrix}
$$

Setelah dikalikan dengan $A$, panjang dan arah vektor bisa berubah. Misalnya, $\vec{y}$ dan $\vec{z}$ berubah arah setelah transformasi.

### Contoh Penjumlahan dan Perkalian Matriks

Misalkan:

$$
A = \begin{bmatrix} 3 & 0 \\ 1 & -1 \end{bmatrix}
\vec{p} = \begin{bmatrix} 1 \\ 3 \end{bmatrix}
\vec{q} = \begin{bmatrix} 2 \\ -1 \end{bmatrix}
$$

Langkah pertama:

$$
\vec{p} + \vec{q} = \begin{bmatrix} 1 + 2 \\ 3 + (-1) \end{bmatrix}
= \begin{bmatrix} 3 \\ 2 \end{bmatrix}
$$

Transformasi masing-masing:

$$
A\vec{p} = \begin{bmatrix} 3(1) + 0(3) \\ 1(1) + (-1)(3) \end{bmatrix}
= \begin{bmatrix} 3 \\ -2 \end{bmatrix}
$$

$$
A\vec{q} = \begin{bmatrix} 3(2) + 0(-1) \\ 1(2) + (-1)(-1) \end{bmatrix}
= \begin{bmatrix} 6 \\ 3 \end{bmatrix}
$$

$$
A(\vec{p} + \vec{q}) = A\begin{bmatrix} 3 \\ 2 \end{bmatrix}
= \begin{bmatrix} 3(3) + 0(2) \\ 1(3) + (-1)(2) \end{bmatrix}
= \begin{bmatrix} 9 \\ 1 \end{bmatrix}
$$

$$
A\vec{p} + A\vec{q} = \begin{bmatrix} 3 \\ -2 \end{bmatrix} + \begin{bmatrix} 6 \\ 3 \end{bmatrix}
= \begin{bmatrix} 9 \\ 1 \end{bmatrix}
$$

Hal ini membuktikan bahwa:

$A(\vec{p} + \vec{q}) = A\vec{p} + A\vec{q}$

yang menunjukkan sifat linear dari transformasi matriks.

---

## Transformasi di Bidang Kartesian

Transformasi bidang Kartesian mengubah posisi, bentuk, atau orientasi objek di $\mathbb{R}^2$ atau $\mathbb{R}^3$ dengan menggunakan matriks transformasi linear.

### Jenis-Jenis Transformasi

#### 1. **Translasi (Pergeseran)**

Memindahkan objek sejauh vektor $\vec{v} = [a, b]$:

$$
T(\vec{x}) = \vec{x} + \vec{v}
$$

Contoh:

$$
T\left(\begin{bmatrix} x \\ y \end{bmatrix}\right) = \begin{bmatrix} x + 3 \\ y - 3 \end{bmatrix}
$$

#### 2. **Rotasi (Perputaran)**

Memutar objek dengan sudut $\theta$ terhadap titik asal:

$$
R_\theta = \begin{bmatrix} \cos \theta & -\sin \theta \\ \sin \theta & \cos \theta \end{bmatrix}
$$

Contoh rotasi $90^\circ$:

$$
R_{90^\circ} = \begin{bmatrix} 0 & -1 \\ 1 & 0 \end{bmatrix},\quad
R_{90^\circ} \begin{bmatrix} 1 \\ 0 \end{bmatrix} = \begin{bmatrix} 0 \\ 1 \end{bmatrix}
$$

#### 3. **Penskalaan (Scaling)**

Mengubah ukuran objek:

$$
S = \begin{bmatrix} s_x & 0 \\ 0 & s_y \end{bmatrix}
$$

Contoh skala 2 kali di sumbu x:

$$
S \begin{bmatrix} 3 \\ 4 \end{bmatrix} = \begin{bmatrix} 6 \\ 4 \end{bmatrix}
$$

#### 4. **Refleksi (Pencerminan)**

Contoh:

- Terhadap sumbu $x$: $\begin{bmatrix} 1 & 0 \\ 0 & -1 \end{bmatrix}$
- Terhadap sumbu $y=x$: $\begin{bmatrix} 0 & 1 \\ 1 & 0 \end{bmatrix}$

#### 5. **Shear (Geser)**

Contoh shear horizontal:

$$
\text{Shear} = \begin{bmatrix} 1 & k \\ 0 & 1 \end{bmatrix}
$$

---

## Sifat Transformasi Linear

- Garis lurus tetap lurus setelah transformasi.
- Titik asal tetap (kecuali pada translasi).
- Dapat dikomposisikan: contoh rotasi dan skala dapat digabung dengan $R_\theta \cdot S$.

---

## Latihan 5.1.4 Soal No 1,2,5 dan 6

Diberikan $\vec{x} = \begin{bmatrix} 1 \\ 1 \end{bmatrix}$ dan $\vec{y} = \begin{bmatrix} -1 \\ 2 \end{bmatrix}$, hitung dan sketsa:

### Soal 1

$
A = \begin{bmatrix} 1 & -1 \\ 2 & 3 \end{bmatrix}
$

Dan dua vektor sebagai berikut:

$$
\vec{x} = \begin{bmatrix} 1 \\ 1 \end{bmatrix} 
\vec{y} = \begin{bmatrix} -1 \\ 2 \end{bmatrix}
$$

Langkah 1 : Mencari hasil transformasi dari vektor $\vec{x}$ oleh matriks $A$:
$$
A\vec{x} =
\begin{bmatrix} 1 & -1 \\ 2 & 3 \end{bmatrix}
\begin{bmatrix} 1 \\ 1 \end{bmatrix} =
\begin{bmatrix} 1(1) + (-1)(1) \\ 2(1) + 3(1) \end{bmatrix} =
\begin{bmatrix} 0 \\ 5 \end{bmatrix}
$$

Langkah 2 : Mencari hasil transformasi dari vektor $\vec{y}$ oleh matriks $A$:

$$
A\vec{y} =
\begin{bmatrix} 1 & -1 \\ 2 & 3 \end{bmatrix}
\begin{bmatrix} -1 \\ 2 \end{bmatrix} =
\begin{bmatrix} 1(-1) + (-1)(2) \\ 2(-1) + 3(2) \end{bmatrix} =
\begin{bmatrix} -1 - 2 \\ -2 + 6 \end{bmatrix} =
\begin{bmatrix} -3 \\ 4 \end{bmatrix}
$$

Hasil :

$$
\vec{x} = \begin{bmatrix} 1 \\ 1 \end{bmatrix}
\vec{y} = \begin{bmatrix} -1 \\ 2 \end{bmatrix}
A\vec{x} = \begin{bmatrix} 0 \\ 5 \end{bmatrix}
A\vec{y} = \begin{bmatrix} -3 \\ 4 \end{bmatrix}
$$

![1](https://hackmd.io/_uploads/B1Z0EdDA1g.png)

---

### Soal 2
$
A = \begin{bmatrix} 2 & 0 \\ -1 & 3 \end{bmatrix}
$

Dan dua buah vektor:

$$
\vec{x} = \begin{bmatrix} 1 \\ 1 \end{bmatrix} 
\vec{y} = \begin{bmatrix} -1 \\ 2 \end{bmatrix}
$$

Langkah pertama : Hitung hasil dari $A\vec{x}$

$$
A\vec{x} = 
\begin{bmatrix} 2 & 0 \\ -1 & 3 \end{bmatrix}
\begin{bmatrix} 1 \\ 1 \end{bmatrix} =
\begin{bmatrix} 2(1) + 0(1) \\ -1(1) + 3(1) \end{bmatrix} =
\begin{bmatrix} 2 \\ 2 \end{bmatrix}
$$

Langkah kedua : Hitung hasil dari $A\vec{y}$

$$
A\vec{y} = 
\begin{bmatrix} 2 & 0 \\ -1 & 3 \end{bmatrix}
\begin{bmatrix} -1 \\ 2 \end{bmatrix} =
\begin{bmatrix} 2(-1) + 0(2) \\ -1(-1) + 3(2) \end{bmatrix} =
\begin{bmatrix} -2 \\ 1 + 6 \end{bmatrix} =
\begin{bmatrix} -2 \\ 7 \end{bmatrix}
$$

Hasil :

$$
\vec{x} = \begin{bmatrix} 1 \\ 1 \end{bmatrix}
\vec{y} = \begin{bmatrix} -1 \\ 2 \end{bmatrix}
A\vec{x} = \begin{bmatrix} 2 \\ 2 \end{bmatrix}
A\vec{y} = \begin{bmatrix} -2 \\ 7 \end{bmatrix}
$$

![2](https://hackmd.io/_uploads/rkyU8dP01l.png)

---

### Soal 5

Misalkan titik awal berada di origin $(0, 0)$. Diberikan dua vektor dasar:

$$
\vec{x} = \begin{bmatrix} 1 \\ 0 \end{bmatrix}
\vec{y} = \begin{bmatrix} 0 \\ 1 \end{bmatrix}
\vec{x} + \vec{y} = \begin{bmatrix} 1 \\ 1 \end{bmatrix}
$$

Setelah dikenai transformasi oleh matriks $A$, didapatkan:


$\vec{x}$ dipetakan ke titik $(0.5, 1)$
$\vec{y}$ dipetakan ke titik $(1, 2)$
$\vec{x} + \vec{y}$ dipetakan ke titik $(1.5, 3)$


Sehingga dapat disimpulkan bahwa matriks transformasi $A$ adalah:

$
A = \begin{bmatrix} 0.5 & 1 \\ 1 & 2 \end{bmatrix}
$

![5](https://hackmd.io/_uploads/rkLjXYwAkl.png)

---

### Soal 6

Titik awal terletak di $(0, 0)$ dan diberikan dua vektor:

$$
\vec{x} = \begin{bmatrix} 1 \\ 0 \end{bmatrix}
\vec{y} = \begin{bmatrix} 0 \\ 1 \end{bmatrix}
\vec{x} + \vec{y} = \begin{bmatrix} 1 \\ 1 \end{bmatrix}
$$

Setelah diterapkan transformasi, didapatkan hasil berikut:

$\vec{x}$ menjadi $(-1, 1)$
$\vec{y}$ menjadi $(1, 1)$
$\vec{x} + \vec{y}$ menjadi $(0, 2)$

Maka, matriks transformasi yang sesuai adalah:

$
A = \begin{bmatrix} -1 & 1 \\ 1 & 1 \end{bmatrix}
$

![6](https://hackmd.io/_uploads/H1S5IFwCJx.png)
