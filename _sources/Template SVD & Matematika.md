---
title: Template SVD & Matematika
tags: [SVD, Linear Algebra, Math, Template]

---

---
title: Penjelasan SVD (Singular Value Decomposition)
tags: [SVD, Aljabar Linear, Data Science]
---

# 📚 Singular Value Decomposition (SVD)

## 🔍 Apa Itu SVD?

*Singular Value Decomposition (SVD)* adalah teknik dekomposisi matriks dalam aljabar linear yang memecah sebuah matriks \( A \) menjadi tiga matriks:

$$
A = U \Sigma V^T
$$

*Penjelasan:*

- \( A \): matriks asli berukuran \( m \times n \)  
- \( U \): matriks ortogonal berukuran \( m \times m \)  
- \( \Sigma \): matriks diagonal berukuran \( m \times n \) dengan nilai singular di diagonal  
- \( V^T \): transpose dari matriks ortogonal \( V \) berukuran \( n \times n \)

---

## Langkah-Langkah Menghitung SVD

Misalkan \( A \) adalah matriks berukuran \( m \times n \), maka langkah-langkahnya:

1. Hitung \( A^T A \)
2. Temukan nilai eigen \( \lambda_i \) dan eigenvektor \( v_i \) dari \( A^T A \)
3. Hitung nilai singular:

   $$
   \sigma_i = \sqrt{\lambda_i}
   $$

4. Hitung vektor \( u_i \) dengan rumus:

   $$
   u_i = \frac{1}{\sigma_i} A v_i
   $$

5. Susun kembali:

   $$
   A = U \Sigma V^T
   $$

---

## Contoh SVD Matriks \( 2 \times 3 \)

Misalkan:

$$
A = \begin{bmatrix}
3 & 1 & 1 \\
-1 & 3 & 1
\end{bmatrix}
$$

### 1. Hitung Transpose \( A^T \):

$$
A^T = \begin{bmatrix}
3 & -1 \\
1 & 3 \\
1 & 1
\end{bmatrix}
$$

### 2. Hitung \( A^T A \):

\begin{bmatrix}
3 & -1 \\
1 & 3 \\
1 & 1
\end{bmatrix}
\begin{bmatrix}
3 & 1 & 1 \\
-1 & 3 & 1
\end{bmatrix}
=
\begin{bmatrix}
10 & 0 & 2 \\
0 & 10 & 6 \\
2 & 6 & 2
\end{bmatrix}


### 3. Hitung nilai eigen dan vektor eigen dari \( A^T A \)

- Temukan \( \lambda_i \), lalu:

  $$
  \sigma_i = \sqrt{\lambda_i}
  $$

### 4. Hitung vektor \( u_i \):

$$
u_i = \frac{1}{\sigma_i} A v_i
$$

### 5. Susun hasil akhir:

$$
A = U \Sigma V^T
$$

> Perhitungan manual ini biasanya dibantu dengan software seperti Python (NumPy), MATLAB, atau kalkulator online.

---

## Kegunaan SVD

- Reduksi Dimensi (PCA)
- Sistem Rekomendasi (Netflix, Spotify)
- Kompresi Gambar
- Analisis Data & Machine Learning
- Penyelesaian sistem persamaan linier & pseudoinverse

---