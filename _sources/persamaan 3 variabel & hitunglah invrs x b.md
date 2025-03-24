---
title: persamaan 3 variabel & hitunglah invrs x b

---

# persamaan 3 variabel & hitunglah invrs x b

## Langkah 1: Membuat Sistem Persamaan Linear
Kita membuat tiga persamaan linear dengan tiga variabel \(x\), \(y\), dan \(z\):

$
\begin{cases}
x + y + z = 1 \quad \text{(Persamaan 1)} \\
2x + 3y + z = 0 \quad \text{(Persamaan 2)} \\
x + 2y + 2z = 0 \quad \text{(Persamaan 3)}
\end{cases}
$

## Langkah 2: Tulis dalam Bentuk Matriks
Sistem persamaan di atas dapat ditulis dalam bentuk matriks \(AX = B\), di mana:
- \(A\) adalah matriks koefisien,
- \(X\) adalah vektor variabel \([x, y, z]^T\),
- \(B\) adalah vektor hasil \([1, 0, 0]^T\).

Matriks \(A\) dan vektor \(B\) adalah:
$
A = \begin{bmatrix}
1 & 1 & 1 \\
2 & 3 & 1 \\
1 & 2 & 2
\end{bmatrix}
$

B = 
$
\begin{bmatrix}
1 \\
0 \\
0
\end{bmatrix}
$

## Langkah 3: Hitung Invers Matriks \(A\)
Invers matriks \(A\) (\(A^{-1}\)) dihitung menggunakan metode eliminasi Gauss-Jordan.

\subsection*{Langkah 3.1: Tulis Matriks Augmented \([A | I]\)}
Gabungkan matriks \(A\) dengan matriks identitas \(I\):
$
[A | I] = \begin{bmatrix}
1 & 1 & 1 & | & 1 & 0 & 0 \\
2 & 3 & 1 & | & 0 & 1 & 0 \\
1 & 2 & 2 & | & 0 & 0 & 1
\end{bmatrix}
$

### Langkah 3.2: Lakukan Operasi Baris Elementer
1. $\textbf{Baris 2 = Baris 2 - 2 \(\times\) Baris 1}:$
   $
   \begin{bmatrix}
   1 & 1 & 1 & | & 1 & 0 & 0 \\
   0 & 1 & -1 & | & -2 & 1 & 0 \\
   1 & 2 & 2 & | & 0 & 0 & 1
   \end{bmatrix}
   $

2. $\textbf{Baris 3 = Baris 3 - Baris 1}:$
   $
   \begin{bmatrix}
   1 & 1 & 1 & | & 1 & 0 & 0 \\
   0 & 1 & -1 & | & -2 & 1 & 0 \\
   0 & 1 & 1 & | & -1 & 0 & 1
   \end{bmatrix}
   $

3. $\textbf{Baris 3 = Baris 3 - Baris 2}:$
   $
   \begin{bmatrix}
   1 & 1 & 1 & | & 1 & 0 & 0 \\
   0 & 1 & -1 & | & -2 & 1 & 0 \\
   0 & 0 & 2 & | & 1 & -1 & 1
   \end{bmatrix}
   $

4. $\textbf{Baris 3 = Baris 3 / 2}:$
   $
   \begin{bmatrix}
   1 & 1 & 1 & | & 1 & 0 & 0 \\
   0 & 1 & -1 & | & -2 & 1 & 0 \\
   0 & 0 & 1 & | & 0.5 & -0.5 & 0.5
   \end{bmatrix}
   $

5. $\textbf{Baris 2 = Baris 2 + Baris 3}:$
   $
   \begin{bmatrix}
   1 & 1 & 1 & | & 1 & 0 & 0 \\
   0 & 1 & 0 & | & -1.5 & 0.5 & 0.5 \\
   0 & 0 & 1 & | & 0.5 & -0.5 & 0.5
   \end{bmatrix}
   $

6. $\textbf{Baris 1 = Baris 1 - Baris 2 - Baris 3}:$
   $
   \begin{bmatrix}
   1 & 0 & 0 & | & 2 & 0 & -1 \\
   0 & 1 & 0 & | & -1.5 & 0.5 & 0.5 \\
   0 & 0 & 1 & | & 0.5 & -0.5 & 0.5
   \end{bmatrix}
   $

### Langkah 3.3: Tulis Invers Matriks \(A^{-1}\)
Setelah operasi baris elementer, matriks di sebelah kanan adalah invers matriks \(A\):
$
A^{-1} = \begin{bmatrix}
2 & 0 & -1 \\
-1.5 & 0.5 & 0.5 \\
0.5 & -0.5 & 0.5
\end{bmatrix}
$

## Langkah 4: Hitung Solusi \(X = A^{-1}B\)
Untuk mendapatkan solusi \(X\), kita kalikan \(A^{-1}\) dengan \(B\):
$
X = A^{-1}B = \begin{bmatrix}
2 & 0 & -1 \\
-1.5 & 0.5 & 0.5 \\
0.5 & -0.5 & 0.5
\end{bmatrix}
\begin{bmatrix}
1 \\
0 \\
0
\end{bmatrix}
$

Perhitungannya:
$
X = \begin{bmatrix}
2 \cdot 1 + 0 \cdot 0 + (-1) \cdot 0 \\
-1.5 \cdot 1 + 0.5 \cdot 0 + 0.5 \cdot 0 \\
0.5 \cdot 1 + (-0.5) \cdot 0 + 0.5 \cdot 0
\end{bmatrix}
= \begin{bmatrix}
2 \\
-1.5 \\
0.5
\end{bmatrix}
$

## Hasil
Solusi dari sistem persamaan adalah:
$
\begin{bmatrix}
x = 2, \quad y = -1.5, \quad z = 0.5
\end{bmatrix}
$

### Catatan
Jika ingin hasil perkalian \(A^{-1}B\) adalah \([1, 0, 0]^T\), dapat memodifikasi vektor \(B\) sebagai berikut:

$
\begin{bmatrix} B = A \cdot \end{bmatrix}
\begin{bmatrix}
1 \\
0 \\
0
\end{bmatrix}
$
Dengan demikian, \(B\) akan menjadi:
$
B = \begin{bmatrix}
1 & 1 & 1 \\
2 & 3 & 1 \\
1 & 2 & 2
\end{bmatrix}
\begin{bmatrix}
1 \\
0 \\
0
\end{bmatrix}
= \begin{bmatrix}
1 \\
2 \\
1
\end{bmatrix}
$


Kemudian, hitung \(X = A^{-1}B\):

$
X = A^{-1}B = \begin{bmatrix}
2 & 0 & -1 \\
-1.5 & 0.5 & 0.5 \\
0.5 & -0.5 & 0.5
\end{bmatrix}
\begin{bmatrix}
1 \\
2 \\
1
\end{bmatrix}
= \begin{bmatrix}
1 \\
0 \\
0
\end{bmatrix}
$

Hasilnya adalah \([1, 0, 0]^T\), sesuai dengan yang diinginkan.
