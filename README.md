## Deskripsi program 
Program ini menghasilkan sejumlah bilangan acak menggunakan fungsi random() dari modul random di Python. 
Pengguna diminta untuk memasukkan nilai N,yang menentukan jumlah bilangan acak yang lebih kecil dari 0.5 yang akan dihasilkan.
Setiap bilangan acak yang kurang dari 0.5 akan ditampilkan bersama dengan urutan atau indeksnya.

## Fitur dari program 
program ini dibuat menggunakan bahasa python, dengan fitur yang meliputi: 
- Meminta input dari pengguna untuk jumlah bilangan acak (N) yang lebih kecil dari 0.5.
- Menghasilkan bilangan acak antara 0 dan 1, dan hanya menampilkan bilangan yang lebih kecil dari 0.5.
- Menampilkan urutan (indeks) dari setiap bilangan acak yang valid.

  ## Output program
  ```python
  from random import random

#Meminta input jumlah bilangan acak yang lebih kecil dari 0.5
n = int(input("Masukkan nilai N: "))
count = 0

#Loop untuk menghasilkan dan menampilkan bilangan acak yang kurang dari 0.5
while count < n:
    num = random()
    if num < 0.5:
        count += 1
        print(f"data ke-{count} => {num}")

print("Selesai")
```
## input program
