---
title: Cross Product (Perkalian Silang)

---

# Cross Product (Perkalian Silang)

## Pengertian
Perkalian silang (\textit{cross product}) adalah operasi vektor yang menghasilkan vektor baru yang tegak lurus terhadap kedua vektor asalnya. Perkalian silang hanya berlaku di ruang tiga dimensi ($\mathbb{R}^3$).

Jika diberikan dua vektor:

$$ \mathbf{u} = (u_1, u_2, u_3) $$
$$ \mathbf{v} = (v_1, v_2, v_3) $$

Maka hasil perkalian silangnya adalah:
$\mathbf{u} \times \mathbf{v} = (u_2v_3 - u_3v_2, u_3v_1 - u_1v_3, u_1v_2 - u_2v_1)$

## Solusi Menggunakan Determinan
Perkalian silang dapat dihitung menggunakan determinan matriks berikut:

$$
\mathbf{u} \times \mathbf{v} = \begin{vmatrix}
\mathbf{i} & \mathbf{j} & \mathbf{k} \\
u_1 & u_2 & u_3 \\
v_1 & v_2 & v_3 \\
\end{vmatrix}
$$

Langkah-langkahnya:
 1. Bentuk matriks dengan basis vektor $\mathbf{i}, \mathbf{j}, \mathbf{k}$ di baris pertama.
 2. Baris kedua dan ketiga diisi komponen vektor $\mathbf{u}$ dan $\mathbf{v}$.
 3. Hitung determinan menggunakan ekspansi kofaktor.

Contoh: 
$\mathbf{u} = (1, 2, 3)$
$\mathbf{v} = (4, 5, 6)$

Maka:
$\mathbf{u} \times \mathbf{v} = \begin{vmatrix}
\mathbf{i} & \mathbf{j} & \mathbf{k} \\
1 & 2 & 3 \\
4 & 5 & 6 \\
\end{vmatrix}
= \mathbf{i}(2 \cdot 6 - 3 \cdot 5) - \mathbf{j}(1 \cdot 6 - 3 \cdot 4) + \mathbf{k}(1 \cdot 5 - 2 \cdot 4)$
$= \mathbf{i}(12 - 15) - \mathbf{j}(6 - 12) + \mathbf{k}(5 - 8)$
$= -3\mathbf{i} + 6\mathbf{j} - 3\mathbf{k} = (-3, 6, -3)$

## Sifat-Sifat Perkalian Silang


 1. Anti-komutatif:
    $\mathbf{u} \times \mathbf{v} = -(\mathbf{v} \times \mathbf{u})$
    
 2. Distributif terhadap penjumlahan:
    $\mathbf{u} \times (\mathbf{v} + \mathbf{w}) = \mathbf{u} \times \mathbf{v} + \mathbf{u} \times \mathbf{w}$
    
 3. Perkalian dengan skalar:
    $(k\mathbf{u}) \times \mathbf{v} = k(\mathbf{u} \times \mathbf{v})$
    
 4. Hubungan dengan sudut:
    $\|\mathbf{u} \times \mathbf{v}\| = \|\mathbf{u}\| \|\mathbf{v}\| \sin \theta$
(di mana $\theta$ adalah sudut antara $\mathbf{u}$ dan $\mathbf{v}$)
    
 5. Vektor nol jika paralel:
    $\mathbf{u} \times \mathbf{v} = \mathbf{0} \text{ jika } \mathbf{u} \text{ dan } \mathbf{v} \text{ sejajar}$
    
 6. Tegak lurus terhadap vektor asal:
    $\mathbf{u} \times \mathbf{v} \perp \mathbf{u} \text{ dan } \mathbf{v}$


## Aplikasi Perkalian Silang

1. Menghitung luas jajar genjang dari dua vektor ($\|\mathbf{u} \times \mathbf{v}\|$).
2. Menghitung volume paralelepiped menggunakan triple scalar product :
    $V = |\mathbf{u} \cdot (\mathbf{v} \times \mathbf{w})|$


## Contoh Soal \& Solusi
Soal
Hitung $\mathbf{a} \times \mathbf{b}$ jika $\mathbf{a} = (2, -1, 3)$ dan $\mathbf{b} = (0, 4, -2)$.

Solusi:
$\mathbf{a} \times \mathbf{b} = \begin{vmatrix}
\mathbf{i} & \mathbf{j} & \mathbf{k} \\
2 & -1 & 3 \\
0 & 4 & -2 \\
\end{vmatrix}$
$= \mathbf{i}((-1)(-2) - (3)(4)) - \mathbf{j}((2)(-2) - (3)(0)) + \mathbf{k}((2)(4) - (-1)(0))$
$= \mathbf{i}(2 - 12) - \mathbf{j}(-4 - 0) + \mathbf{k}(8 - 0)$
$= -10\mathbf{i} + 4\mathbf{j} + 8\mathbf{k} = (-10, 4, 8)$

## Kesimpulan
Perkalian silang berguna dalam geometri vektor, fisika (torsi, momentum sudut), dan grafika komputer. Dengan determinan, perhitungannya menjadi sistematis, dan sifat-sifatnya membantu dalam analisis vektor 3D.


