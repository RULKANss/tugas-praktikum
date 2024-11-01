## Flowchart
![Flowchart](/flochart8.png)


## kode program
```
tipe_tiket = input("Masukkan tipe tiket (reguler/VIP): ").strip().lower()
status_member = input("Apakah Anda memiliki kartu member? (ya/tidak): ").strip().lower()
if tipe_tiket == "reguler":
    harga_tiket = 50000
elif tipe_tiket == "vip":
    harga_tiket = 100000
else:
    print("Tipe tiket tidak valid.")
    harga_tiket = 0
if status_member == "ya" and harga_tiket > 0:
    diskon = harga_tiket * 0.2
    total_harga = harga_tiket - diskon
else:
    total_harga = harga_tiket
if harga_tiket > 0:
    print(f"Total harga yang harus dibayar: Rp{total_harga:.2f}")
```


## Output program
```
PS C:\project ai> & C:/Users/Syahrul/AppData/Local/Microsoft/WindowsApps/python3.11.exe "c:/project ai/latihan.py"
Masukkan tipe tiket (reguler/VIP): reguler
Apakah Anda memiliki kartu member? (ya/tidak): tidak
Total harga yang harus dibayar: Rp35000.00
PS C:\project ai> & C:/Users/Syahrul/AppData/Local/Microsoft/WindowsApps/python3.11.exe "c:/project ai/latihan.py"
Masukkan tipe tiket (reguler/VIP): reguler
Apakah Anda memiliki kartu member? (ya/tidak): ya
Total harga yang harus dibayar: Rp24500.00
PS C:\project ai> & C:/Users/Syahrul/AppData/Local/Microsoft/WindowsApps/python3.11.exe "c:/project ai/latihan.py"
Masukkan tipe tiket (reguler/VIP): vip    
Apakah Anda memiliki kartu member? (ya/tidak): tidak
Total harga yang harus dibayar: Rp90000.00
PS C:\project ai> & C:/Users/Syahrul/AppData/Local/Microsoft/WindowsApps/python3.11.exe "c:/project ai/latihan.py"
Masukkan tipe tiket (reguler/VIP): vip
Apakah Anda memiliki kartu member? (ya/tidak): ya
Total harga yang harus dibayar: Rp63000.00
PS C:\project ai>
```


## Cara kerja program

- Program meminta pengguna untuk memasukkan tipe tiket (reguler atau VIP) dan status keanggotaan (ya atau tidak).
- Berdasarkan tipe tiket yang dipilih, program menetapkan harga tiket yang sesuai (Rp50.000 untuk reguler dan Rp100.000 untuk VIP).
- Jika tipe tiket tidak valid, program mencetak pesan kesalahan dan menetapkan harga tiket menjadi 0.
- Jika pengguna memiliki kartu member dan harga tiket valid, program menghitung diskon 20% dari harga tiket.
- Total harga yang harus dibayar kemudian ditampilkan, dengan format dua angka desimal, jika harga tiket lebih dari 0.


## Flowchart
![Flowchart](/flowchartkalku1.png)


## kode program 
```
def kalkulator():
    angka1 = float(input("Masukkan angka pertama: "))
    operator = input("Masukkan operator (+, -, *, /): ")
    angka2 = float(input("Masukkan angka kedua: "))
    if operator == '+':
        hasil = angka1 + angka2
    elif operator == '-':
        hasil = angka1 - angka2
    elif operator == '*':
        hasil = angka1 * angka2
    elif operator == '/':
        if angka2 != 0:
            hasil = angka1 / angka2
        else:
            return "Error: Pembagian dengan nol tidak diperbolehkan."
    else:
        return "Error: Operator tidak valid."

    return f"Hasil: {hasil}"
print(kalkulator())
```


## Output program
```
PS C:\project ai> & C:/Users/Syahrul/AppData/Local/Microsoft/WindowsApps/python3.11.exe "c:/project ai/latihan2.py"
Masukkan angka pertama: 11
Masukkan operator (+, -, *, /): *
Masukkan angka kedua: 23
Hasil: 253.0
PS C:\project ai> & C:/Users/Syahrul/AppData/Local/Microsoft/WindowsApps/python3.11.exe "c:/project ai/latihan2.py"
Masukkan angka pertama: 121
Masukkan operator (+, -, *, /): +
Masukkan angka kedua: 112
Hasil: 233.0
PS C:\project ai> & C:/Users/Syahrul/AppData/Local/Microsoft/WindowsApps/python3.11.exe "c:/project ai/latihan2.py"
Masukkan angka pertama: 22
Masukkan operator (+, -, *, /): /
Masukkan angka kedua: 2
Hasil: 11.0
PS C:\project ai> & C:/Users/Syahrul/AppData/Local/Microsoft/WindowsApps/python3.11.exe "c:/project ai/latihan2.py"
Masukkan angka pertama: 1121
Masukkan operator (+, -, *, /): -   
Masukkan angka kedua: 1000
Hasil: 121.0
PS C:\project ai>
```


## Flowchart
![Flowchart](/flowchartkalku1.png)
