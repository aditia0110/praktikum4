# Praktikum4

# Belajar struktur kondisi dan perulangan pda python


1. Membuat folder dengan nama Praktikum4 lalu didalamnya kita buat dua folder lagi yaitu **Struktur Kondisi** dan **Perulangan** dan di dalam folder tersebut kita buat file **Latihan1.py** dan **Latihan2.py**

Contohnya sepeerti pada Gambar berikut : 

<img width="134" alt="image" src="https://user-images.githubusercontent.com/115475348/200100664-a9fd3e8d-c5e1-4809-a285-166238da4e7a.png">

2. Langkah selanjutnya kita buka folder **Struktur Kondisi** dan buka file **Latihan1** kemudian imput codingan seperti berikut :

`# menerima input yang diketik dengan menyimpannya didalam variabel`

`bilanganSatu = input("Masukan bilangan Pertama : ")`

`bilanganKedua = input("Masukan bilangan Kedua : ")`  

`# mengkonversi input string ke integer karena method input() selalu mengembalikan type data string`

`bilanganSatu = int(bilanganSatu)`

`bilanganKedua = int(bilanganKedua)`

`# mengecek untuk menentukan bilangan terbesar dari kedua bilangan`

`if bilanganSatu > bilanganKedua :`

`print("Bilangan ", bilanganSatu, "lebih besar dari bilangan", bilanganKedua)`
    
`else :`

`print("Bilangan ", bilanganKedua, "lebih besar dari bilangan", bilanganSatu)`
    
    
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

 




