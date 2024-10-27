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


