# **Rangkuman BE Week1**
## Web Server & RESTful API
Web server terdiri dari 2 komponen penting:
**<div align="justify">Hardware**
<div align="justify">Di sisi perangkat keras, server web adalah komputer yang menyimpan perangkat lunak server web dan file komponen situs web. (misalnya, dokumen HTML, gambar, CSS stylesheet, dan file JavaScript) Server web terhubung ke Internet dan mendukung pertukaran data fisik dengan perangkat lain yang terhubung ke web.
  
**<div align="justify">Software**
<div align="justify">Di sisi perangkat lunak, server web mencakup beberapa bagian yang mengontrol bagaimana pengguna web mengakses file yang dihosting. Minimal, ini adalah server HTTP. Server HTTP adalah perangkat lunak yang memahami URL (alamat web) dan HTTP (protokol yang digunakan browser Anda untuk melihat halaman web). Server HTTP dapat diakses melalui nama domain situs web yang disimpannya, dan mengirimkan konten situs web yang dihosting ini ke perangkat pengguna akhir.

  &nbsp;
  
<div align="justify">Rest – Representational state transfer
<div align="justify">Salah satu arsitektur design untuk membuat web service

<div align="justify">Rules milik rest
  <div align="justify">1.	Uniform interface
  <div align="justify">2.	Client-server
  <div align="justify">3.	Stateless 
  <div align="justify">4.	Cacheable
  <div align="justify">5.	Layered system
  <div align="justify">6.	Code on demand (optimal)
<div align="justify">Api yang menerapkan rules di atas disebut RESTful
  
  &nbsp;
  
**HTTP  method :**
- Get (menggambil data)
- Post (mengirim data baru)
- Delete (hapus data)
- Put / PATCH (update data)

  &nbsp;
  
**Status code :**
-	2xx  - success
-	3xx  - redirect
-	4xx  - client error
-	5xx  - server error


## Intro Node.Js
  
Node.js adalah runtime, Node Js adalah perangkat lunak yang diciptakan secara khusus untuk membantu pengembangan aplikasi berbasis web. Namun, yang perlu dipahami, Node Js bukanlah sebuah bahasa pemrograman baru, melainkan runtime atau yang juga disebut interpreter JavaScript.
  
  &nbsp;
  
Node.js menggunakan arsitektur “Single Threaded Event Loop” untuk menangani beberapa klien bersamaan. Model Pemrosesan Node.js didasarkan pada model berbasis peristiwa JavaScript bersama dengan mekanisme panggilan balik JavaScript.
  
   &nbsp;
  
Thread dalam ilmu komputer adalah eksekusi menjalankan beberapa tugas atau program secara bersamaan. Setiap unit yang mampu mengeksekusi kode disebut thread.

  &nbsp;
  
Sebelum masuk lebih dalam ke Node JS, terdapat beberapa materi yang perlu direview dan di pahami lagi dari bahasa pemorgraman javascript agar mempermudah memahami Node JS  yaitu :

- Arrow function expression (Arrow expression merupakan fitur terbaru dari javascript, yaitu mempermudah membuat sintaks function menggunakan “=>”)
- Asynchronous (Asynchronous merupakan konsep yang paling penting dari javascript. Pada dasarnya, javascript mengeksekusi code secara single thread dan berurutan baris per baris yang disebut dengan synchronous. Sedangkan asynchronous memungkinkan mengeksekusi code tanpa berurutan dengan cara “skip” code dan melanjutkan eksekusi code selanjutnya. Konsep ini menungkinkan code kita tidak terjadi blocking dan lebih efisien.)

- JSON (JSON atau Javascript Object Notation merupakan format yang digunakan untuk menyimpan dan mengirim data menggunakan konsep object di javascript. JSON dapat digunakan di hampir semua bahasa pemrograman sehingga sangat cocok untuk dipelajari)

   &nbsp;
  
**Install Node JS**
- Untuk mengetes apakah berhasil terinstall, dapat menjalankan “node -v” untuk mengecek versi NodeJS yang terinstal.
               
                  node -v    
 
- Kita dapat menggunakan node di terminal kita dengan mengetik “node” kemudian bisa membuat code javascript dan langsung dieksekusi
  
                  node 
  
  &nbsp;
  
