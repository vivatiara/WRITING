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
   
 

*Multidimensional array* (array multidimensi) adalah sebuah array yang berisikan array lagi didalamnya. Konsepnya penggunaannya sama dengan array biasa (satu dimensi), hanya saja jumlah indeks yang digunakan saat mengakses nilai didalam array adalah sebanyak dimensi dari array tersebut.

Contoh array multidimensi antara lain diagram kartesius dan matriks. Diagram kartesius dan matriks adalah array multidimensi yang sama-sama membutuhkan koordinat untuk mengakses nilai didalamnya.

```
(y)
4 |       *
3 |     *
2 |   *
1 | *
  + - - - - (x)
0   1 2 3 4

Diagram kartesius adalah contoh array 2 dimensi. Setiap titik pada diagram di atas memiliki koordinat (x,y) tertentu yaitu (1,1), (2,2), (3,3), dan (4,4).
```

**berikut contoh array 2 dimensi pada JavaScript dan cara penggunaannya**

```javascript
// cara deklarasi array 2 dimensi kosong
var arr2D = [[]];

// contoh array 2 dimensi
var arr2D = [ [1,2], [3,4], [5,6] ];
var murid = [ ['Budi', 'SD 1 Cicayur'], ['Suci', 'SD 23 Beji'] ];

// cara mengakses nilai didalam array 2 dimensi
console.log(arr2D[0]);    // [1,2]
console.log(arr2D[0][1]); // 2
console.log(murid[1]);    // ['Suci', 'SD 23 Beji']
console.log(murid[1][1]); // 'SD 23 Beji''

// array 2 dimensi dengan built-in functions
arr2D.push([7,8]);        // arr2D = [ [1,2], [3,4], [5,6], [7,8] ]
arr2D[1].push(0);         // arr2D = [ [1,2], [3,4,0], [5,6], [7,8] ]
arr2D[0].pop();           // arr2D = [ [1], [3,4,0], [5,6], [7,8] ]
arr2D[2].pop();           // arr2D = [ [1], [3,4,0], [5], [7,8] ]
```
   

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
  
  

           // ada 2 cara
           // - promise (then catch)
           // - async await

           // ===================== Promise ===================
           // promise
           // namaPromis.then().catch()
           nonton("jalan")
           .then(result => {
             console.log(result);
           }).catch(err => {
             console.log(err)
           })

           // ===================== async await ===============
           // async await -> car utk nangkep obj promise
           // buat async function
           async function asyncNonton() {
             try {
               let result = await nonton("jalan")
               console.log(result);
             } catch (error) {
               console.log(error)
             }
           }
           asyncNonton()

           // async arrow
           // let asyncNonton = async () => { }
  
  
 **async arrow**
  
            // let asyncNonton = async () => { }
  
  

## JavaScript Intermediate - Asynchronous - Promise
  
  <div align="justify">"Memproduksi kode" adalah kode yang bisa memakan waktu lama

  <div align="justify">"Mengkonsumsi kode" adalah kode yang harus menunggu hasilnya

  <div align="justify">Janji adalah objek JavaScript yang menautkan kode yang menghasilkan dan mengonsumsi kode

  <div align="justify">Pending
  <div align="justify">Fulfilled
  <div align="justify">Rejected
      
  <div align="justify"> Objek Promise mendukung dua properti: status dan hasil.

  <div align="justify">Sementara objek Promise "tertunda" (berfungsi), hasilnya tidak ditentukan.

  <div align="justify">Ketika objek Janji "terpenuhi", hasilnya adalah nilai.

  <div align="justify">Ketika objek Promise "ditolak", hasilnya adalah objek error.
   
   
            // ============== Menampilkan data digimon pada web ============

            // belum pakai fetch.......................
            // pakai data dummy
            let listDigimonNonFetch = document.getElementById("list-digimon-non-fetch")
            let digimons = ["Agumon", "Gabumon", "Patamon"]

            digimons.forEach(item => {
              console.log(item)
              listDigimonNonFetch.innerHTML += `<h3>${item}</h3>`

              // alternative
              // let textDigimon = document.createElement("h3")
              // textDigimon.innerText = item
              // containerDigimon.append(textDigimon)
            })

            // sesudah pakai fetch......................
            // async await
            listDigimon = document.getElementById("list-digimon")

            let getDataDigimon = async () => {
              let URL = "https://digimon-api.vercel.app/api/digimon"
              let response = await fetch(URL)
              let digimons = await response.json()

              // menampilkan 10 data digimon
              digimons.slice(0, 10).forEach((item, index) => {
                  listDigimon.innerHTML += 
                  `<div>
                    <img src="${item.img}" alt="" width="200">
                    <h3>${item.name}</h3>
                  </div>`
              })
            }

            getDataDigimon()
   
     
      
  - ### Berikut ini cara menggunakan Promise:
      
         myPromise.then(
         function(value) { /* code if successful */ },
         function(error) { /* code if some error */ }
         );

 - ### Promise Object Properties
 
 <div align="justify">Objek Promise JavaScript dapat berupa:
 
 
