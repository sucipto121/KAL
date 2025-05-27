# Perkalian Titik (Dot Product)

## Oleh : Sucipto Budiono


Dalam bagian ini, kita memperkenalkan operasi aljabar sederhana yang dikenal sebagai **hasil kali titik (dot product)**, yang membantu kita mengukur panjang vektor dan sudut yang dibentuk oleh sepasang vektor. Untuk vektor-vektor dua dimensi **v** dan **w**, hasil kali titik  (**v · w**) didefinisikan sebagai bilangan skalar berikut:

$$
\mathbf{v} \cdot \mathbf{w} = 
\begin{bmatrix}
v_1 \\
v_2
\end{bmatrix}
\cdot
\begin{bmatrix}
w_1 \\
w_2
\end{bmatrix}
= v_1w_1 + v_2w_2.
$$

Sebagai contoh,

$$
\begin{bmatrix}
2 \\
-3
\end{bmatrix}
\cdot
\begin{bmatrix}
4 \\
1
\end{bmatrix}
= 2 \cdot 4 + (-3) \cdot 1 = 5.
$$

### Latihan hasil kali titik
a. Hitung 
$$
\begin{bmatrix}
3 \\
4
\end{bmatrix}
\cdot
\begin{bmatrix}
2 \\
-2
\end{bmatrix}.
$$

b. Gambarkan vektor $\mathbf{v} = \begin{bmatrix} 3 \\ 4 \end{bmatrix}$ di bawah ini. Kemudian gunakan teorema Pythagoras untuk menentukan panjang dari $\mathbf{v}$.

