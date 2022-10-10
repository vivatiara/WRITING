# **Rangkuman Week3**

## JS Intermediate-Array

- ### Apa itu Array?
 <div align="justify">Mengorganisasi data dan menyimpan data adalah core concept dari programming.

- ### Bagaimana kalau kita ingin menyimpan banyak data pada 1 variabel?

              let arr = ["hallo", 1, true]

              arr[0] = "selamat datang"

              console.log(arr);
              console.log(arr.length);
              console.log(arr[0])
              console.log(arr[1])
              console.log(arr[2])

              let arrBuah = [
                "jeruk", 
                "semangka", 
                "pepaya", 
                "rambutan",
                "melon",
                "belimbing"
              ]
  
- ### MENGAPA Array ada
  <div align="justify">Karena Array adalah tipe data list order yang dapat menyimpan tipe data apapun di dalamnya. Array dapat menyimpan tipe data String,      Number, Boolean, dan lainnya.

- ### Contoh Array
   **<div align="justify">Pada javascript, array dapat kita buat dengan tanda kurung siku ([...])**
      
          
          var products = [];

    <div align="justify">Maka variabel products akan berisi sebuah array kosong.
       &nbsp;
      
    **<div align="justify"> Kita bisa mengisi data ke dalam array, lalu setiap data dipisah dengan tanda koma (,)**
      
        var products = ["Flashdisk", "SDD", "Monitor"];
     
     **<div align="justify">Cara Mengambil Data dari Array**
      <div align="justify"> Seperti yang sudah kita kethaui… Array akan menyimpan sekumpulan data dan memberinya nomer indeks agar mudah diakses. Indeks array selalu dimauli dari nol 0.Misalkan kita punya array seperti ini:
    
        var makanan = ["Nasi Goreng", "Mie Ayam", "Mie Gelas"];
       
     <div align="justify">Bagaimana cara kita mengambil nilai "Mie Ayam"?

     <div align="justify"> Jawabannya seperti ini:
        
         makanan[1] //-> "Mie Ayam"
     
    **<div align="justify">Mencetak isi Array dengan Perulangan**
      
         document.write(products[0]);
         document.write(products[1]);
         document.write(products[2]);
         document.write(products[3]);
         document.write(products[4]);
      
    **<div align="justify">Mari kita lihat contohnya:**
      
          <!DOCTYPE html>
          <html lang="en">
          <head>
              <title>Array dan perulangan</title>
          </head>
          <body>
              <script>
                  // membuat array
                  var products = ["Senter", "Radio", "Antena", "Obeng"];

                  document.write("<h3>Daftar Produk:</h3>");
                  document.write("<ol>");
                  // menggunakan perulangan untuk mencetak semua isi array
                  for(let i = 0; i < products.length; i++){
                      document.write(`<li>${ products[i] }</li>`);
                  }
                  document.write("</ol>");
              </script>
          </body>
          </html>
    
   Hasilnya:
      
     ![89](https://user-images.githubusercontent.com/80299731/194806598-944c50dc-52aa-42c7-93ed-f36d23405ddb.JPG)
  
  **Kita bisa mengunakan perulangan dengan method forEach().**
      
           arrBuah.forEach((item) => {
           console.log(item)
         })
      
   **Cara Menambahkan Data ke Dalam Array**
      
<div align="justify">ada dua cara yang bisa dilakukan untuk menambah data ke dalam array:
<div align="justify">1. Mengisi menggunakan indeks;
<div align="justify">2. Mengisi menggunakan method push().
 
 <div align="justify">Mengisi dengan indeks maksudnya adalah 
  
         var buah = ["Apel", "Jeruk", "Manggis"];
  
  Terdapat tiga data di dalam array buah dengan indeks:

 <div align="justify">0: "Apel"
 <div align="justify">1: "Jeruk"
 <div align="justify">2: "Manggis"
  
 Kita ingin menambahkan data lagi pada indeks ke-3, maka kita bisa melakukannya seperti ini:
  
         buah[3] = "Semangka";
 
  Mengisi menggunakan method push()
  
         arrBuah.push("duku")          // di akhir
         arrBuah.unshift("anggur")     // di awal
  
  **Cara Menghapus Data Array**
  
  <div align="justify">Sama seperti menambahkan data ke array, menghapus data juga memiliki dua cara:

<div align="justify">1, Menggunakan delete;
<div align="justify">2. Menggunakan method pop().

         delete buah[2];
 
 Kita dapat menghapus data dengan nomer indeks tertentu dengan delete. Sedangkan pop() akan menghapus dari belakang.

 <div align="justify">Kekurangan dari delete, ia akan menciptakan ruang kosong di dalam array.
  
  ![image_2022-10-10_132729140](https://user-images.githubusercontent.com/80299731/194808736-9704fd9a-063f-496f-bc88-ac9f0e7bad91.png)

 Menggunakan method pop().
  
          arrBuah.pop()        // di akhir
          arrBuah.shift()      // di awal
  
  **Mengubah isi Array**
  
           var bahasa = ["Javascript", "Kotlin", "Java", "PHP", "Python"];
           bahasa[1] = "C++";
  
  Maka "Kotlin" akan diganti dengan "C++".
  
  **<div align="justify">map**
  <div align="justify">map() melakukan perulangan/looping dengan membuat array baru.
 
   
         // map..........................
       // bisa dengan return
       let buahSegar = arrBuah.map((item) => {
         return item + " " + "segar"
       })
       console.log(buahSegar)
   
   
 - ### Method-method penting pada Array 
  
## JS Intermediate-Multidimensional Array

## JS Intermediate-Object

## Js Intermediate-Recursive

## JavaScript Intermediate - Asynchronous - Introduction

## JavaScript Intermediate - Asynchronous - Promise

## Js Intermediate-Web Storage

