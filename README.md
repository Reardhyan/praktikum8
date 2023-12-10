# praktikum8
OOP

Bahasa Pemrograman

# Class

• Membuat Class

• Membuat Instance class
class Person(): # definisi class
def __init__(self, nama):
self.nama = nama
self.alamat = ""

ari = Person('Ari')
dina = Person('Dina')

• Mengakses Atribut

• Menambahkan Method atau Fungsi
def hitung(a, b): # definisi fungsi
return a + b

class Person():
def __init__(self, nama):
self.nama = nama
self.alamat = ""

def cetak(self):
print("\nNama: {}\nAlamat: {}"\

.format(self.nama, self.alamat))

# Private dan Public Atribut

• Menambahkan atribut private
class Person():
def __init__(self, nama):
self.nama = nama
self.alamat = ""
self.__umur = 0 # antribut private

def __cek_umur(self):
if self.__umur > 17:
return "sudah dewasa"

# Private dan Public Atribut

• Mengakses atribut
ari.nama = 'Ari Santoso' # mengubah nilai atribut
ari.alamat = 'Bekasi' # mengubah nilai atribut

print(ari.nama) # mengakses atribut
print(ari.alamat) # mengakses atribut

ari.cetak() # memanggil fungsi / method

# Setter dan Getter

• Menambahkan Property Setter dan Getter
class Person():

....

@property
def umur(self):
return self.__umur

@umur.setter
def umur(self, value):
self.__umur = value

# Inheritance atau Pewarisan

• Membuat Sub Class

• Instance Class
class Mahasiswa(Person):
def __init__(self, nim, nama):
Person.__init__(self, nama)
self.nim = nim

mhs1 = Mahasiswa('1234', 'Ratna')
mhs1.umur = 25
mhs1.alamat = "Bekasi"
mhs1.cetak_nama()

# Overriding

• Pada Class Person terdapat fungsi cetak_data

• Pada class Mahasiswa fungsi cetak_data ditulis ulang
def cetak_data(self):

print("\nNama: {}\nAlamat: {}\nUmur: {}"\

.format(self.nama, self.alamat, self.__umur))

#overriding
def cetak_data(self):
print("\nNim: {}\nNama: {}\nAlamat: {}\nUmur: {}"\

.format(self.nim, self.nama, self.alamat, self.umur))

Tugas Praktikum

Buat program sederhana dengan mengaplikasikan penggunaan class. Buatlah
class untuk menampilkan daftar nilai mahasiswa, dengan ketentuan:
• Method tambah() untuk menambah data
• Method tampilkan() untuk menampilkan data
• Method hapus(nama) untuk menghapus data berdasarkan nama
• Method ubah(nama) untuk mengubah data berdasarkan nama

• Buat diagram class, flowchart dan penjelasan programnya pada
README.md.
• Commit dan push repository ke github.
![code](https://github.com/Reardhyan/praktikum8/assets/148032571/5b72e9ed-6446-48e3-b883-e51308024bb7)
![Screenshot (142)](https://github.com/Reardhyan/praktikum8/assets/148032571/be97203d-d8af-4a17-8e55-8ff19f25886b)
