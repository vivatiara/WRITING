# **Rangkuman Week1**

## Unix Commad Line
- ### CLI (Command Line Interface)
  <div align="justify">Merupakan program yang memungkinkan pengguna mengetik perintah teks yang memerintahkan komputer untuk melakukan tugas tertentu, atau juga CLI itu berbasis Tulisan.
  
- ### Shell
  <div align="justify">Merupakan perintah - perintah yang digunakan untuk menginstruksikan sistem operasi.
  <div align="justify"> Shell juga merupakan program yang digunakan untuk berkomunikasi atau memerintah sistem.
    
- ### Terminal Emulator
  <div align="justify"> adalah aplikasi untuk mengakses CLI. User dan komputer dihubungkan dengan terminal, dimana terminal yaitu tempat/aplikasi dimana user dapat mengetikan atau memberikan suatu perintah. Disinilah tempat dimana shell akan berperan.
    
- ### File System Structure
  <div align="justify">sebuah bentuk struktur dari direktori atau file - file yang ada di dalam komputer.
    
- ### Command

  - **pwd** (print working directory), untuk melihat current working directory
  - **dir** (directory), untuk melihat directory
  - **cd** (change directory), untuk pindah directory
  - **ls** (list), untuk melihat isi file di dalam directory
  - **touch**, untuk membuat file directory
  - **cp** (copy), untuk menyalin file directory
  - **mv** (move), untuk memindahkan file directory
  - **rm** (remove), untuk menghapus file directory
    
   &nbsp;
  
  ## Git & Github
 - ### Apa itu Git & Github  
    - Git
    <div align="justify">Git adalah aplikasi yang dapat melacak setiap perubahan yang terjadi pada suatu folder atau file, Git biasanya digunakan oleh para programmer sebagai tempat penyimpanan file pemrograman mereka karena lebih efektif, File -file yg disimpan digit akan terlacak seluruh perubahannya, termasuk siapa yang mengubah sehingga programmer merasa aman.

    - Github
    <div align="justify">Merupakan vendor penyedia layanan git yang dimiliki oleh microsoft atau secara definisi merupakan layanan hosting berbasis web sebagai repositori git dan GitHub merupakan layanan cloud yang berguna untuk menyimpan dan mengelola sebuah project yang dinamakan repository.
  &nbsp;
      
 - ### Perbedaan antara Git dan Github  
| **Git** | **Github** | 
| ----------- | :---------: 
| 1. Meng-install software di penyimpanan lokal | 1. Host melalui layanan cloud |
| 2. Dikelola oleh The Linux Foundation | 2. Diakuisisi oleh Microsoft pada 2018 |
| 3. Akses secara offline | 3. Akses secara online | 
|5. Berfokus pada version control dan code sharing|5. Berfokus pada source code hosting terpusat|
  &nbsp;    
      
  - ### Mengapa wajib menggunakan Git & Github?
    - Alasan utamanya adalah sepandai apapun programmer, tidak akan mampu untuk mengerjakan semuanya sendiri selamanya. Maka dari itu dengan menggunakan Git & Github akan memudahkan programmer untuk bisa bekerja sama dalam sebuah tim. Tujuan besarnya adalah programmer bisa berkolaborasi dengan programmer lainnya dengan mengerjakan proyek yang sama tanpa harus repot copy paste folder aplikasi yang terupdate.
    - platform ini memungkinkan programmer dalam mengubah kode secara otomatis. Hal tersebut dapat menghemat waktu bagi programmer untuk menyusun dan mengubah sebuah kode.

&nbsp;
      
 - ### alur kerja dari Git dan Github
      - Git
         <div align="justify">Cara kerja Git melibatkan beberapa file proyek yang tersimpan di direktori proyek. Kemudian, file yang tersimpan tadi akan         diperbarui yang dipindah ke Staging Area. Setelah peninjauan, file kode tersebut dimuat ke Git Repository, berikut gambar diagram alur kerja Git. 
      
      - Github
          <div align="justify"> Cara kerja pada GitHub harus terkoneksi pada internet sehingga tidak perlu meng-install sebuah software ke dalam perangkat keras. Hal ini memberikan keringanan penyimpanan komputer yang kita gunakan karena file project tersimpan oleh cloud GitHub.
          
