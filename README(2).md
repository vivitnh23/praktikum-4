## Deskripsi Program 
Program Python ini menghitung laba yang diperoleh setiap bulan berdasarkan modal awal tertentu. Laba yang dihitung bervariasi setiap bulan,
dengan persentase laba yang berbeda-beda di setiap periode.Program ini menunjukkan bagaimana laba berkembang selama 8 
bulan dengan skema persentase yang ditentukan untuk setiap bulan.

## Fitur Program 
- Modal Awal: Menggunakan modal awal sebesar 100 juta.
- Perhitungan Laba: Laba dihitung berdasarkan persentase tertentu yang berbeda setiap bulan.
- Laba per Bulan:
Bulan 1 dan 2: Tidak ada laba.
Bulan 3 dan 4: Laba 1% dari modal awal.
Bulan 5 dan 6: Laba 5% dari modal awal.
Bulan 7: Laba 5% dari modal awal.
Bulan 8: Laba 3% dari modal awal.

## Kode Program 
```python
modal_awal = 100000000
total_laba = 0

print("Laba per bulan:")

for bulan in range(1, 9):
    if bulan == 1 or bulan == 2:
        laba = 0  # Bulan pertama dan kedua belum ada laba
    elif bulan == 3 or bulan == 4:
        laba = modal_awal * 0.01  # Bulan ketiga dan keempat laba 1%
    elif bulan == 5 or bulan == 6:
        laba = modal_awal * 0.05  # Bulan kelima dan keenam laba 5%
    elif bulan == 7:
        laba = modal_awal * 0.05  # Bulan ketujuh laba tetap 5%
    elif bulan == 8:
        laba = modal_awal * 0.03  # Bulan kedelapan laba turun menjadi 3%
    
    print(f"Laba bulan ke-{bulan} sebesar: {laba}")
    total_laba += laba  # Menambahkan laba bulanan ke total laba

print(f"Total laba adalah: {total_laba}")
```

# Output Program 
````
Laba per bulan:
Laba bulan ke-1 sebesar: 0
Laba bulan ke-2 sebesar: 0
Laba bulan ke-3 sebesar: 1000000.0
Laba bulan ke-4 sebesar: 1000000.0
Laba bulan ke-5 sebesar: 5000000.0
Laba bulan ke-6 sebesar: 5000000.0
Laba bulan ke-7 sebesar: 5000000.0
Laba bulan ke-8 sebesar: 3000000.0
Total laba adalah: 20000000.0
````

# Cara Kerja Program 
- Inisialisasi Modal dan Laba: Program dimulai dengan modal awal sebesar 100 juta dan total laba 0.
- Perulangan Bulanan: Program menghitung laba setiap bulan selama 8 bulan dengan persentase laba yang berbeda setiap bulan:
Bulan 1 dan 2: Tidak ada laba.
Bulan 3 dan 4: Laba 1% dari modal.
Bulan 5 dan 6: Laba 5% dari modal.
Bulan 7: Laba 5% dari modal.
Bulan 8: Laba 3% dari modal.
Menampilkan Laba per Bulan: Program mencetak laba setiap bulan dan menambahkannya ke total laba.

Total Laba: Setelah perulangan selesai, program menampilkan total laba yang terkumpul selama 8 bulan.
