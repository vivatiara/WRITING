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
   
    
  
## JS Intermediate-Multidimensional Array

## JS Intermediate-Object
- ### Apa itu Object
   
  <div align="justify">object adalah sebuah tipe data pada variabel yang menyimpan properti dan fungsi (method)
   
  **<div align="justify">Properti** adalah data lengkap dari sebuah object.
   
  **<div align="justify">Method** adalah action dari sebuah object. Apa saja yang dapat dilakukan dari suatu object.
  
 **<div align="justify">Do’s**
  
  <div align="justify">1. Object dapat mengupdate value dari key yang sudah tersedia
  <div align="justify">2. Object dapat menambahkan key dan value baru


 <div align="justify">Tipe data yang sudah kita pelajari:
  
<div align="justify">1. number
<div align="justify">2. string
<div align="justify">3. boolean
<div align="justify">4. null
<div align="justify">5. undefined
<div align="justify">6. array
<div align="justify">7. object

 <div align="justify">Sama seperti tipe data sebelumnya. Object dapat diassign kedalam sebuah variabel.
  
  <div align="justify">Object person

  
              let person = {};



**Mengakses Object dan Property Object**

        let person = {
        name : 'john Doe;,
        age : 25,
        isverified : true,
        }

        console.llog(person):
   
**memanggil nama objek dengan variable**
   
         let properti = "umur";
         console.log(siswa[properti]);

         siswa.nama = siswa.umur;
         console.log(siswa);
   
 **cara akses objek terbagi menjadi 2**
<div align="justify">1. dot notation
<div align="justify">2. bracket
 
         //dot notation
         let siswa = {
         nama: "terra",
         umur: 17,
         hobi: "memancing",
         "nomor handphone": 182367599,
 
         console.log(siswa.nama);
         // console.log(siswa.nomor handphone);
 
 
         // bracket
          console.log(siswa["nama"]);
          console.log(siswa["nomor handphone"]);
 
 
         // memanggil nama objek dengan variable
         let properti = "umur";
         console.log(siswa[properti]);

         siswa.nama = siswa.umur;
         console.log(siswa);
         Footer
 
 
**menambahkan properti baru ke dalam objek**
 
 
          let buku = {
            judul: "mantan jadi manten",
            penulis: "hayati",
            "jumlah halaman": 250,
          };

          console.log(buku);

          buku.tahun = 2022;
          buku.terjual = 3000;
          console.log(buku);

          buku["penerbit"] = "gramedia";
          console.log(buku);
 
 **Create object**
           // note: key pada object biasanya disebut juga dengan properti

           let nama_obj = {
             key1: "value",
             key2: "value2",
           };

           let siswa = {
             nama: "terra",
             umur: 17,
             hobi: "memancing",
             "nomor handphone": 082367599,
           };

           console.log(siswa);
 
 

## Js Intermediate-Recursive
 
- ### apa itu Recursive
 <div align="justify">Recursive adalah function yang memanggil dirinya sendiri sampai kondisi tertentu. Recursive kebanyakan digunakan untuk case matematika, fisika, kimia, dan yang berhubungan dengan calculation.
  
- ### Ciri dari rekursif:
 <div align="justify">1. Fungsi rekursif selalu memiliki kondisi yang menyatakan kapan fungsi tersebut berhenti. Kondisi ini harus dapat dibuktikan akan                            tercapai, karena jika tidak tercapai maka kita tidak dapat membuktikan bahwa fungsi akan berhenti, yang berarti algoritma kita tidak                           benar.
<div align="justify">2. Fungsi rekursif selalu memanggil dirinya sendiri sambil mengurangi atau memecahkan data masukan setiap panggilannya. Hal ini penting                      diingat, karena tujuan utama dari rekursif ialah memecahkan masalah dengan mengurangi masalah tersebut menjadi masalah-masalah kecil.


 - ### Struktur recursive
 
              function rwcursive() {
              recursive() ;
              }
 
 - ## contoh 
 
 **<div align="justify">Rekursi dengan Angka**
 
               function sum(l){
                  if (empty(l)) {
                      return 0;
                  } else {
                      return car(l) + sum(cdr(l));
                  }
              }
 
 
<div align="justify">Fungsi empty mengembalikan nilai true jika list tidak memiliki elemen. fungsi car mengembalikan elemen pertama dalam list. Sebagai contoh, car([1,2,3,4]) mengembalikan nilai 1. Fungsi cdr mengembalikan list tanpa elemen pertama. Sebagai contoh, cdr([1,2,3,4]) mengembalikan nilai [2,3,4]. Apa yang terjadi ketika kita menjalankan sum([1,2,3,4])?

## JavaScript Intermediate - Asynchronous - Introduction
 
 - ### Asynchronous
 <div align="justify">Pemrograman Asynchronous adalah teknik yang memungkinkan program Anda untuk memulai tugas yang berpotensi berjalan lama dan masih dapat responsif terhadap peristiwa lain saat tugas itu berjalan, daripada harus menunggu sampai tugas itu selesai. Setelah tugas itu selesai, program Anda disajikan dengan hasilnya.
  
- ### Synchronous programming
  
  
            const name = 'Miriam';
          const greeting = `Hello, my name is ${name}!`;
          console.log(greeting);
          // "Hello, my name is Miriam!"

## JavaScript Intermediate - Asynchronous - Promise

## Js Intermediate-Web Storage

