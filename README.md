# ## NAMA : HARIS ADRIANSYAH
## NIM : 312410286
## KELAS : TI.24.A4
## MATKUL : BAHASA PEMROGRAMAN
# LATIHAN PRATIKUM 5
# ![1](https://github.com/user-attachments/assets/0f5a81bb-0022-41a9-a99d-c3e8a8db85f6)
# Elemen Py
```python 
list_a = [1, 2, 3, 4, 5]

print(list_a[2])

print(list_a[1:4])

print(list_a[-1])

list_a[3] = 10
print(list_a)

list_a[3:] = [11, 12, 13]
print(list_a)

list_b = list_a[:2]
print(list_b)

list_b.append("misalnya")
print(list_b)

list_b.extend([14, 15, 16])
print(list_b)

list_a.extend(list_b)
print(list_a)
```
# CODE PROGRAM DI VISUAL CODE SEPERTI BERIKUT : 
# ![Cuplikan layar 2024-11-18 194349](https://github.com/user-attachments/assets/206711c9-eda2-4450-9ae9-f02d60acc4a4)
## Hasil Dari Program Berikut :
# ![Cuplikan layar 2024-11-18 194810](https://github.com/user-attachments/assets/806202af-e0f6-4918-a1ec-1f05061bd69c)

# MENAMBAH DATA.PY
```Python
class Mahasiswa:
    def _init_(self, nama, nim, nilai_tugas, nilai_uts, nilai_uas):
        self.nama = nama
        self.nim = nim
        self.nilai_tugas = nilai_tugas
        self.nilai_uts = nilai_uts
        self.nilai_uas = nilai_uas

    def hitung_nilai_akhir(self):
        return (self.nilai_tugas + self.nilai_uts + self.nilai_uas) / 3

mahasiswa = []

while True:
    nama = input("Nama: ")
    nim = int(input("NIM: "))
    nilai_tugas = int(input("Nilai Tugas: "))
    nilai_uts = int(input("Nilai UTS: "))
    nilai_uas = int(input("Nilai UAS: "))

    mahasiswa.append(Mahasiswa(nama, nim, nilai_tugas, nilai_uts, nilai_uas))

    tambah_data = input("Tambah data (y/t)? ")
    if tambah_data.lower() == "t":
        break

print("-" * 60)
print("| No | Nama       | NIM  | Tugas | UTS  | UAS  | Akhir     |")
print("-" * 60)

for i, mhs in enumerate(mahasiswa):
    nilai_akhir = mhs.hitung_nilai_akhir()
    print(f"| {i+1:<2} | {mhs.nama:<10} | {mhs.nim:<4} | {mhs.nilai_tugas:<5} | {mhs.nilai_uts:<5} | {mhs.nilai_uas:<5} | {nilai_akhir:<9.2f} |")

print("-" * 60)
```
# PENJELASAN DARI CODE MENAMBAH DATA :
```Python
class Mahasiswa:
    def __init__(self, nama, nim, nilai_tugas, nilai_uts, nilai_uas):
        self.nama = nama
        self.nim = nim
        self.nilai_tugas = nilai_tugas
        self.nilai_uts = nilai_uts
        self.nilai_uas = nilai_uas
__init__: Konstruktor ini digunakan untuk menginisialisasi objek Mahasiswa dengan atribut: nama, nim, nilai_tugas, nilai_uts, nilai_uas

def hitung_nilai_akhir(self):
    return (self.nilai_tugas + self.nilai_uts + self.nilai_uas) / 3
```
## Metode ini mengembalikan nilai akhir mahasiswa, yang merupakan rata-rata dari nilai_tugas, nilai_uts, dan nilai_uas.
```Python
mahasiswa = []
```
## Sebuah daftar kosong mahasiswa disiapkan untuk menyimpan objek Mahasiswa yang akan ditambahkan
```Python
while True:
    nama = input("Nama: ")
    nim = int(input("NIM: "))
    nilai_tugas = int(input("Nilai Tugas: "))
    nilai_uts = int(input("Nilai UTS: "))
    nilai_uas = int(input("Nilai UAS: "))

    mahasiswa.append(Mahasiswa(nama, nim, nilai_tugas, nilai_uts, nilai_uas))

    tambah_data = input("Tambah data (y/t)? ")
    if tambah_data.lower() == "t":
        break
```
## Meminta pengguna untuk memasukkan data mahasiswa berulang kali hingga pengguna memasukkan t untuk berhenti, Setiap input digunakan untuk membuat data Mahasiswa, yang kemudian ditambahkan ke dalam daftar mahasiswa
```Python
print("-" * 60)
print("| No | Nama       | NIM  | Tugas | UTS  | UAS  | Akhir     |")
print("-" * 60)

for i, mhs in enumerate(mahasiswa):
    nilai_akhir = mhs.hitung_nilai_akhir()
    print(f"| {i+1:<2} | {mhs.nama:<10} | {mhs.nim:<4} | {mhs.nilai_tugas:<5} | {mhs.nilai_uts:<5} | {mhs.nilai_uas:<5} | {nilai_akhir:<9.2f} |")

print("-" * 60)
```
## Header tabel dicetak terlebih dahulu, diikuti oleh baris-baris data untuk setiap mahasiswa, Untuk setiap mahasiswa, metode hitung_nilai_akhir dipanggil untuk menghitung nilai akhir, lalu data ditampilkan dalam format tabel
# CODE PROGRAM DI VISUAL CODE SEBAGAI BERIKUT : 
# ![WhatsApp Image 2024-11-17 at 03 17 50_b5acd00f](https://github.com/user-attachments/assets/e96a477b-7926-4005-9f22-ee54ee98601b)
## HASIL PROGRAM DI ATAS SEPERTI DI BAWAH INI :
# ![WhatsApp Image 2024-11-17 at 03 18 47_7483efda](https://github.com/user-attachments/assets/9b7703a5-616e-4232-bfa4-5209df5ed982)

# DAN DI BAWAH INI ADALAH FLOWCHART NYA : 
# ![Screenshot 2024-11-13 083635](https://github.com/user-attachments/assets/fd62b92c-443e-47e4-b088-05bb79c81b93)


