# BIODATA
NAMA  = ADINDA AULIA NABILA PUTRI
KELAS = TI.24.A.4
NIM   = 312410309


# soal latihan

  ![Screenshot (17)](https://github.com/user-attachments/assets/3d70e15a-62e1-43fc-b8e6-7ad9b3ef4186)

# Pemrograman Menentukan nilai akhir 
```PYTHON
(nama = input("Masukkan nama:")
uts = input("Masukkan nilai UTS:")
uas = input("Masukkan nilai UAS:")
tugas = input("Masukkan nilai Tugas:")
akhir = (int(tugas) * .2) + (int(uts) * .4) + (int(uas) * .4)
keterangan = ("TIDAK LULUS", "LULUS")[akhir > 60.0]
if akhir > 80:
    huruf = "A"
elif akhir > 70:
     huruf = "B"
elif akhir > 50:
     huruf = "C"
elif akhir > 40:
     huruf = "D"
else:
    huruf = "E"
print("\nNama :",nama)
print("Nilai UTS :",uts)
print("Nilai UAS :",uas)
print("Nilai Tugas :",tugas)
print("Nilai Akhir :",akhir)
print("\nNilai Huruf :",huruf)
print("Keterangan :",keterangan))
````
fungsi input () digunakan untuk memasukkan atau informasi ke dalam sistem 

```PYTHON
(akhir = (int(tugas) * .2) + (int(uts) * .4) + (int(uas) * .4))
````
Fungsi int(tugas), int(uts), dan int(uas) digunakan untuk mengoversi nilai bilangan bulat, 
bilangan positif atau bilangan negatif, serta nol.

```PYTHON
(keterangan = ("TIDAK LULUS", "LULUS")[akhir > 60.0])
````

Jika nilai akhir lebih besar dari 60 makan keterangannya "LULUS", 
dan jika nilai akhir lebih kecil dari 60 maka keterangannya "TIDAK LULUS"

```PYTHON
print("\nNama :",nama)
print("Nilai UTS :",uts)
print("Nilai UAS :",uas)
print("Nilai Tugas :",tugas)
print("Nilai Akhir :",akhir)
print("\nNilai Huruf :",huruf)
print("Keterangan :",keterangan))
````
Fungsi print() ini akan mencetak variable program tersebut 

