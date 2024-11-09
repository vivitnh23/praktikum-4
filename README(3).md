## Deskripsi Program 
Program Python ini mensimulasikan penggunaan mesin ATM sederhana. Pengguna dapat melakukan dua aksi utama: menarik uang dan
keluar dari aplikasi. Program ini menghitung saldo pengguna dan memungkinkan mereka untuk menarik uang sesuai dengan saldo yang tersedia. 
Jika saldo tidak mencukupi, program akan memberikan peringatan.

## Fitur Program
- Saldo Awal: Program dimulai dengan saldo awal sebesar Rp 1.000.000.
- Menu Interaktif: Pengguna dapat memilih untuk menarik uang atau keluar dari aplikasi.
- Validasi Input: Program memeriksa apakah jumlah penarikan tidak melebihi saldo yang tersedia dan memastikan input pengguna valid.
- Penanganan Kesalahan: Program akan menangani kesalahan jika pengguna memasukkan input yang tidak valid (misalnya, input bukan angka).

  ## Kode Program
  ```python
  def atm():
    saldo = 1000000  # Initial balance
    while True:
        print(f"Saldo saat ini: Rp {saldo}")
        print("1. Tarik Uang")
        print("2. Keluar")
        
        pilihan = input("Pilih menu (1/2): ")
        
        if pilihan == '1':
            try:
                jumlah_penarikan = int(input("Masukkan jumlah penarikan: "))
                if jumlah_penarikan <= saldo:
                    saldo -= jumlah_penarikan
                    print("Penarikan berhasil!")
                else:
                    print("Saldo tidak mencukupi.")
            except ValueError:
                print("Input tidak valid. Masukkan angka.")
        elif pilihan == '2':
            print("Terima kasih telah menggunakan ATM!")
            break
        else:
            print("Pilihan tidak valid. Coba lagi.")
        print()

    atm()
```

# Output Program
````
Saldo saat ini: Rp 1000000
1. Tarik Uang
2. Keluar
Pilih menu (1/2): 1
Masukkan jumlah penarikan: 500000
Penarikan berhasil!

Saldo saat ini: Rp 500000
1. Tarik Uang
2. Keluar
Pilih menu (1/2): 2
Terima kasih telah menggunakan ATM!
````

# Cara Kerja Program
- Saldo Awal: Program dimulai dengan saldo Rp 1.000.000.
- Menu Pilihan: Program menampilkan dua opsi:
1: Tarik uang (memasukkan jumlah penarikan).
2: Keluar dari program.
Penarikan:
Jika pengguna memilih tarik uang, program memeriksa apakah jumlah penarikan tidak melebihi saldo.
Jika cukup, saldo dikurangi dan penarikan berhasil.
Jika saldo tidak cukup, program memberi peringatan.
- Keluar: Jika memilih keluar, program mengucapkan terima kasih dan berhenti.
- Validasi Input: Program memastikan input yang dimasukkan valid (angka) dan memberikan pesan error jika input salah.
