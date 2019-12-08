# Praktikum5

## Algoritma Pemrograman
1. Pertama dalam kita menjalankan program daftar nilai mahasiswa dengan menggunakan dictionary: ketik "L" pada program untuk melihat apakah ada data Mahasiswa yang sudah masuk.

![lihat](https://user-images.githubusercontent.com/56240498/70388994-30cdee80-19ec-11ea-9f73-af2bd2313bab.png)

2. Kedua: tambahkan data mahasiswa dengan klik tombol "T" pada program lalu masukan,nama,nim,nilai tugas,uts dan juga uas

![tambah](https://user-images.githubusercontent.com/56240498/70389019-7a1e3e00-19ec-11ea-94a9-47fe6d249677.png)

3. Lalu cari file yang sudah kita tambahkan dengan cara mengklik tombol "C" pada program dan tuliskanlah nama mahasiswa nya:

![cari](https://user-images.githubusercontent.com/56240498/70389040-c2d5f700-19ec-11ea-89b5-1565702a7f65.png)

4. Kemudian ubahlah file yang sudah di isi dengan file yang berbeda,dengan cara mengklik tombol "U" dan lihat kembali:

![ubah](https://user-images.githubusercontent.com/56240498/70389060-f153d200-19ec-11ea-845e-29f33c22211c.png)

5. Ketika sudah berhasil mengubahnya lalu kita Lihat dan sudah berubah,kemudian kita coba Hapus data mahasiswa yang sudah kita buat dengan cara mengklik tombol "H":

![hapus](https://user-images.githubusercontent.com/56240498/70389064-fca6fd80-19ec-11ea-9156-d9decf0b5fe1.png)

6. Langkah terakhir adalah langkah yang paling mudah,karena semuanya sudah sukses dan berhasil,lalu klik tombol "K" untuk Keluar

![keluar](https://user-images.githubusercontent.com/56240498/70389067-0466a200-19ed-11ea-9b11-3997a05defea.png)

# Flowchartnya

![flowchart ricky](https://user-images.githubusercontent.com/56240498/70390386-089abb80-19fd-11ea-9df5-dc71ec06c8aa.png)

### Penjelasan flowchart:
1. while True:
2. c = input("(L)ihat, (T)ambah, (U)bah, (H)apus, (C)ari, (K)eluar: ")
3. if c.lower() == 'k':
4. elif c.lower() == 'l':
5. print daftar nilai i=0
6. for x in data.items(): i+=1
7. print (" | {6:2} | {0:9s} | {1:11} | {2:6d} | {3:6d} | {4:6d} | {5:6.2f} |"
.format(x[0], x[1][0], x[1][1], x[1][2], x[1][3], x[1][4], i))
8. elif c.lower() == 't':
9. input nama = input(" Nama : ") nim = input(" NIM : ") nilaiuts = int(input(" Nilai UTS : ")) nilaiuas = int(input(" Nilai UAS : ")) nilaitgs = int(input(" Nilai TUGAS : "))
10. akhir = (nilaitgs * 30/100 + nilaiuts * 35/100 + nilaiuas * 35/100) data[nama] = nim, nilaitgs, nilaiuts, nilaiuas, akhir
11. elif c.lower() == 'u':
12. input nama :
13. if nama in data.keys(): nim = input("NIM : ") nilaiuts = int(input("Nilai UTS : ")) nilaiuas = int(input("Nilai UAS : ")) nilaitgs = int(input("Nilai TUGAS : ")) akhir = (nilaitgs * 30/100 + nilaiuts * 35/100 + nilaiuas * 35/100) data[nama] = nim, nilaitgs, nilaiuts, nilaiuas, akhir
14. else: print("Data {0} tidak ada".format(nama))
15. elif c.lower() == 'h':
16. input nama :
17. if nama in data.keys():
18. del data[nama]
19. else: print("Data {0} tidak ada".format(nama))
20. elif c.lower() == 'c':
21. input nama :
22. if nama in data.keys(): print (" daftar nilai ") print (" | {0:9s} | {1:11} | {2:6d} | {3:6d} | {4:6d} | {5:6.2f} |"
.format(nama, nim, nilaitgs, nilaiuts, nilaiuas, akhir))
23. else: print("Data {0} tidak ada".format(nama))
24. else: print("Pilih menu yang tersedia")
