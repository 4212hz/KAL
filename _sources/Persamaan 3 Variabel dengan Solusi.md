---
title: Persamaan 3 Variabel dengan Solusi

---

# Solusi Sistem Persamaan Linear x=1,y=0,z=0

# DEFINISI MATRIKS INVERS
Matriks invers adalah konsep dalam aljabar linear dimana untuk suatu matriks persegi A berukuran n×n, terdapat matriks B berukuran n×n yang memenuhi:
AB = BA = Iₙ
dengan:

Iₙ = matriks identitas berukuran n×n

B disebut invers dari A, dinotasikan A⁻¹

## Syarat Keberadaan Invers
Suatu matriks memiliki invers jika dan hanya jika:

Matriks tersebut persegi (jumlah baris = jumlah kolom)

Determinan matriks ≠ 0 (det(A) ≠ 0)

Matriks memiliki rank penuh (full rank)

##  Sifat-Sifat Matriks Invers
Jika A dan B matriks invertible:

(A⁻¹)⁻¹ = A

(AB)⁻¹ = B⁻¹A⁻¹

(kA)⁻¹ = (1/k)A⁻¹ untuk skalar k ≠ 0

(Aᵀ)⁻¹ = (A⁻¹)ᵀ

det(A⁻¹) = 1/det(A)

## Contoh Perhitungan Invers
Untuk matriks 2×2:
A = [a b; c d]
A⁻¹ = (1/det(A)) × [d -b; -c a]
dimana det(A) = ad - bc ≠ 0

##  Metode Menghitung Invers
a. Metode OBE (Operasi Baris Elementer):

Bentuk matriks augmented [A|I]

Lakukan operasi baris hingga menjadi [I|A⁻¹]

b. Metode Adjoin:
A⁻¹ = (1/det(A)) × adj(A)
dengan adj(A) = matriks adjoin dari A

c. Metode Dekomposisi (LU, QR, dll.)

##  Matriks Singular vs Non-Singular

Non-Singular: Matriks yang memiliki invers (det(A) ≠ 0)

Singular: Matriks yang tidak memiliki invers (det(A) = 0)

## Aplikasi Matriks Invers

Penyelesaian sistem persamaan linear AX = B → X = A⁻¹B

Analisis rangkaian listrik

Komputer grafis dan transformasi linear

Kriptografi dan pengolahan sinyal

# Tugas: Contoh Persamaan 3 Variabel dengan Solusi \( x = 1 \), \( y = 0 \), \( z = 0 \)

Persamaan:
$
\begin{cases}
3x + 2y + z = 3 \\
2x + y + 4z = 2 \\
x + 3y + 2z = 1
\end{cases}
$

## Langkah Penyelesaian:

1. Bentuk Matriks Augmented:
$
\begin{bmatrix}
3 & 2 & 1 & 3 \\
2 & 1 & 4 & 2 \\
1 & 3 & 2 & 1
\end{bmatrix}
$

2. Mencari Invers Matriks \( A \):

