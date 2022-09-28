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
| 4. Akses secara offline | 4. Akses secara online | 
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

    ![git_innit](https://raw.githubusercontent.com/Jirjatss/week-1/main/gambar/git_init.JPG)

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

    ![](gambar/tebal-miring.JPG)

  - Tag HTML Untuk Membuat tulisan dengan link

    ```html
    <a href="">Welcome To AMMAN Coding Bootcamp BATCH 3</a>
    ```

    Hasilnya di web browser

    ![](gambar/link.jpg)

  - Tag Untuk Membuat Daftar/List

    - Ordered List

      ```html
      <ol>
        Dafunda
        <li>Dafunda Tekno</li>
        <li>Dafunda Otaku</li>
        <li>Dafunda Games</li>
      </ol>
      ```

      Hasilnya di web browser

      ![](gambar/ol.jpg)

    - Unordered List

      ```html
      <ul>
        Dafunda
        <li>Dafunda Tekno</li>
        <li>Dafunda Otaku</li>
        <li>Dafunda Games</li>
      </ul>
      ```

      Hasilnya di web browser

      ![](gambar/ul.jpg)

  - Tag HTML Untuk Menampilkan gambar

    ```html
    <img src="https://bit.ly/2FKluzq" alt="Si Kucing"></img>
    ```

    Hasilnya di web browser

    ![](gambar/gambar.jpg)

    &nbsp;

- Deploy HTML

  <div align="justify">Deploy adalah sebuah proses untuk menyebarkan aplikasi yang sudah kita kerjakan supaya bisa digunakan oleh orang-orang. Jika aplikasi kita HTML atau Web App kita perlu mendeploy ke server. Untuk melakukan hal tersebut kita bisa menggunakan layanan yang bernama Netlify
            
