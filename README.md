# Praktikum4

# Belajar struktur kondisi dan perulangan pada python


1. Membuat folder dengan nama Praktikum4 lalu didalamnya kita buat dua folder lagi yaitu **Struktur Kondisi** dan **Perulangan** dan di dalam folder tersebut kita buat file **Latihan1.py** dan **Latihan2.py**

Contohnya sepeerti pada Gambar berikut : 

<img width="134" alt="image" src="https://user-images.githubusercontent.com/115475348/200100664-a9fd3e8d-c5e1-4809-a285-166238da4e7a.png">

2. Langkah selanjutnya kita buka folder **Struktur Kondisi** dan buka file **Latihan1** kemudian imput codingan seperti berikut :

        # menerima input yang diketik dengan menyimpannya didalam variabel
        bilanganSatu = input("Masukan bilangan Pertama : ")
        bilanganKedua = input("Masukan bilangan Kedua : ")  

        # mengkonversi input string ke integer karena method input() selalu mengembalikan type data string
        bilanganSatu = int(bilanganSatu)
        bilanganKedua = int(bilanganKedua)

        # mengecek untuk menentukan bilangan terbesar dari kedua bilangan
        if bilanganSatu > bilanganKedua :
            print("Bilangan ", bilanganSatu, "lebih besar dari bilangan", bilanganKedua)
        else :
            print("Bilangan ", bilanganKedua, "lebih besar dari bilangan", bilanganSatu)
    
<img width="495" alt="input latihan 1 struktur kondisi" src="https://user-images.githubusercontent.com/115475348/200101223-79f905d7-eb22-4905-a010-aa18c0d2f440.png">

3. Langkah selanjutnya jika sudah diinput lalu kita jalankan, dan akan keluar hasil seperti berikut ini :

<img width="767" alt="hasil latihan 1 struktur kondisi" src="https://user-images.githubusercontent.com/115475348/200101379-fb18605f-af25-42dd-ac1c-1205954d059d.png">

 4. Selanjutnya buka **Latihan2.py** pada folder **Struktur Kondisi** lalu input codingan berikut ini : 
 
        # variable angka untuk menampung jumlah angka yang diinputkan berupa array/list
        angka = []
        # variable bilangan untuk menentukan jumlah bilangan yang diinginkan
        bilangan = input("Masukan jumlah bilangan yang diinginkan : ")
        
        # mengkonversi input string ke integer karena method input() selalu mengembalikan type data string
        bilangan = int(bilangan)
        
        print("Program mengurutkan data ")
        
        # melakukan perulangan berdasarkan jumlah dari variable bilangan
        
        for i in range(0, bilangan):
        
          # melakukan perulangan input sampai jumlah dari variabel bilangan yang sudah ditentukan
          # misal bilangan sama dengan 4 maka akan dimunculkan input 4 kali lalu disimpan dari variable => data

          data = int(input("Masukan Bilangan Ke-" + str(i+1) + " : "))

          # menambahkan isi dari variable data ke variable angka yang type datanya berupa array
          # contoh input pertama [3] => input ke-dua [3,5] => input ke-tiga [3,5,2] => input ke-empat[3,5,2,9] dan seterusnya sesuai jumlah variable bilangan
          angka.append(data)
          
        # menampilkan hasil program
        # method sorted() berfungsi untuk mengurutkan nilai dari terkecil ke terbesar,
        print("Bilangan yang sudah diurutkan dari terkecil ke terbesar", sorted(angka))

 <img width="832" alt="input latihan 2 struktur kondisi" src="https://user-images.githubusercontent.com/115475348/200102405-18a78d12-8d60-47f2-9714-0d9f132aeb09.png">

5. Jika suda diinput selanjutnya kita jalankan, dan akan keluar hasil seperti berikut ini : 

<img width="764" alt="hasil latihan 2 struktur kondisi" src="https://user-images.githubusercontent.com/115475348/200102498-681cd9a8-2cff-4c73-8211-c1e54850f8ff.png">

6. Selanjutnya kita masuk kedalam folder **Perulangan** dan buka file **Latihan1.py** lalu input codingan berikut ini :

        # melakukan perulangan dari 0 sampai 10
        for i in range (0, 10):
            # menampilkan variabel i , (" " * 3) Artinya menambahkan spasi tiga kali lalu end => yaitu memulai baris baru setelah nilai terakhir
            print(i, " " * 3, end= '')
    
            # melakukan perulangan dari 1 sampai 10
            for j in range (1, 10):
                # menampilkan output j + i , (" " * 3) Artinya menambahkan spasi tiga kali lalu end => yaitu memulai baris baru setelah nilai terakhir
                print(j+i, " " * 3, end='')
            print()

<img width="713" alt="input latihan 1 perulangan" src="https://user-images.githubusercontent.com/115475348/200103242-e349d374-bc97-44ee-89d5-59ec578303d2.png">

7. Jika sudah diinput selanjutnya kita jalankan, dan akan keluar hasil seperti berikut ini :

<img width="762" alt="hasil latihan 1 perulangan" src="https://user-images.githubusercontent.com/115475348/200103598-210cc1ea-a06c-4e6b-8581-0145dc92901e.png">

8. Selanjutnya buka **Latihan2.py** pada folder **Perulangan** lalu input kembali codingan berikut ini :

        # import module random untuk mengenerate angka acak 0.3222...dst
        from random import random

        # variable jumlahNilai menampung input masukan lalu diconvert ke integer
        jumlahNilai = int(input('Masukan jumlah nilai yang ingin dicari : '))

        # variable nilaiRandom & kurangDariNolKomaLima berupa array/list untuk menyimpan data yang diperlukan nanti.
        nilaiRandom = []
        kurangDariNolKomaLima = []

        # looping data berdasarkan jumlahNilai,
        for i in range(0, jumlahNilai):
            # variable n = menyimpan angka random contoh: 0.9905112793033766
            n = random()
    
            # menambahkan n ke variabel nilaiRandom
            # fungsi append() untuk menambahkan data ke dalam variabel yang type datanya berupa array/list
            nilaiRandom.append(n)
    
            # apakah n < dari 0.5 ? jika iya tampilkan lalu break dan memulai ke angka random selanjutnya
            while n < 0.5:
        
                # menambahkan n jika kurang dari 0.5 ke variable kurangDariNolKomaLima
                kurangDariNolKomaLima.append(n)
        
                # menampilkan output n
                print("data ke-", str(i+1), " => ", n)
                break
    
    
        print()
        # menampilkan output keseluruhan nilai random
        print("Berikut keseluruhan nilai Random dari total ", jumlahNilai,
                "yaitu ", nilaiRandom)

        print()
        # menampilkan output keseluruhan nilai n < 0.5
        print("Berikut nilai yang kurang dari 0.5 berjumlah ", len(kurangDariNolKomaLima),
                "yaitu ", kurangDariNolKomaLima)
                
<img width="452" alt="input latihan 2 perulangan" src="https://user-images.githubusercontent.com/115475348/200104148-a4b3869a-2048-4001-96d5-22c9d2d20cd9.png">
                
9. Jika sudah diinput selanjutnya kita jalankan, dan akan keluar tampilan seperti berikut ini :

<img width="763" alt="hasil latihan 2 perulangan" src="https://user-images.githubusercontent.com/115475348/200104207-d19e4810-3171-4457-8d1f-1de39007bbf5.png">


Sekian sedikit penjelasan dari saya, kurang lebihnya mohon maaf

Terimakasih


