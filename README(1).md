## Deskripsi program 
Program ini menghasilkan sejumlah bilangan acak menggunakan fungsi random() dari modul random di Python. 
Pengguna diminta untuk memasukkan nilai N,yang menentukan jumlah bilangan acak yang lebih kecil dari 0.5 yang akan dihasilkan.
Setiap bilangan acak yang kurang dari 0.5 akan ditampilkan bersama dengan urutan atau indeksnya.

## Fitur dari program 
program ini dibuat menggunakan bahasa python, dengan fitur yang meliputi: 
- Meminta input dari pengguna untuk jumlah bilangan acak (N) yang lebih kecil dari 0.5.
- Menghasilkan bilangan acak antara 0 dan 1, dan hanya menampilkan bilangan yang lebih kecil dari 0.5.
- Menampilkan urutan (indeks) dari setiap bilangan acak yang valid.

  ## Kode Program 
  ```python
  from random import random

  n = int(input("masukan nilai N: "))
  count = 0

  while count < n:
      num = random()
      if num < 0.5:
        count += 1
        print(f"data ke-{count} => {num}")
  
  print("selesai")
```
# Output Program
```'
Masukkan nilai N: 3
data ke-1 => 0.13874598480703348
data ke-2 => 0.44327004245785784
data ke-3 => 0.4887813949571461
Selesai

````

# Cara Kerja Program
- Input: Program meminta pengguna untuk memasukkan nilai N, yaitu jumlah angka yang lebih kecil dari 0.5 yang ingin dicetak.
- Perulangan: Program menghasilkan angka acak antara 0 dan 1 menggunakan random().
- Pengecekan: Jika angka yang dihasilkan kurang dari 0.5, angka tersebut dicetak dan dihitung.
- Berhenti: Program terus menghasilkan angka acak hingga jumlah angka yang lebih kecil dari 0.5 mencapai N, lalu mencetak "Selesai" dan berhenti.