# Hasil Screenshot dari Visual Studio Code 

  ![Screenshot (24)](https://github.com/user-attachments/assets/4f86c842-acc1-47f7-b5f8-dee277e9d090)

# Program Menampilkan Status Gaji Karyawan 

```PYTHON
(gaji = int(input("Masukkan gaji:"))
berkeluarga = (False, True)[input("Sudah berkeluarga? (Y/T)") == "Y"]
punya_rumah = (False, True)[input("Punya rumah? (Y/T)") == "Y"]

if gaji > 3000000:
    print ("Gaji sudah diatas UMR")
    if berkeluarga:
        print ("Wajib ikutan asuransi dan menabung untuk pensiun")
    else:
        print ("Tidak perlu ikutan asuransi")
    if punya_rumah:
        print ("wajib bayar pajak rumah")

    else:
        print ("tidak wajib bayar pajak rumah")
else:
    print ("Gaji belum UMR")
````

Struktur kondisi ini menggunakan if, elif, dan else.

```PYTHON
(gaji = int(input("Masukkan gaji:"))
````
inputan ini akan memasukkan gaji, karena memiliki fungsi input()

```PYTHON
(berkeluarga = (False, True)[input("sudah berkeluarga? (Y/T") == "Y"]
punya_rumah = (False, True)[input("punya rumah? (Y/T") == "Y"])
````

inputan ini menggunakan fungsi string yang masukkan beberapa huruf,
dan (False, True) ini adalah fungsi pemilihan Y/T,
supaya tidak menggunakan if dilanjutkan program tersebut.

```PYTHON
(if berkeluarga:
        print ("Wajib ikutan asuransi dan menabung untuk pensiun")
    else:
        print ("Tidak perlu ikutan asuransi"))
````

Jika memiliki rumah Output yang keluar "Wajib bayar Pajak",
dan jika tidak memiliki rumah Output yang keluar "Tidak wajib membayar Pajak".

```PYTHON
(else:
   print ("Gaji belum UMR"))
````

Apabila gaji tidak melebihi dari 3000000 program akan mencetak "Gaji belum UMR"

# Hasil Screenshot dari Visual Studio Code
  ![Screenshot (25)](https://github.com/user-attachments/assets/5ddb97b4-2c14-4944-a2e5-cf77cbe42266)

# Program Membandingkan 3 Input Bilangan

```PYTHON
(a = int(input("Masukkan bilangan A: "))
b = int(input("Masukkan bilangan B: "))
c = int(input("Masukkan bilangan C: "))

if a+b == c or b+c == a or c+a == b:
    print("BENAR")
else:
    print("SALAH"))
````

```PYTHON
(if a+b == c or b+c == a or c+a == b:
print("BENAR")
else:
print("SALAH"))
````

Jika A ditambah B hasilnya C, bahasa pemrogramnya OR, 
dan jika B ditambah C hasilnya A, dan C ditambah A maka hasilnya B.
maka pemrograman akan mencetak "BENAR".

# Hasil Screenshot dari Visual Studio Code
  ![Screenshot (26)](https://github.com/user-attachments/assets/5220f42c-9c79-49ec-a877-baa4a3f14286)

  

# LATIHAN 3

# Program Pemesanan Tiket Bioskop
   ![Screenshot (27)](https://github.com/user-attachments/assets/f803ab35-6bc2-4f6e-ad4c-17fd43a948e1)

```PYTHON
HARGA_REGULER = 50000
HARGA_VIP = 100000
DISKON_MEMBER = 0.2  # 20% diskon

def hitung_harga_tiket():
    print("=== Program Hitung Harga Tiket Bioskop ===")
    print("\nPilih tipe tiket:")
    print("1. Reguler (Rp50.000)")
    print("2. VIP (Rp100.000)")
    
    # Input tipe tiket
    while True:
        try:
            tipe_tiket = int(input("\nMasukkan pilihan (1/2): "))
            if tipe_tiket in [1, 2]:
                break
            print("Error: Pilihan tidak valid. Silakan pilih 1 atau 2.")
        except ValueError:
            print("Error: Mohon masukkan angka 1 atau 2.")

    # Input status member
    while True:
             member = input("Apakah anda memiliki kartu member? (y/n): ").lower()
        if member in ['y', 'n']:
            break
        print("Error: Mohon masukkan 'y' atau 'n'.")

    # Menentukan harga dasar menggunakan operator ternary
    harga_dasar = HARGA_REGULER if tipe_tiket == 1 else HARGA_VIP
    
    # Menghitung total harga dengan mempertimbangkan diskon member menggunakan operator ternary
    total_harga = harga_dasar * (1 - DISKON_MEMBER) if member == 'y' else harga_dasar
    
    # Menampilkan rincian pembayaran
    print("\n=== Rincian Pembayaran ===")
    print(f"Tipe Tiket: {'Reguler' if tipe_tiket == 1 else 'VIP'}")
    print(f"Status Member: {'Ya' if member == 'y' else 'Tidak'}")
    print(f"Harga Dasar: Rp{harga_dasar:,.0f}")
    if member == 'y':
        print(f"Diskon Member (20%): Rp{(harga_dasar * DISKON_MEMBER):,.0f}")
    print(f"Total Pembayaran: Rp{total_harga:,.0f}")

# Menjalankan program
if _name_ == "_main_":
    hitung_harga_tiket())
````

Program ini akan menentukan harga pesanan tiket bioskop, yang reguler/vip,
dan jika vip harga 100.000, dan jika reguler 80.000, dan jika memiliki kartu member pelanggan tersebut akan mendapatkan diskon 20%

# Hasil Screenshot dari Visual Studio Code 
 
  ![Screenshot (29)](https://github.com/user-attachments/assets/f117e346-8cd9-42e1-a542-46973e1ae65c)
  ![Screenshot (30)](https://github.com/user-attachments/assets/897d0866-dde2-43a4-a032-9206eab8a2d9)

# Hasil Flowchart nya
  
  ![Untitled Diagram drawio (2)](https://github.com/user-attachments/assets/e0ccf18a-326b-467d-8230-c4a2d4d334bb)



# Program Kalkulator Sederhana
   ![Screenshot (31)](https://github.com/user-attachments/assets/cfa8108e-0986-4500-9fee-c1af42212ce9)

```PYTHON
(if operator == '+':
     hasil = angka1 + angka2
     print(f"Hasil penjumlahan: {hasil}")
 elif operator == '-':
     hasil = angka1 - angak2
     print(f"Hasil pengurangan: {hasil}")
 elif operator == '*':
     hasil = angka1 * angka2
     print(f"Hasil perkalian: {hasil}")
 elif operator == '/':
     if angka2 != 0:
         hasil = angka1 / angka2
         print(f"Hasil pembagian: {hasil}")
     else:
         print("Error: Pembagian dengan nol tidak diperbolehkan.")

else:
   print("Error: Operator tidak valid. Silahkan gunakan +, -. *, atau /.")
```` 
Program kalkulator sedehana dalam python adalah proyek yang baik untuk pemula dan programmer tingkat lanjut. program ini memungkinkan pengguna untuk melakukan operasi matematika seperti penjumlahan, pengurangan, perkalian, dan pembagian. 

# Hasil dan Pemrogram Screenshot dari Visual Studio Code 
   ![Screenshot (33)](https://github.com/user-attachments/assets/f52d6458-dc20-4080-b8d8-2c14b0f7170e)
   ![Screenshot (32)](https://github.com/user-attachments/assets/a3225764-f656-439a-9835-5ad322120020)

# Hasil Flowchart nya







   
