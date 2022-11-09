# **Rangkuman Week5**
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
## Design Database with MySQL
## Design Database with MySQL
## 