![image](https://hackmd.io/_uploads/B17MWWxfgg.png)


### Latihan Soal

a. Hitung hasil kali titik $\mathbf{v} \cdot \mathbf{v}$. Bagaimana hubungan antara hasil kali titik ini dengan panjang vektor $\mathbf{v}$?

b. Ingat bahwa matriks $\begin{bmatrix} 0 & -1 \\ 1 & 0 \end{bmatrix}$ merepresentasikan transformasi matriks yang melakukan rotasi vektor sebesar $90^\circ$ berlawanan arah jarum jam. Mulailah dengan vektor $\mathbf{v} = \begin{bmatrix} 3 \\ 4 \end{bmatrix}$, temukan vektor $\mathbf{w}$, yaitu hasil rotasi $\mathbf{v}$ sebesar $90^\circ$, dan gambarkan di atas.

c. Berapakah nilai hasil kali titik $\mathbf{v} \cdot \mathbf{w}$?

d. Misalkan $\mathbf{v} = \begin{bmatrix} a \\ b \end{bmatrix}$, buatlah a,b nilai sembarang. Temukan vektor $\mathbf{w}$ yang dihasilkan dari rotasi $\mathbf{v}$ sebesar $90^\circ$, lalu hitung hasil kali titik $\mathbf{v} \cdot \mathbf{w}$.

e. Misalkan $\mathbf{v}$ dan $\mathbf{w}$ adalah dua vektor yang saling tegak lurus. Menurut Anda, berapa nilai hasil kali titik $\mathbf{v} \cdot \mathbf{w}$?

## Geometri dari Hasil Kali Titik

Hasil kali titik didefinisikan, secara umum, untuk dua vektor berdimensi $m$ sebagai berikut:

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
= v_1w_1 + v_2w_2 + \ldots + v_mw_m.
$$

Hal penting yang perlu diingat adalah bahwa hasil kali titik akan menghasilkan sebuah bilangan skalar. Dengan kata lain, kedua vektor digabungkan dalam cara tertentu sehingga menghasilkan sebuah nilai, dan seperti yang akan kita lihat, angka ini memberikan informasi geometris .

### Contoh 

Kita menghitung hasil kali titik antara dua vektor berdimensi empat sebagai berikut:

$$
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
= 2(-1) + 0(3) + (-3)(1) + 1(2) = -3.
$$

 Sifat-sifat Hasil Kali Titik



## **Sifat-sifat Pertama Pekalian Titik**

Misalkan $\mathbf{x}, \mathbf{y}$, dan $\mathbf{u}$ adalah vektor-vektor di ruang vektor $\mathbb{R}^n$, dan misalkan $r$ adalah sebuah skalar. Maka berlaku sifat-sifat berikut:

1. **Komutatif**:  
   $$
   \mathbf{x} \cdot \mathbf{y} = \mathbf{y} \cdot \mathbf{x}
   $$

2. **Distributif terhadap Penjumlahan Vektor**:  
   $$
   \mathbf{u} \cdot (\mathbf{x} + \mathbf{y}) = \mathbf{u} \cdot \mathbf{x} + \mathbf{u} \cdot \mathbf{y}
   $$

3. **Distributif terhadap Penjumlahan Vektor (dari sisi kiri)**:  
   $$
   (\mathbf{x} + \mathbf{y}) \cdot \mathbf{u} = \mathbf{x} \cdot \mathbf{u} + \mathbf{y} \cdot \mathbf{u}
   $$

4. **Homogenitas Skalar**:  
   $$
   r(\mathbf{x} \cdot \mathbf{y}) = (r\mathbf{x}) \cdot \mathbf{y} = \mathbf{x} \cdot (r\mathbf{y})
   $$

5. **Positif Semidefinisi**:  
   $$
   \mathbf{x} \cdot \mathbf{x} \geq 0
   $$
   dengan kesamaan terjadi jika dan hanya jika $\mathbf{x} = \mathbf{0}$.

---

### Penjelasan 
1. **Komutatif**: Hasil kali titik dua vektor tidak bergantung pada urutan.
2. **Distributif**: Hasil kali titik distributif terhadap penjumlahan vektor.
3. **Homogenitas Skalar**: Mengalikan salah satu vektor dengan skalar sebelum atau setelah hasil kali titik memberikan hasil yang sama.
4. **Positif Semidefinisi**: Hasil kali titik suatu vektor dengan dirinya sendiri selalu non-negatif, dan bernilai nol hanya jika vektor tersebut adalah vektor nol.

---

### Contoh Praktis:
Misalkan:
$$
\mathbf{x} = \begin{bmatrix} 1 \\ 2 \end{bmatrix}, \quad \mathbf{y} = \begin{bmatrix} 3 \\ -1 \end{bmatrix}, \quad \mathbf{u} = \begin{bmatrix} 2 \\ 1 \end{bmatrix}, \quad r = 2
$$

#### 1. Komutatif:
$$
\mathbf{x} \cdot \mathbf{y} = \begin{bmatrix} 1 \\ 2 \end{bmatrix} \cdot \begin{bmatrix} 3 \\ -1 \end{bmatrix} = (1)(3) + (2)(-1) = 3 - 2 = 1
$$
$$
\mathbf{y} \cdot \mathbf{x} = \begin{bmatrix} 3 \\ -1 \end{bmatrix} \cdot \begin{bmatrix} 1 \\ 2 \end{bmatrix} = (3)(1) + (-1)(2) = 3 - 2 = 1
$$

#### 2. Distributif:
$$
\mathbf{u} \cdot (\mathbf{x} + \mathbf{y}) = \begin{bmatrix} 2 \\ 1 \end{bmatrix} \cdot \left( \begin{bmatrix} 1 \\ 2 \end{bmatrix} + \begin{bmatrix} 3 \\ -1 \end{bmatrix} \right) = \begin{bmatrix} 2 \\ 1 \end{bmatrix} \cdot \begin{bmatrix} 4 \\ 1 \end{bmatrix} = (2)(4) + (1)(1) = 8 + 1 = 9
$$
$$
\mathbf{u} \cdot \mathbf{x} + \mathbf{u} \cdot \mathbf{y} = \begin{bmatrix} 2 \\ 1 \end{bmatrix} \cdot \begin{bmatrix} 1 \\ 2 \end{bmatrix} + \begin{bmatrix} 2 \\ 1 \end{bmatrix} \cdot \begin{bmatrix} 3 \\ -1 \end{bmatrix} = (2)(1) + (1)(2) + (2)(3) + (1)(-1) = 2 + 2 + 6 - 1 = 9
$$

#### 3. Homogenitas Skalar:
$$
r(\mathbf{x} \cdot \mathbf{y}) = 2 \cdot 1 = 2
$$
$$
(r\mathbf{x}) \cdot \mathbf{y} = \begin{bmatrix} 2 \\ 4 \end{bmatrix} \cdot \begin{bmatrix} 3 \\ -1 \end{bmatrix} = (2)(3) + (4)(-1) = 6 - 4 = 2
$$
$$
\mathbf{x} \cdot (r\mathbf{y}) = \begin{bmatrix} 1 \\ 2 \end{bmatrix} \cdot \begin{bmatrix} 6 \\ -2 \end{bmatrix} = (1)(6) + (2)(-2) = 6 - 4 = 2
$$

#### 4. Positif Semidefinisi:
$$
\mathbf{x} \cdot \mathbf{x} = \begin{bmatrix} 1 \\ 2 \end{bmatrix} \cdot \begin{bmatrix} 1 \\ 2 \end{bmatrix} = (1)(1) + (2)(2) = 1 + 4 = 5 \geq 0
$$



Berikut adalah **terjemahan dan konversi ke format Markdown** dari teks yang kamu berikan:

---

## Perkalian titik dan Panjang Vektor



### Panjang Vektor di $\mathbb{R}^2$

1. **Panjang Vektor di $\mathbb{R}^2$:**
   - Dalam ruang vektor dua dimensi ($\mathbb{R}^2$), panjang vektor $\mathbf{x} = (x, y)$ didefinisikan sebagai jarak dari titik asal $(0, 0)$.
   - Jarak ini dihitung menggunakan **Teorema Pythagoras**, yang menyatakan bahwa:
     $$
     \text{Panjang vektor } \mathbf{x} = \sqrt{x^2 + y^2}.
     $$

2. **Interpretasi Geometris:**
   - Vektor $\mathbf{x} = (x, y)$ dapat diwakili oleh garis lurus dari titik asal $(0, 0)$ hingga titik $(x, y)$.
   - Panjang vektor ini adalah hipotenusa segitiga siku-siku dengan kaki-kakinya sepanjang $x$ dan $y$.
   - Di $\mathbb{R}^2$, panjang vektor adalah jaraknya ke titik asal, sehingga untuk vektor $\mathbf{x} = (x, y)$, Teorema Pythagoras digunakan untuk menghitung jarak:

$$
d = \sqrt{x^2 + y^2}.
$$

![image](https://hackmd.io/_uploads/S17Egz-Gxl.png)

3. **Contoh:**
   Misalkan kita memiliki vektor $\mathbf{x} = (3, 4)$. Maka panjangnya adalah:
   $$
   |\mathbf{x}| = \sqrt{3^2 + 4^2} = \sqrt{9 + 16} = \sqrt{25} = 5.
   $$

---


- **Panjang vektor** juga disebut **norma Euclidean** atau **norma 2**.


Dengan cara sama di $\mathbb{R}^3$. Seperti di $\mathbb{R}^2$, kita mendapatkan $d' = \sqrt{x^2 + y^2}$. Dengan menerapkan Teorema Pythagoras sekali lagi, kita mendapatkan $d^2 = d'^2 + z^2$, yang memberikan panjang dalam $\mathbb{R}^3$.

---


### Panjang Vektor di $\mathbb{R}^3$

1. **Panjang Vektor di $\mathbb{R}^3$:**
   - Di ruang vektor tiga dimensi ($\mathbb{R}^3$), panjang vektor $\mathbf{x} = (x, y, z)$ dapat dihitung dengan menggunakan **Teorema Pythagoras** secara bertahap.
   - Pertama, hitung proyeksi vektor pada bidang $xy$:
     $$
     d' = \sqrt{x^2 + y^2}
     $$
   - Kemudian, gunakan hasil ini untuk menghitung panjang total vektor di $\mathbb{R}^3$:
     $$
     d^2 = d'^2 + z^2 = (\sqrt{x^2 + y^2})^2 + z^2 = x^2 + y^2 + z^2
     $$

2. **Interpretasi Geometris:**
   - Vektor $\mathbf{x} = (x, y, z)$ dapat diwakili oleh garis lurus dari titik asal $(0, 0, 0)$ hingga titik $(x, y, z)$.
   - Panjang vektor ini adalah hipotenusa segitiga siku-siku dalam ruang tiga dimensi.


![image](https://hackmd.io/_uploads/BJ7FmfWfxx.png)




3. **Contoh:**
   Misalkan kita memiliki vektor $\mathbf{x} = (3, 4, 5)$. Maka panjangnya adalah:
   $$
   |\mathbf{x}| = \sqrt{3^2 + 4^2 + 5^2} = \sqrt{9 + 16 + 25} = \sqrt{50} = 5\sqrt{2}.
   $$



- Rumus ini dapat diperluas ke ruang vektor berdimensi lebih tinggi ($\mathbb{R}^n$):
  $$
  \|\mathbf{x}\| = \sqrt{x_1^2 + x_2^2 + \cdots + x_n^2}.
  $$

---



Sifat penting dari hasil kali titik adalah dapat memberikan informasi geometris tentang vektor-vektor dan hubungannya satu sama lain. Perhatikan panjang suatu vektor $\mathbf{v} = \begin{bmatrix} 3 \\ 2 \end{bmatrix}$ seperti yang ditunjukkan dalam berikut

![image](https://hackmd.io/_uploads/SkjpQWgMlg.png)

**Gambar** Vektor $\mathbf{v} = \begin{bmatrix} 3 \\ 2 \end{bmatrix}$.

Kita dapat menemukan panjang vektor ini menggunakan teorema Pythagoras, karena vektor tersebut membentuk sisi miring segitiga siku-siku dengan kaki horizontal sepanjang 3 dan kaki vertikal sepanjang 2. Panjang vektor $\mathbf{v}$, yang kita notasikan sebagai $|\mathbf{v}|$, adalah

$$
|\mathbf{v}| = \sqrt{3^2 + 2^2} = \sqrt{13}.
$$

Sehingga hasil kali titik vektor $\mathbf{v}$ dengan dirinya sendiri adalah

$$
\mathbf{v} \cdot \mathbf{v} = 3(3) + 2(2) = 13 = |\mathbf{v}|^2.
$$

Sehingga didapatkan

$$
\mathbf{v} \cdot \mathbf{v} = |\mathbf{v}|^2.
$$

Oleh karena itu  hasil kali titik dua vektor memberikan informasi tentang sudut antara keduanya. Perhatikan **gambar berikut**

![image](https://hackmd.io/_uploads/HyV_zilGge.png)



---

 Gambar Perkalian titik $\mathbf{v} \cdot \mathbf{w}$ mengukur sudut $\theta$.

Untuk memahami ini, kita akan menerapkan **Hukum Cosinus**, yang menyatakan bahwa

$$
|\mathbf{w} - \mathbf{v}|^2 = |\mathbf{v}|^2 + |\mathbf{w}|^2 - 2|\mathbf{v}||\mathbf{w}|\cos\theta
$$

$$
(\mathbf{w} - \mathbf{v}) \cdot (\mathbf{w} - \mathbf{v}) = \mathbf{v} \cdot \mathbf{v} + \mathbf{w} \cdot \mathbf{w} - 2|\mathbf{v}||\mathbf{w}|\cos\theta
$$

$$
\mathbf{w} \cdot \mathbf{w} + \mathbf{v} \cdot \mathbf{v} - 2\mathbf{v} \cdot \mathbf{w} = \mathbf{v} \cdot \mathbf{v} + \mathbf{w} \cdot \mathbf{w} - 2|\mathbf{v}||\mathbf{w}|\cos\theta
$$

$$
-2\mathbf{v} \cdot \mathbf{w} = -2|\mathbf{v}||\mathbf{w}|\cos\theta
$$

$$
\mathbf{v} \cdot \mathbf{w} = |\mathbf{v}||\mathbf{w}|\cos\theta
$$

Oleh karena itu kita dapatkan 


$$
\mathbf{v} \cdot \mathbf{w} = |\mathbf{v}||\mathbf{w}|\cos\theta.
$$

Keimpulannya :

### Sifat Geometris dari perkalian titik (Dot Product)

Perkalian titik memberikan informasi geometris berikut:

$\mathbf{v} \cdot \mathbf{v} = |\mathbf{v}|^2$

$\mathbf{v} \cdot \mathbf{w} = |\mathbf{v}| |\mathbf{w}| \cos \theta$

di mana $\theta$ adalah sudut antara vektor $\mathbf{v}$ dan $\mathbf{w}$.

---

### Latihan 1

**a.** Gambarkan vektor $\mathbf{v} = \begin{bmatrix} 3 \\ 2 \end{bmatrix}$ dan $\mathbf{w} = \begin{bmatrix} -1 \\ 3 \end{bmatrix}$ menggunakan bidang gambar berikut

---

![image](https://hackmd.io/_uploads/SJ_lHjgGel.png)

 
 

---

### Latihan 2

**a.** Hitung panjang $|\mathbf{v}|$ dan $|\mathbf{w}|$ menggunakan hasil klai titik (**dot product**).

**b.** Hitung dot product $\mathbf{v} \cdot \mathbf{w}$ dan gunakan untuk mencari sudut antara $\mathbf{v}$ dan $\mathbf{w}$.

**c.** Perhatikan vektor $\mathbf{x} = \begin{bmatrix} -2 \\ 3 \end{bmatrix}$. Sertakan dalam gambar Anda di Gambar latihan 1 dan cari sudut antara $\mathbf{v}$ dan $\mathbf{x}$.

**d.** Jika dua vektor saling tegak lurus, apa yang bisa Anda katakan tentang dot product-nya? Jelaskan.

**d.** Untuk nilai $k$ berapakah vektor $\begin{bmatrix} 6 \\ k \end{bmatrix}$ agar tegak lurus terhadap $\mathbf{w}$?



###  Sifat Ortogonalitas Vektor

Jika  vektor $\mathbf{v}$ dan $\mathbf{w}$ saling tegak lurus, sudut di antara keduanya $\theta = 90^\circ$ dan kita dapatkan:

$$
\mathbf{v} \cdot \mathbf{w} = |\mathbf{v}| |\mathbf{w}| \cos \theta = |\mathbf{v}| |\mathbf{w}| \cos 90^\circ = 0.
$$

Oleh karena itu, dot product antara vektor-vektor yang tegak lurus harus bernilai nol. Hal ini mengarah pada definisi berikut.

**Definisi**:  Vektor $\mathbf{v}$ dan $\mathbf{w}$ adalah **ortogonal** jika $\mathbf{v} \cdot \mathbf{w} = 0$.



---


Kita telah melihat bahwa dot product memberikan informasi geometris tentang vektor. Operasi ini juga memberikan cara untuk membandingkan vektor. 

**Contoh:**  
Perhatikan vektor-vektor $\mathbf{u}$, $\mathbf{v}$, dan $\mathbf{w}$ yang ditunjukkan pada gambar berikut.

![image](https://hackmd.io/_uploads/H1cFPiezel.png)

- Vektor $\mathbf{v}$ dan $\mathbf{w}$ terlihat cukup mirip karena arah yang mereka tentukan hampir sama.  
- Sebaliknya, $\mathbf{u}$ tampak cukup berbeda dengan kedua vektor $\mathbf{v}$ dan $\mathbf{w}$.

**Pengukuran Kesamaan Vektor:**  
Kesamaan antara vektor akan diukur dengan mencari sudut di antara mereka:

$$
\text{Semakin kecil sudut} \rightarrow \text{Semakin mirip vektor-vektor tersebut}
$$


##  Vektor Satuan di $\mathbb{R}^n$

Vektor satuan (unit vector) adalah vektor dengan panjang satu.

Jelas bahwa vektor $\mathbf{x}$ adalah vektor satuan jika dan hanya jika:
$$
\|\mathbf{x}\|^2 = \mathbf{x} \cdot \mathbf{x} = 1.
$$

---

### Membentuk Vektor Satuan

Misalkan $\mathbf{x}$ adalah vektor tak nol di $\mathbb{R}^n$. Maka:
$$
\frac{\mathbf{x}}{\|\mathbf{x}\|}
$$
adalah vektor satuan.

#### Bukti:
$$
\frac{\mathbf{x}}{\|\mathbf{x}\|} \cdot \frac{\mathbf{x}}{\|\mathbf{x}\|} = \frac{\mathbf{x} \cdot \mathbf{x}}{\|\mathbf{x}\|^2} = \frac{\|\mathbf{x}\|^2}{\|\mathbf{x}\|^2} = 1
$$

---





 

 **Contoh:**
   Misalkan $\mathbf{x} = \begin{bmatrix} 3 \\ 4 \end{bmatrix}$:
   - Panjang vektor:
     $$
     \|\mathbf{x}\| = \sqrt{3^2 + 4^2} = \sqrt{9 + 16} = \sqrt{25} = 5.
     $$
   - Vektor satuan:
     $$
     \mathbf{u} = \frac{\mathbf{x}}{\|\mathbf{x}\|} = \frac{1}{5} \begin{bmatrix} 3 \\ 4 \end{bmatrix} = \begin{bmatrix} \frac{3}{5} \\ \frac{4}{5} \end{bmatrix}.
     $$
   - Verifikasi:
     $$
     \|\mathbf{u}\| = \sqrt{\left(\frac{3}{5}\right)^2 + \left(\frac{4}{5}\right)^2} = \sqrt{\frac{9}{25} + \frac{16}{25}} = \sqrt{1} = 1.
     $$

---

Referensi 

https://linearalgebra.math.umanitoba.ca/math1220/section-33.html