---
title: SVD

---

# Singular Value Decomposition (SVD)
## Pengertian
Singular Value Decomposition) adalah teknik faktorisasi matriks yang menyatakan suatu matriks $A$ menjadi hasil perkalian tiga matriks:

$A = U \Sigma V^T$

Dengan:

$A$: matriks asli berukuran $m n$
$U$: matriks ortogonal berukuran $m m$ (vektor singular kiri)
$\Sigma$: matriks diagonal berukuran $m n$ dengan nilai singular pada diagonal utama
$V^T$: transpose dari matriks ortogonal $V$ berukuran $n n$ 

Properti Penting SVD

Nilai singular $\sigma_1 \geq \sigma_2 \geq \dots \geq \sigma_r > 0$ selalu non-negatif
Rank matriks $A$ sama dengan jumlah nilai singular tak-nol
Norma Frobenius $\|A\|_F = \sqrt{\sum \sigma_i^2}$
Norma spektral $\|A\|_2 = \sigma_1$

# Kegunaan SVD
1. Reduksi Dimensi (Dimensionality Reduction)
    * Digunakan dalam PCA (Principal Component Analysis)
2. Sistem Rekomendasi (Recommendation Systems)
    * Memfaktorkan matriks rating user-item
3. Pemrosesan Gambar (Image Processing)
    * Kompresi gambar dengan memotong nilai singular kecil
4. Pemrosesan Bahasa Alami (NLP)
    * LSA (Latent Semantic Analysis) untuk analisis dokumen
5. Penyelesaian Persamaan Linear (Linear Systems)
    * Menyelesaikan sistem under/over-determined
6. Analisis Jaringan (Network Analysis)
    * Deteksi komunitas dalam graf sosial



# Contoh Perhitungan SVD
Diberikan matriks:
$A = \begin{bmatrix} 2 & 0 \\ 0 & 3 \\ 1 & 1 \end{bmatrix}$

Langkah 1: Hitung $A^TA$
$A^TA = \begin{bmatrix} 5 & 1 \\ 1 & 10 \end{bmatrix}$

Langkah 2: Cari Nilai Eigen
Persamaan karakteristik:
$\det(A^TA - \lambda I) = \lambda^2 - 15\lambda + 49 = 0$
Solusi:
$\lambda_1 \approx 11.19, \quad \lambda_2 \approx 3.81$

Langkah 3: Nilai Singular
$\sigma_1 = \sqrt{11.19} \approx 3.35, \quad \sigma_2 = \sqrt{3.81} \approx 1.95$

Langkah 4: Matriks $V$
Vektor eigen ternormalisasi:
$V \approx \begin{bmatrix} 0.19 & -0.98 \\ 0.98 & 0.19 \end{bmatrix}$

Langkah 5: Matriks $U$
$U \approx \begin{bmatrix} 0.11 & -1.01 \\ 0.88 & 0.29 \\ 0.35 & -0.41 \end{bmatrix}$


# Contoh 2: 
SVD Matriks $A = \begin{bmatrix} 1 & 2 \\ 3 & 4 \\ 5 & 6 \end{bmatrix}$

Langkah 1: Hitung $A^TA$
$A^TA = \begin{bmatrix} 1 & 3 & 5 \\ 2 & 4 & 6 \end{bmatrix}
\begin{bmatrix} 1 & 2 \\ 3 & 4 \\ 5 & 6 \end{bmatrix} 
= \begin{bmatrix} 35 & 44 \\ 44 & 56 \end{bmatrix}$


Langkah 2: Cari nilai eigen $\lambda$ dari $A^TA$
$\det(A^TA - \lambda I) = \begin{vmatrix}
35 - \lambda & 44 \\
44 & 56 - \lambda
\end{vmatrix} = 0$

$(35 - \lambda)(56 - \lambda) - 44^2 = 0$
$\lambda^2 - 91\lambda + 1960 - 1936 = 0$
$\lambda^2 - 91\lambda + 24 = 0$
$\lambda = \frac{91 \pm \sqrt{8281 - 96}}{2} = \frac{91 \pm \sqrt{8185}}{2}$
$\lambda_1 \approx 90.27, \quad \lambda_2 \approx 0.73$

Langkah 3: Hitung nilai singular
$\sigma_1 = \sqrt{90.27} \approx 9.50, \quad \sigma_2 = \sqrt{0.73} \approx 0.85$
$\Sigma = \begin{bmatrix}
9.50 & 0 \\
0 & 0.85 \\
0 & 0
\end{bmatrix}$

Langkah 4: Cari vektor eigen untuk $V$
Untuk $\lambda_1 \approx 90.27$:
$(A^TA - 90.27I)\mathbf{v} = \begin{bmatrix}
-55.27 & 44 \\
44 & -34.27
\end{bmatrix}\mathbf{v} = 0$

Solusi: $v_1 \approx \begin{bmatrix} 0.62 \\ 0.78 \end{bmatrix}$ (ternormalisasi)

Untuk $\lambda_2 \approx 0.73$:
$(A^TA - 0.73I)\mathbf{v} = \begin{bmatrix}
34.27 & 44 \\
44 & 55.27
\end{bmatrix}\mathbf{v} = 0$

Solusi: $v_2 \approx \begin{bmatrix} -0.78 \\ 0.62 \end{bmatrix}$ (ternormalisasi)

$V \approx \begin{bmatrix}
0.62 & -0.78 \\
0.78 & 0.62
\end{bmatrix}$


Langkah 5: Hitung matriks $U$
$u_1 = \frac{1}{\sigma_1}A v_1 \approx \frac{1}{9.50}\begin{bmatrix} 1 & 2 \\ 3 & 4 \\ 5 & 6 \end{bmatrix}
\begin{bmatrix} 0.62 \\ 0.78 \end{bmatrix} \approx \begin{bmatrix} 0.23 \\ 0.52 \\ 0.82 \end{bmatrix}$


$u_2 = \frac{1}{\sigma_2}A v_2 \approx \frac{1}{0.85}\begin{bmatrix} 1 & 2 \\ 3 & 4 \\ 5 & 6 \end{bmatrix}
\begin{bmatrix} -0.78 \\ 0.62 \end{bmatrix} \approx \begin{bmatrix} 0.54 \\ -0.83 \\ 0.12 \end{bmatrix}$

Kolom ketiga $U$ dapat dicari dengan Gram-Schmidt:
$U \approx \begin{bmatrix}
0.23 & 0.54 & -0.81 \\
0.52 & -0.83 & -0.19 \\
0.82 & 0.12 & 0.56
\end{bmatrix}$

Hasil Akhir SVD
$A \approx U \Sigma V^T \approx \begin{bmatrix}
0.23 & 0.54 & -0.81 \\
0.52 & -0.83 & -0.19 \\
0.82 & 0.12 & 0.56
\end{bmatrix}
\begin{bmatrix}
9.50 & 0 \\
0 & 0.85 \\
0 & 0
\end{bmatrix}
\begin{bmatrix}
0.62 & 0.78 \\
-0.78 & 0.62
\end{bmatrix}$

