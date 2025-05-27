# Mencatat Materi Dot Product

**Dot product** atau **perkalian titik** adalah operasi matematika yang mengalikan dua vektor dan menghasilkan sebuah nilai skalar. Operasi ini sangat penting dalam berbagai bidang ilmu seperti fisika, matematika, grafika komputer, dan machine learning karena mampu menggambarkan hubungan sudut dan proyeksi antar vektor.

---

## Pengertian Dot Product

Misalkan terdapat dua vektor \(\mathbf{A} = (A_x, A_y, A_z)\) dan \(\mathbf{B} = (B_x, B_y, B_z)\) dalam ruang 3 dimensi. Dot product didefinisikan sebagai:

\[
\mathbf{A} \cdot \mathbf{B} = A_x B_x + A_y B_y + A_z B_z
\]

Jika vektor berada di ruang 2 dimensi, maka rumusnya cukup:

\[
\mathbf{A} \cdot \mathbf{B} = A_x B_x + A_y B_y
\]

Secara geometris, dot product dapat dihitung dengan:

\[
\mathbf{A} \cdot \mathbf{B} = |\mathbf{A}| \times |\mathbf{B}| \times \cos \theta
\]

Dimana:  
- \(|\mathbf{A}|\) dan \(|\mathbf{B}|\) adalah panjang atau *magnitude* vektor \(\mathbf{A}\) dan \(\mathbf{B}\)  
- \(\theta\) adalah sudut antara kedua vektor

Rumus ini memberikan cara untuk menghubungkan operasi aljabar komponen dengan interpretasi geometris berupa sudut antara vektor.

---

## Interpretasi Geometris Dot Product

Dot product mengukur **sejauh mana dua vektor "searah"** atau komponen satu vektor dalam arah vektor lain.  

- Jika \(\mathbf{A} \cdot \mathbf{B} > 0\), berarti sudut antara vektor kurang dari 90°, sehingga vektor cenderung searah.  
- Jika \(\mathbf{A} \cdot \mathbf{B} = 0\), maka vektor saling tegak lurus atau ortogonal, tidak ada komponen proyeksi yang sama.  
- Jika \(\mathbf{A} \cdot \mathbf{B} < 0\), maka sudut antara vektor lebih dari 90°, sehingga vektor berlawanan arah.

Interpretasi ini sangat berguna untuk analisis arah dan hubungan antar vektor dalam ruang.

---

## Properti Penting Dot Product

Dot product memiliki beberapa sifat penting yang mempermudah perhitungan dan analisis vektor:

1. **Komutatif**  
   \[
   \mathbf{A} \cdot \mathbf{B} = \mathbf{B} \cdot \mathbf{A}
   \]  
   Urutan vektor tidak mempengaruhi hasil.

2. **Distributif terhadap penjumlahan**  
   \[
   \mathbf{A} \cdot (\mathbf{B} + \mathbf{C}) = \mathbf{A} \cdot \mathbf{B} + \mathbf{A} \cdot \mathbf{C}
   \]

3. **Hasil dot product dengan diri sendiri**  
   \[
   \mathbf{A} \cdot \mathbf{A} = |\mathbf{A}|^2
   \]  
   Hasil ini sama dengan kuadrat panjang vektor \(\mathbf{A}\).

4. **Bersifat bilinear dan skalar**  
   Dot product menghasilkan nilai skalar, bukan vektor.

---

## Hubungan dengan Proyeksi Vektor

Dot product juga berguna untuk menghitung **proyeksi vektor** \(\mathbf{A}\) pada \(\mathbf{B}\). Proyeksi ini menunjukkan seberapa besar \(\mathbf{A}\) "terlempar" ke arah \(\mathbf{B}\), dan rumusnya:

\[
\text{proj}_{\mathbf{B}} \mathbf{A} = \frac{\mathbf{A} \cdot \mathbf{B}}{|\mathbf{B}|}
\]

Nilai ini memberikan panjang bayangan \(\mathbf{A}\) jika diproyeksikan ke arah \(\mathbf{B}\).

---

## Contoh Perhitungan Dot Product dan Sudut Antar Vektor

Misalnya dua vektor 2D:  
\[
\mathbf{A} = (3, 4), \quad \mathbf{B} = (2, 1)
\]

Perhitungan dot product:  
\[
\mathbf{A} \cdot \mathbf{B} = 3 \times 2 + 4 \times 1 = 10
\]

Panjang vektor:  
\[
|\mathbf{A}| = \sqrt{3^2 + 4^2} = 5, \quad |\mathbf{B}| = \sqrt{2^2 + 1^2} = \sqrt{5}
\]

Sudut antara vektor:  
\[
\cos \theta = \frac{10}{5 \times \sqrt{5}} = \frac{2}{\sqrt{5}} \approx 0.894
\]  
\[
\theta = \cos^{-1}(0.894) \approx 26.57^\circ
\]

Proyeksi \(\mathbf{A}\) pada \(\mathbf{B}\):  
\[
\text{proj}_{\mathbf{B}} \mathbf{A} = \frac{10}{\sqrt{5}} \approx 4.47
\]

---

## Contoh Kode Python untuk Menghitung Dot Product

```python
import numpy as np

# Mendefinisikan dua vektor
A = np.array([3, 4])
B = np.array([2, 1])

# Hitung dot product
dot_product = np.dot(A, B)
print("Dot product A · B:", dot_product)

# Hitung panjang vektor
magnitude_A = np.linalg.norm(A)
magnitude_B = np.linalg.norm(B)

# Hitung sudut dalam radian dan derajat
cos_theta = dot_product / (magnitude_A * magnitude_B)
theta_rad = np.arccos(cos_theta)
theta_deg = np.degrees(theta_rad)

print(f"Sudut antara A dan B: {theta_deg:.2f} derajat")