**Build In Module Node JS**
- Console (merupakan module bawaan dari javascript yang ada di node JS untuk digunakan sebagai debug atau menampilkan code secara interface)
- Process adalah modules yang digunakan untuk menampilkan dan mengontrol prosess Node JS yang sedang dijalankan.
- OS module merupakan module yang digunakan untuk menyediakan informasi terkait sistem operasi komputer yang digunakan user.
- Module Util merupakan alat bantu / utilities untuk mendukung kebutuhan internal API di Node JS
- Events
- Errors merupakan modules yang dapat digunakan untuk mendefinisikan error di Node JS sehingga lebih informatif. Kita juga dapat menghandle error menggunakan try catch
- Buffer merupakan modules yang digunakan untuk mengakses, mengelola dan mengubah tipe data raw atau tipe data bytes
- Fs atau “file system” merupakan module yang dapat membantu berinteraksi dengan file yang ada diluar code. FS paling sering digunakan untuk membaca file dengan ekstensi .txt, .csv, dan .json
- Timers merupakan modules yang digunakan untuk melakukan scheduling atau mengatur waktu pemanggilan fungsi yang dapat diatur di waktu tertentu

   &nbsp;
  
**Node JS Web Server**
- Untuk menggunakan modul HTTP, gunakan require()
- Gunakan method createServer() untuk membuat server HTTP
- Callback function yang digunakan pada method http.createServer(), akan dijalankan ketika seseorang mencoba mengakses komputer pada port 8080.

  
## Express Js
  
Express.js adalah framework web app untuk Node.js yang ditulis dengan bahasa pemrograman JavaScript. Express.js adalah framework back end. Artinya, ia bertanggung jawab untuk mengatur fungsionalitas website, seperti pengelolaan routing dan session, permintaan HTTP, penanganan error, serta pertukaran data di server. 
  
   &nbsp;
  
Back end app adalah aplikasi yang berjalan di server-side yang bekerja untuk memberikan informasi berupa data sesuai request dari client / browser / front end app. Umumnya server-side app membuat REST API

  &nbsp;
  
RESTful API / REST API merupakan penerapan dari API (Application Programming Interface). 

Sedangkan REST (Representional State Transfer) adalah sebuah arsitektur metode komunikasi yang menggunakan protokol HTTP untuk pertukaran data dimana metode ini sering diterapkan dalam pengembangan aplikasi. Dengan tujuannya untuk menjadikan sistem memiliki performa yang baik, cepat dan mudah untuk di kembangkan (scale) terutama dalam pertukaran dan komunikasi data.

   &nbsp;
  
RESTFUL API memiliki 4 komponen penting yaitu:

- URL Design
- HTTP Verbs
- HTTP Response Code
- Format Response
  
  &nbsp;
  
Installation and Preparation
- Install express JS.  xpressJS adalah sebuat modules atau package yang dikembangkan menggunakan bahasa javascript, maka kita bisa menggunakan NPM untuk menginstall express JS

              nmp install express --save
  
- Preparation, Terdapat beberapa module yang perlu diinstal untuk mempermudah develop server side application, seperti nodemon (agar dapat restart application otomatis selama proses development)

             nmp install --save-dev  nodemon

- Routes, Routes adalah sebuah end point yang diapat kita akses menggunakan URL di website. Didalam routes kita perlu menentukan method API, alamat dan response apa saja yang akan dikeluarkan
- method, Kita dapat menggunakan method yang dalam REST API seperti POST, PUT, PATCH dan DELETE
- Response, Di dalam route kita dapat mengirim response menggunakan parameter dari route express.js yaitu “res.Send()” untuk mengirim plain text ketika kita mengakses route tersebut. 
- Query, Query merupakan parameter yang digunakan untuk membantu menentukan tindakan yang lebih spesifik daripada hanya sekedar router biasa. Biasanya query ditaruh di akhir route dengan memberikan informasi diawali dengan “?” kemudian tedapat key dan data
- Status Code, Dalam pengaplikasian back end application, kita sangat perlu memberikan status code sebagai informasi apakah route yang kita akses berjalan sebagaimana mestinya dan tidak terjadi error.

  &nbsp;
  