# Latihan soal

## 1. Luas Jajaran Genjang (2D)
Diberikan:
Vektor $\mathbf{u} = \begin{bmatrix} 1 \\ 2 \end{bmatrix}$, $\mathbf{v} = \begin{bmatrix} 2 \\ 1 \end{bmatrix}$. 

Rumus Luas:
$\text{Luas} = \left| \det(\mathbf{u}, \mathbf{v}) \right| = \left| u_1 v_2 - u_2 v_1 \right|$

Perhitungan:
$\det(\mathbf{u}, \mathbf{v}) = (1)(1) - (2)(2) = 1 - 4 = -3$

$\text{Luas} = \left| -3 \right| = \boxed{3} \text{ satuan luas}$

## 2. Luas Jajaran Genjang (2D)
Diberikan:
$Vektor \mathbf{u} = \begin{bmatrix} 2 \\ 0 \end{bmatrix}, \mathbf{v} = \begin{bmatrix} 0 \\ 3 \end{bmatrix}.$

Perhitungan:
$\det(\mathbf{u}, \mathbf{v}) = (2)(3) - (0)(0) = 6 - 0 = 6$

$\text{Luas} = \left| 6 \right| = \boxed{6} \text{ satuan luas}$

## 3. Luas Segitiga (3D)
Diberikan:
Titik sudut $A(0,0,0)$, $B(1, 3, -1)$, $C(2, 1, 1)$.

Langkah:
1. Buat vektor $\mathbf{AB}$ dan $\mathbf{AC}$: 
$\mathbf{AB} = B - A = \begin{bmatrix} 1 \\ 3 \\ -1 \end{bmatrix}, \quad \mathbf{AC} = C - A = \begin{bmatrix} 2 \\ 1 \\ 1 \end{bmatrix}$

2. Hitung cross product $\mathbf{AB} \times \mathbf{AC}$:
$\mathbf{AB} \times \mathbf{AC} = 
\begin{vmatrix}
\mathbf{i} & \mathbf{j} & \mathbf{k} \\
1 & 3 & -1 \\
2 & 1 & 1 \\
\end{vmatrix}
= \mathbf{i}(3 \cdot 1 - (-1) \cdot 1) - \mathbf{j}(1 \cdot 1 - (-1) \cdot 2) + \mathbf{k}(1 \cdot 1 - 3 \cdot 2)$

$= \mathbf{i}(3 + 1) - \mathbf{j}(1 + 2) + \mathbf{k}(1 - 6) = 4\mathbf{i} - 3\mathbf{j} - 5\mathbf{k} = \begin{bmatrix} 4 \\ -3 \\ -5 \end{bmatrix}$

3. Hitung norm cross product: \\
$\|\mathbf{AB} \times \mathbf{AC}\| = \sqrt{4^2 + (-3)^2 + (-5)^2} = \sqrt{16 + 9 + 25} = \sqrt{50} = 5\sqrt{2}$

4. Luas segitiga = $\frac{1}{2} \times \|\mathbf{AB} \times \mathbf{AC}\|$:
$\text{Luas} = \frac{1}{2} \times 5\sqrt{2} = \boxed{\frac{5\sqrt{2}}{2}} \text{ satuan luas}$

## 4. Luas Segitiga (3D)
Diberikan:
Titik sudut $P(5, 2, -1)$, $Q(3, 6, 2)$, $R(1, 0, 4)$. 

Langkah:
1. Buat vektor $\mathbf{PQ}$ dan $\mathbf{PR}$:
$\mathbf{PQ} = Q - P = \begin{bmatrix} -2 \\ 4 \\ 3 \end{bmatrix}, \quad \mathbf{PR} = R - P = \begin{bmatrix} -4 \\ -2 \\ 5 \end{bmatrix}$

2. Hitung cross product $\mathbf{PQ} \times \mathbf{PR}$:
$\mathbf{PQ} \times \mathbf{PR} = 
\begin{vmatrix}
\mathbf{i} & \mathbf{j} & \mathbf{k} \\
-2 & 4 & 3 \\
-4 & -2 & 5 \\
\end{vmatrix}
= \mathbf{i}(4 \cdot 5 - 3 \cdot (-2)) - \mathbf{j}(-2 \cdot 5 - 3 \cdot (-4)) + \mathbf{k}(-2 \cdot (-2) - 4 \cdot (-4))$

$= \mathbf{i}(20 + 6) - \mathbf{j}(-10 + 12) + \mathbf{k}(4 + 16) = 26\mathbf{i} - 2\mathbf{j} + 20\mathbf{k} = \begin{bmatrix} 26 \\ -2 \\ 20 \end{bmatrix}$

3. Hitung norm cross product:
$\|\mathbf{PQ} \times \mathbf{PR}\| = \sqrt{26^2 + (-2)^2 + 20^2} = \sqrt{676 + 4 + 400} = \sqrt{1080} = 6\sqrt{30}$

4. Luas segitiga = $\frac{1}{2} \times \|\mathbf{PQ} \times \mathbf{PR}\|$:
$\text{Luas} = \frac{1}{2} \times 6\sqrt{30} = \boxed{3\sqrt{30}} \text{ satuan luas}$
