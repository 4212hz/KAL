---
title: Perkalian Titik (Dot Product)

---

# Perkalian Titik (Dot Product)

## Definisi
Perkalian titik (dot product) adalah operasi aljabar yang mengukur hubungan antara dua vektor. Untuk vektor $\mathbf{v}$ dan $\mathbf{w}$ di ruang dua dimensi, dot product didefinisikan sebagai:
$\mathbf{v} \cdot \mathbf{w} = v_1w_1 + v_2w_2.$
Contoh:
$\begin{bmatrix} 2 \\ -3 \end{bmatrix} \cdot \begin{bmatrix} 4 \\ 1 \end{bmatrix} = 2 \cdot 4 + (-3) \cdot 1 = 5.$



## Geometri dari Hasil Kali Titik
Hasil kali dari dua titik akan menghasilkan sebuah bilangan skalar. Hasil kali titik untuk dua vektor berdimensi $m$ sebagai berikut:

$$
\mathbf{v} \cdot \mathbf{w} = 
\begin{bmatrix}
v_1 \\
v_2 \\
\vdots \\
v_m
\end{bmatrix}
\cdot
\begin{bmatrix}
w_1 \\
w_2 \\
\vdots \\
w_m
\end{bmatrix}
= v_1 w_1 + v_2 w_2 + \cdots + v_m w_m
$$

### Contoh Perhitungan
$$
\mathbf{v} \cdot \mathbf{w} = 
\begin{bmatrix}
2 \\
0 \\
-3 \\
1
\end{bmatrix}
\cdot
\begin{bmatrix}
-1 \\
3 \\
1 \\
2
\end{bmatrix}
= 2(-1) + 0(3) + (-3)(1) + 1(2) = -3
$$

### Contoh Penerapan Dot Product dalam Basis Dua Dimensi
$$
A = \begin{bmatrix}
1 & 0 \\
0 & 1
\end{bmatrix}, \quad
\mathbf{v} = \begin{bmatrix} 1 \\ 0 \end{bmatrix}, \quad
\mathbf{w} = \begin{bmatrix} 0 \\ 1 \end{bmatrix}
$$

$$
\begin{bmatrix} 1 \\ 0 \end{bmatrix} \cdot 
\begin{bmatrix} 0 \\ 1 \end{bmatrix} = 
1 \times 0 + 0 \times 1 = 0
$$ 

### Contoh Lain
$$
A = \begin{bmatrix}
2 & 4 \\
-3 & 1
\end{bmatrix}, \quad
\mathbf{v} = \begin{bmatrix} 2 \\ -3 \end{bmatrix}, \quad
\mathbf{w} = \begin{bmatrix} 4 \\ 1 \end{bmatrix}
$$

$$
\begin{bmatrix} 2 \\ -3 \end{bmatrix} \cdot 
\begin{bmatrix} 4 \\ 1 \end{bmatrix} = 
2 \times 4 + (-3) \times 1 = 5
$$

## Vektor Ortogonal
Jika dua vektor membentuk sudut $90^\circ$, maka dot product-nya nol. Contoh:

$$
\mathbf{v} = \begin{bmatrix} -1 \\ 2 \end{bmatrix}, \quad
\mathbf{u} = \begin{bmatrix} 2 \\ 1 \end{bmatrix}
$$

$$
\mathbf{v} \cdot \mathbf{u} = (-1)(2) + 2(1) = 0
$$

## Perkalian Titik dan Panjang Vektor
Panjang Vektor di $\mathbb{R}^2$}
Panjang vektor $\mathbf{x} = (x,y)$:

$$
\|\mathbf{x}\| = \sqrt{x^2 + y^2}
$$

### Contoh Perhitungan
Untuk $\mathbf{u} = (3,4)$:

$$
\|\mathbf{u}\| = \sqrt{3^2 + 4^2} = \sqrt{9 + 16} = \sqrt{25} = 5
$$


### Contoh Lain
Untuk $\mathbf{v} = (5,12)$:

$$
\|\mathbf{v}\| = \sqrt{5^2 + 12^2} = \sqrt{25 + 144} = \sqrt{169} = 13
$$

## Contoh 3 Dimensi
Untuk vektor $\mathbf{w} = (1,2,2)$:

$$
\|\mathbf{w}\| = \sqrt{1^2 + 2^2 + 2^2} = \sqrt{1 + 4 + 4} = \sqrt{9} = 3
$$



## contoh penerapan Dot Product dalam Basis dua dimensi menggunakan geogebra:

<iframe src="https://www.geogebra.org/classic/ja8x3vuj?embed" width="800" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>


<iframe src="https://www.geogebra.org/classic/aawhgt67?embed" width="800" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>


## Implementasi Geometris
<iframe src="https://www.geogebra.org/classic/j5xmhmxn?embed" width="800" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>