Apa Itu Middleware ?

- Middleware function adalah sebuah fungsi yang memiliki akses ke object request (req), object response (res), dan sebuah fungsi next didalam request-response cycle.
- Fungsi next biasanya di berikan nama variable next.

Bagaimana Cara Middleware Bekerja?

- Untuk memahami cara kerja middleware, bayangkan Anda memiliki stan minuman lemon di mana pelanggan membawa lemon mereka sendiri dan Anda membuat minuman lemon dari buah yang di bawa langsung oleh pelanggan.

- Anda bertanggung jawab untuk mengevaluasi asal dan kesegaran buah lemon, membuang lemon di bawah standar, dan, akhirnya, membuat minuman lemonnya.

- Untuk mengurangi beban kerja Anda, Anda mempekerjakan seorang pekerja — kita akan memanggilnya Larry — yang bertugas untuk memastikan lemon ditanam secara organik dan tanpa bahan kimia berbahaya.

- Dalam analogi ini, Larry adalah middleware yang berfungsi antara Anda dan pelanggan Anda.

  
## Design Database with MySQL
  
Menentukan Entity
  
- Berdasarkan requirement yang ada kita bisa mulai untuk mengidentifikasi entity dalam database.
- Beberapa kandidat yang paling sering menjadi sebuah entity : peoples, things, events, locations
- Mari kita lihat kembali requirement yang ada, dan kita mulai list entity yang ada.
- Berikut adalah kandidat yang bisa dijadikan enitity dalam database :
  - User
  - Singer
  - Track
  - Album
  - Playlist
  
  &nbsp;
  
Menentukan Atribbutes dari Entity
  
- Tahapan ini kita akan menentukan attributes apa saja yang akan datanya kita simpan di dalam sebuah entity.
- Attributes yang di perlukan didalam entity kemungkinan sudah ada di dalam requirements document, atau mungkin juga diperlukan penafsiran kita sendiri sebagai database developer.
  
  &nbsp;
  
![image_2022-11-11_203013892](https://user-images.githubusercontent.com/80299731/201350267-8a79df58-adf2-4848-9040-7de53dc4177f.png)

![image_2022-11-11_203225149](https://user-images.githubusercontent.com/80299731/201350653-b3827ec1-3de8-441f-b165-471f9d885bb6.png)

![image_2022-11-11_203349467](https://user-images.githubusercontent.com/80299731/201350892-8e6e3747-57c3-4f67-9a47-5bd6d1e9d0bf.png)


 ![image_2022-11-11_203447309](https://user-images.githubusercontent.com/80299731/201351061-7e2ae52b-27b5-4170-8f4b-4c35564ced7d.png)
 
  &nbsp;
  
Membuat SQL Table dari Entity
- Setelah kita punya ERD, maka kita akan lanjut dengan create table berdasarkan dengan data yang kita punya.
- Pada kali ini kita akan menggunakan terminal untuk menjalankan query SQL
  
   &nbsp;
  
                          Membuat Table User
                          CREATE TABLE ‘user’ (
                          ‘user_id INT NOT NULL auto_INCREMENT,
                          ‘name’ VARCHAR(50) NOT NULL DEFAULT ‘’,
                          ‘Email’ VARCHAR(50) NOT NULL DEFAULT ‘’,
                          ‘password’ VARCHART(50) NOT NULL DEFAULT ‘’,
                          PRIMARY KEY (‘user_id)
                          )
  
  &nbsp;
  
Apa itu Basis Data Relasional?
<div align="justify">Menurut Oracle, database relasional adalah "sejenis database yang menyimpan dan menyediakan akses ke titik data yang terkait satu sama lain". Oke terdengar bagus
  
  &nbsp;
  
foreign key adalah pengenal unik atau kombinasi pengenal unik yang menghubungkan dua tabel atau lebih dalam suatu database. Foreign key juga sering disebut sebagai kunci asing.
  
  &nbsp;
  
Primary key adalah suatu nilai dalam basis data yang digunakan untuk mengidentifikasi suatu baris dalam tabel. Nilai dari primary key adalah unik.