- ### Promise Syntax
                 let myPromise = new Promise(function(myResolve, myReject) {
                 // "Producing Code" (May take some time)

                   myResolve(); // when successful
                   myReject();  // when error
                 });

                 // "Consuming Code" (Must wait for a fulfilled Promise)
                 myPromise.then(
                   function(value) { /* code if successful */ },
                   function(error) { /* code if some error */ }
                 );

 
 
 
                 // ================== promise dari function =============
                console.log("PROMISES dari function")
                let nonton = (kondisi) => {
                  return new Promise((resolve, reject) => {
                    if (kondisi == "jalan") {
                      resolve("nonton terpenuhi")
                    }
                    reject("batal nonton")
                  })
                }

                nonton("jalan")
                .then(result => {
                  console.log(result)
                })
                .catch(err => {
                  console.log(err);
                })
  
  
  
            // ========================= CALLBACK =====================
             console.log("CALLBACK")
             console.log("A")

             // butuh proses yg memakan waktu
             // callback -> function yg dijadikan sbg argumen
             setTimeout(() => {
               console.log("B")
             }, 1000)

             console.log("C")
 
 
## Js Intermediate-Web Storage

- ### Apa itu Web Storage?
  <div align="justify">Web storage adalah salah satu Web API yang dapat menyimpan data secara lokal pada sisi client. Berbeda dengan objek atau array, data yang disimpan pada objek atau array JavaScript bersifat sementara, dan akan hilang jika terjadi reload atau pergantian URL pada browser. Sedangkan data yang disimpan pada Web Storage akan bertahan lebih lama karena data akan disimpan pada storage browser.
   
 **<div align="justify"> HTML web storage; better than cookies.**
   
 - ### Property dan method yang digunakan pada localStorage dan sessionStorage yaitu:

   <div align="justify">key(n) Mendapatkan nama key atau nama data urutan ke-n pada penyimpanan dimulai dari 0.
   <div align="justify">length Mendapatkan jumlah item data yang disimpan pada storage
   <div align="justify">getItem(nama_key) Mendapatkan data dari storage dengan nama yang disebutkan
   <div align="justify">setItem(nama_key, data_disimpan) Menyimpan data ke storage
   <div align="justify">removeItem(nama_key) Menghapus data pada storage dengan nama yang disebutkan
   <div align="justify">clear() Mengosongkan semua data tersimpan pada storage
    
    
    
                    // ==================== check ketika pertama kali website di buka, apakah ada key: theme dan value: dark di storage
                document.querySelector("form").addEventListener("submit", (ev) => {
                  ev.preventDefault();
                  const userInput = document.querySelector("input").value;

                  const li = document.createElement("li");
                  li.innerText = userInput;

                  todos.push(userInput);

                  localStorage.setItem("todo", JSON.stringify(todos));

                  const container = document.querySelector("#list-container");
                  container.appendChild(li);
                });
