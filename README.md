# Praktikum4
Repository ini dibuat untuk memenuhi tugas pertemuan 9 Praktikum 4 - Bahasa Pemrograman

Nama    :   Aditya Achya Ananta Nur

Nim     :   312210714

Kelas   :   TI.22.C.9

# Latihan membuat list, menampilkan list, menambahkan list dan merubah list

1. Membuat folder dan membuat file latihanlist.py 

  <img width="164" alt="Foto 1" src="https://user-images.githubusercontent.com/115473988/202850544-e6b058b9-6a20-4f46-acff-1f00d1f771c3.png">

2. Berikut merupakan latihan pada bahasa pemograman Pyhton dalam penggunaan list

```python
#   Buat sebuah list sebanyak 5 elemen dengan nilai bebas
list_matkul = ["Pemograman","Algoritma","PAI","Medsos","PTI"]

# Tampilkan nilai list ke 3
print(list_matkul[2])

# ambil nilai elemen ke 2 sampai elemen ke 4
print(list_matkul[1:4])

# ambil elemen terakhir
print(list_matkul[4])

# mengubah elmen list ke 4
list_matkul[3] = "Pancasila"
print(list_matkul)

# ubah elemen ke 4 sampai dengan elemen terakhir
list_matkul[3:5] = "Pancasila","B. Indonesia"
print(list_matkul)

# tambah elemen list
# ambil 2 bagian dari list pertama (A) dan jadikan list ke 2 (B)
list_matkul2 = list_matkul [0:2]
print(list_matkul2)

# tambah list_matkul2 dengan nilai string
list_matkul2.append("Medsos")
print(list_matkul2)

# tambah list B dengan 3 nilai
list_matkul2.extend(["B. Indonesia","PTI","PAI"])
print(list_matkul2)

# gabungkan list matkul 2 dengan list matkul 1
list_gabungan = list_matkul2 + list_matkul
print(list_gabungan)
```

3. Maka hasil setelah di run 

    <img width="801" alt="foto 2" src="https://user-images.githubusercontent.com/115473988/202850690-2f94050a-30ce-49b6-bfbb-5b469cee1d98.png">


# Buat program sederhana untuk menambahkan data kedalam sebuah list dengan rincian sebagai berikut:

1.  Membuat flowchart pemograman yang akan dibuat

  <img width="284" alt="foto 5" src="https://user-images.githubusercontent.com/115473988/202850892-b1db7d10-64f8-4b91-9f9d-232d98c49121.png">

2. Membuat file baru pada folder sebelumnya dan diberi nama latihanlist2

  <img width="126" alt="foto 6" src="https://user-images.githubusercontent.com/115473988/202850984-0479f685-a16b-4e2d-b631-b7d0ab72ae50.png">

3. Pastikan menggunakan pip package tabulate pada awal mulai pemograman 
4. Berikut merupakan pemogramman hasil dari flowchat pada nomer ke 1

```python
nilai = []
ulang = True

while ulang:
    nama = input("Masukkan Nama: ")
    nim = input("Masukkan NIM: ")
    tugas = int(input("Masukkan Nilai Tugas: "))
    uts = int(input("Masukkan Nilai UTS: "))
    uas = int(input("Masukkan Nilai UAS: "))
    akhir = (tugas * 30/100) + (uts * 35/100) + (uas * 35/100)

    nilai.append([nama, nim, tugas, uts, uas, int(akhir)])
    if (input("Tambah data (y/t)?") == 't'):
        ulang = False

print("\n                      Daftar Nilai Mahasiswa")
print("==================================================================")
print("|No. |     Nama     |    NIM    | Tugas |  UTS  |  UAS  |  Akhir |")
print("==================================================================")
i = 0
for item in nilai:
    i += 1
    print("| {no:2d} | {nama:12s} | {nim:9s} | {tugas:5d} | {uts:5d} | {uas:5d} | {akhir:6.2f} |"
          .format(no=i, nama=item[0], nim=item[1], tugas=item[2], uts=item[3], uas=item[4], akhir=item[5]))
print("==================================================================")
```
5. Kemudian run program  

6. Dan masukan data mulai dari nama, nim, kelas, mata kuliah, nilai tugas, uts, dan uas sesuai dengan banyaknya jumlah mahasiswa yang kita inginkan jika dirasa kurang makan tekan y dan jika dirasa cukup maka tekan t

7. maka tampilan program akan seperti berikut

  <img width="837" alt="foto 4" src="https://user-images.githubusercontent.com/115473988/202851374-5d6d9df6-f5f7-49f8-a77f-b6f74d449fbd.png">


## TERIMA KASIH
### ADITYA ACHYA ANANTA NUR - 312210714 - TI.22.C. - TEKNIK INFORMATIKA - UNIVERSITAS PELITA BANGSA