Matriks koefisien \( A \) dan matriks identitas \( I \):
$
A = \begin{bmatrix}
3 & 2 & 1 \\
2 & 1 & 4 \\
1 & 3 & 2
\end{bmatrix},
I = \begin{bmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1
\end{bmatrix}
$

Bentuk matriks augmented \([A|I]\):

$
\begin{bmatrix}
3 & 2 & 1 & 1 & 0 & 0 \\
2 & 1 & 4 & 0 & 1 & 0 \\
1 & 3 & 2 & 0 & 0 & 1
\end{bmatrix}
$

3. Operasi Baris Elementer (OBE):


Langkah 1:Tukar R_1 dan R_3
$
\begin{bmatrix}
1 & 3 & 2 & 0 & 0 & 1 \\
2 & 1 & 4 & 0 & 1 & 0 \\
3 & 2 & 1 & 1 & 0 & 0
\end{bmatrix}
$

Langkah 2:$\begin{bmatrix} R_2 \rightarrow R_2 - 2R_1 : \end{bmatrix}$
$
\begin{bmatrix}
1 & 3 & 2 & 0 & 0 & 1 \\
0 & -5 & 0 & 0 & 1 & -2 \\
3 & 2 & 1 & 1 & 0 & 0
\end{bmatrix}
$

Langkah 3:$ \begin{bmatrix} R_3 \rightarrow R_3 - 3R_1 : \end{bmatrix}$

$
\begin{bmatrix}
1 & 3 & 2 & 0 & 0 & 1 \\
0 & -5 & 0 & 0 & 1 & -2 \\
0 & -7 & -5 & 1 & 0 & -3
\end{bmatrix}
$

Langkah 4:$\begin{bmatrix} R_2 \rightarrow -\frac{1}{5}R_2 :\end{bmatrix}$

$
\begin{bmatrix}
1 & 3 & 2 & 0 & 0 & 1 \\
0 & 1 & 0 & 0 & -\frac{1}{5} & \frac{2}{5} \\
0 & -7 & -5 & 1 & 0 & -3
\end{bmatrix}
$

Langkah 5: $\begin{bmatrix} R_1 \rightarrow R_1 - 3R_2: \end{bmatrix}$

$
\begin{bmatrix}
1 & 0 & 2 & 0 & \frac{3}{5} & -\frac{1}{5} \\
0 & 1 & 0 & 0 & -\frac{1}{5} & \frac{2}{5} \\
0 & -7 & -5 & 1 & 0 & -3
\end{bmatrix}
$

Langkah 6:$\begin{bmatrix} R_3 \rightarrow R_3 + 7R_2:\end{bmatrix}$

$
\begin{bmatrix}
1 & 0 & 2 & 0 & \frac{3}{5} & -\frac{1}{5} \\
0 & 1 & 0 & 0 & -\frac{1}{5} & \frac{2}{5} \\
0 & 0 & -5 & 1 & -\frac{7}{5} & -\frac{1}{5}
\end{bmatrix}
$


Langkah 7 :$\begin{bmatrix} R_3 \rightarrow -\frac{1}{5}R_3: \end{bmatrix}$



$
\begin{bmatrix}
1 & 0 & 2 & 0 & \frac{3}{5} & -\frac{1}{5} \\
0 & 1 & 0 & 0 & -\frac{1}{5} & \frac{2}{5} \\
0 & 0 & 1 & -\frac{1}{5} & \frac{7}{25} & \frac{1}{25}
\end{bmatrix}



Langkah 8: $\begin{bmatrix} R_1 \rightarrow R_1 - 2R_3 :\end{bmatrix}$



$
\begin{bmatrix}
1 & 0 & 0 & \frac{2}{5} & \frac{1}{25} & -\frac{7}{25} \\
0 & 1 & 0 & 0 & -\frac{1}{5} & \frac{2}{5} \\
0 & 0 & 1 & -\frac{1}{5} & \frac{7}{25} & \frac{1}{25}
\end{bmatrix}
$

4. Matriks Invers \( A^{-1} \):
$
A^{-1} = \begin{bmatrix}
\frac{2}{5} & \frac{1}{25} & -\frac{7}{25} \\
0 & -\frac{1}{5} & \frac{2}{5} \\
-\frac{1}{5} & \frac{7}{25} & \frac{1}{25}
\end{bmatrix}
$

5. Solusi Sistem Persamaan:
$
X = A^{-1} \cdot B = \begin{bmatrix}
\frac{2}{5} & \frac{1}{25} & -\frac{7}{25} \\
0 & -\frac{1}{5} & \frac{2}{5} \\
-\frac{1}{5} & \frac{7}{25} & \frac{1}{25}
\end{bmatrix}
\begin{bmatrix}
3 \\
2 \\
1
\end{bmatrix}
$

Hitung perkalian matriks:
$
\begin{aligned}
x &= \frac{2}{5} \cdot 3 + \frac{1}{25} \cdot 2 - \frac{7}{25} \cdot 1 = \frac{6}{5} + \frac{2}{25} - \frac{7}{25} = 1, \\
y &= 0 \cdot 3 - \frac{1}{5} \cdot 2 + \frac{2}{5} \cdot 1 = 0 - \frac{2}{5} + \frac{2}{5} = 0, \\
z &= -\frac{1}{5} \cdot 3 + \frac{7}{25} \cdot 2 + \frac{1}{25} \cdot 1 = -\frac{3}{5} + \frac{14}{25} + \frac{1}{25} = 0.
\end{aligned}
$

Solusi Akhir:
$
\begin{bmatrix}
{x = 1}, \quad{y = 0}, \quad {z = 0}.
\end{bmatrix}
$
