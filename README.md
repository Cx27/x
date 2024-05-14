# Diagram Venn untuk Siswa di Kelas

Dalam suatu kelas, 25 orang suka sepak bola, 35 orang suka bulutangkis, dan 15 orang suka keduanya. 3 orang di kelas tidak suka bulutangkis maupun sepak bola. Berikut adalah diagram Venn yang menggambarkan situasi ini:

_________
            /         \
           /           \
          /             \
         /               \
        /    10    15     \ 
       /___________________\
      (          45          )
       \      _______       /
        \    /       \     /
         \  /         \   /
          \            \ /
           \____________/

Di luar kedua lingkaran: 3 orang yang tidak suka keduanya

### Penjelasan Diagram

- **10:** Siswa yang hanya suka sepak bola.
- **20:** Siswa yang hanya suka bulutangkis.
- **15:** Siswa yang suka keduanya.
- **3:** Siswa yang tidak suka bulutangkis maupun sepak bola.

### Total Siswa di Kelas

Jumlah total siswa di kelas adalah 48 orang.

- **45 siswa** suka setidaknya salah satu dari kedua olahraga.
- **3 siswa** tidak suka bulutangkis maupun sepak bola.
- 






# Analisis Keanggotaan Himpunan Fuzzy

## Fungsi Keanggotaan Fuzzy \( \mu_A(x) \)

### Nilai Keanggotaan
- Derajat keanggotaan untuk elemen \( x = 40 \):
  \[
  \mu_A(40) = 0.3
  \]

- Derajat keanggotaan untuk elemen \( x = 3 \):
  \[
  \mu_A(3) = 0.7
  \]

### Penjelasan
- **\(\mu_A(40) = 0.3\)**: Menunjukkan bahwa elemen 40 memiliki derajat keanggotaan sebesar 0.3 dalam himpunan fuzzy \( A \).
- **\(\mu_A(3) = 0.7\)**: Menunjukkan bahwa elemen 3 memiliki derajat keanggotaan sebesar 0.7 dalam himpunan fuzzy \( A \).

### Diagram Venn Fuzzy (Visualisasi Himpunan Fuzzy)

Anda juga bisa menyertakan diagram atau grafik yang merepresentasikan fungsi keanggotaan fuzzy tersebut, misalnya dengan menggunakan matplotlib di Python atau alat grafis lainnya untuk membuat plot keanggotaan.

```python
import matplotlib.pyplot as plt
import numpy as np

# Data keanggotaan
x = np.array([3, 40])
y = np.array([0.7, 0.3])

# Plot fungsi keanggotaan fuzzy
plt.figure(figsize=(8, 5))
plt.plot(x, y, 'bo-', label='Fungsi Keanggotaan Fuzzy')
plt.title('Diagram Keanggotaan Himpunan Fuzzy A')
plt.xlabel('Elemen')
plt.ylabel('Derajat Keanggotaan')
plt.ylim(0, 1)
plt.legend()
plt.grid(True)
plt.show()
