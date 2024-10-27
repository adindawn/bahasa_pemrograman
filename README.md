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
fungsi ```PYTHON (input ()) ```` digunakan untuk memasukkan atau informasi ke dalam sistem 

```PYTHON
(akhir = (int(tugas) * .2) + (int(uts) * .4) + (int(uas) * .4))
````
Fungsi 