&nbsp;
            
 - ### Command di dalam Git & Github
     - git init <nama_proyek>, untuk membuat repositori baru

       ![git init](https://user-images.githubusercontent.com/80299731/192761413-359cbdaf-a7eb-42b5-85b1-4e8eb6fd934b.png)


     - <div align="justify">git commit, untuk melakukan commit atau menyimpan perubahan pada version control pada git. Dan kita bisa menambahkan pesan untuk membeikan checkout pada setiap perbuahan. contohnya "git commit -m "pesan checkout"

    ![git-commit1](<https://raw.githubusercontent.com/Jirjatss/week-1/main/gambar/git-commit1%20(1).jpg>)

     - git push origin, untuk mempublish file atau aplikasi ke github

    ![git-push](https://raw.githubusercontent.com/Jirjatss/week-1/main/gambar/git-push%20-%20Copy.JPG)

     - git clone, untuk melakukan cloning dari github ke komputer atau local

    ![git-clone](<https://raw.githubusercontent.com/Jirjatss/week-1/main/gambar/git-clone%20(1).JPG>)
            
            
## HTML
 - Definisi HTML

  <div align="justify">Merupakan bahasa komputer yang digunakan untuk membuat kerangka atau struktur untuk Web pages (halaman website) di internet. 
    
 - Bagaimana peran HTML pada web development?
    <div align="justify">Web browser seperti Chrome, Firefox, Edge, Safari, atau Opera akan membaca dokumen HTML. Dokumen HTML yang berisi tag-tag HTML akan memberitahu browser bagaimana cara menampilkan sebuah konten.

&nbsp;

- Kerangka HTML

  HTML memiliki sebuah kerangka seperti gambar dibawah ini

  ```html
  <html>
  <head>
  <title>
      Judul Website
    </title>
  <body>
      saya sedang belajar pemrograman HTML dasar.
    </body>
  </html>
  ```

    <div align="justify">Sintak diatas biasa disebut dengan kerangka bahasa pemrograman HTML. Didalam website selalu ada title untuk tiap-tiap web, untuk memasukkan title didalam web kamu harus mengetikkan diantara tag title (dapat diisikan dengan nama website kamu atau yang lainnya). Untuk memasukkan konten-konten, kamu dapat memasukkannya atau mengetikkannya didalam program tepat diantara tag body (Ganti titik-titik dengan konten).

  &nbsp;

- Tag HTML

  <div align="justify">Tag adalah sebauh penanda awalan dan akhiran dari sebuah elemen di HTML. Tag dibuat dengan kurung siku (<...>), lalu di dalamnya berisi nama tag dan kadang juga ditambahkan dengan atribut.

  &nbsp;

  <div align="justify">Tag selalu ditulis berpasangan. Ada tag pembuka dan ada tag penutupnya. Namun, ada juga beberapa tag yang tidak memiliki pasangan penutup. Tag penutup ditulis dengan menambahkan garis miring (/) di depan nama tag, tag HTML memiliki dua tipe utama block-level dan inline tags.
   
   - Elemen block-level memakai semua ruang yang tersedia dan selalu membuat line baru di dalam dokumen. Contoh dari tag block adalah heading dan paragraf.
   - Elemen inline hanya memakai space sesuai dengan kebutuhannya dan tidak membuat line baru di halaman. Biasanya elemen ini akan memformat isi konten dari elemen block-level. Contoh dari tag inline adalah link dan emphasized strings.

  &nbsp;

  Contoh tag HTML

  - Tag untuk membuat tulisan tebal dan miring

    ```html
    <b>Tebal</b> <i>Miring</i>
    ```

    Hasilnya di browser

    ![image_2022-09-28_171431408](https://user-images.githubusercontent.com/80299731/192753803-d421289f-c9d1-4a8f-8666-aa5392caefd0.png)


  - Tag HTML Untuk Membuat tulisan dengan link

    ```html
    <a href="">Welcome To viva tiara Coding Bootcamp BATCH 3</a>
    ```

    Hasilnya di web browser

  ![image_2022-09-28_171642347](https://user-images.githubusercontent.com/80299731/192754221-fb8034bc-2e69-47e5-b1f6-ed5165e2721f.png)


  - Tag Untuk Membuat Daftar/List

    - Ordered List

      ```html
      <ol>
        viv
        <li>viv Tekno</li>
        <li>viv Otaku</li>
        <li>viv Games</li>
      </ol>
      ```

      Hasilnya di web browser

     ![ol](https://user-images.githubusercontent.com/80299731/192755079-6fe122b0-51c4-45d6-90a7-4abdfe764a68.JPG)


    - Unordered List

      ```html
      <ul>
        viv
        <li>viv Tekno</li>
        <li>viv Otaku</li>
        <li>viv Games</li>
      </ul>
      ```

      Hasilnya di web browser

     ![image_2022-09-28_172220655](https://user-images.githubusercontent.com/80299731/192755381-9ba61e54-0a59-4ea5-84d4-717f5c5d6d0c.png)


  - Tag HTML Untuk Menampilkan gambar

    ```html
    <img src="[https://bit.ly/2FKluzq](https://img2.pngdownload.id/20171201/9c4/rabbit-png-image-5a21e60a049693.5834797315121710180188.jpg)" alt="Si Kelinci"></img>
    ```

    Hasilnya di web browser

   ![kelinci](https://user-images.githubusercontent.com/80299731/192757532-f3b88e99-88ab-4b94-bab3-cd2fd3f48a6c.JPG)


    &nbsp;

- Deploy HTML

  <div align="justify">Deploy adalah sebuah proses untuk menyebarkan aplikasi yang sudah kita kerjakan supaya bisa digunakan oleh orang-orang. Jika aplikasi kita HTML atau Web App kita perlu mendeploy ke server. Untuk melakukan hal tersebut kita bisa menggunakan layanan yang bernama Netlify
 
- Bagaimana mendeploy HTML
    - Kita gunakan tools bernama Netlify
    - Kita tinggal masuk ke netlify.com lalu register seperti biasa menggunakan email atau github
    - Setelah itu masuk ke tab Sites lalu drag and drop seluruh folder html kalian
    - Pilih Repository yang akan di Deploy
    - Melakukan Konfigurasi
    - Deploy Website
 &nbsp;
    
## CSS

- Definisi CSS

  <div align="justify">CSS (Cascading Style Sheets) adalah bahasa komputer yang digunakan untuk menambahkan design ke suatu halaman website di internet agar terlihat lebih cantik/menarik. Kita ibaratkan HTML adalah kerangka yang memberi sturuktur pada website, maka CSS adalah baju yang memberi warna dan layout pada website.

&nbsp;

- Cara Menggunakan CSS

  1. Inline Styles
    nline CSS digunakan untuk tag HTML tertentu. Atribut <style> digunakan untuk memberikan style ke tag HTML tertentu.

     Kita menambahkann CSS langsung pada atribut HTML

     ```html
     <p style="color:blue">Tulisan ini berwarna biru</p>
     ```

     ![image_2022-09-28_173813685](https://user-images.githubusercontent.com/80299731/192758549-30a4758a-a726-468c-892d-971b148a726c.png)


  &nbsp;

  2. Internal CSS

     Kode CSS internal diletakkan di dalam bagian <head> pada halaman. CSS internal diletakkan di dalam tag "<style></style>".
    
     ```html
<!DOCTYPE html>
     <html>
       <head>
         <title>Website Pertamaku</title>
         <style>
           body {
             background-color: pink;
           }
           h1 {
             color: black;
           }
           p {
             color: green;
           }
         </style>
       </head>
       <body>
         <h1>Website Pertamaku</h1>
         <p>Selamat Datang</p>
       </body>
     </html>
     ```

     Tampilan dari sintaks diatas adalah

    ![image_2022-09-28_174122940](https://user-images.githubusercontent.com/80299731/192759119-ae9fc673-1dca-4286-af8a-2d0ca25157c7.png)


     &nbsp;

  3. Eksternal CSS

     <div align="justify"> CSS eksternal biasanya diletakkan setelah bagian <head> pada halaman
     Contoh:

     <div align="justify">Kita memiliki dua file: index.html untuk file HTML-nya dan styles.css untuk file CSS-nya.

     ```html
     <!-- File index.html -->

     <!DOCTYPE html>
     <html>
       <head>
         <title>Website Pertamaku</title>
         <link rel="stylesheet" href="styles.css" />
       </head>
       <body>
         <h1>Website Pertamaku</h1>
         <p>Selamat Datang</p>
       </body>
     </html>
     ```

     ```css
     /* File styles.css */

     body {
       background-color: rgb(241, 22, 59);
     }
     h1 {
       color: black;
     }
     p {
       color: rgb(39, 231, 39);
     }
     ```

     Tampilan dari sintaks diatas adalah

     ![2](https://user-images.githubusercontent.com/80299731/192760849-59f9e9eb-ea90-4664-98e3-a83ccb52a874.JPG)


     &nbsp;

- CSS Syntax

  <div align="justify">CSS Syntax adalah syntax yang digunakan untuk menunjuk atau memilih HTML element mana yang ingin diberi style (dihias). CSS syntax terdiri dari selector, property, dan value.

  Syntaxnya seperti ini:

  ```css
  p {
    color: blue;
  }
  ```

  Penjelasan :

  - p

    Adalah sebuah selector berupa element HTML yang akan diubah

  - color

    <div align="justify">Adalah sebuah properti berupa bagian mana dari element HTML yang akan diubah. Contoh diatas kita akan mengubah warna dari teks yang ada di element p

  - blue

    Adalah value yaitu nilai/hiasan berupa warna biru

  &nbsp;


