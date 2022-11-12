# **Rangkuman BE Week2**

## Back-End Development, Database Intro, Database

Back-end adalah segala macam teknologi yang ada di sisi server dari sebuah website atau aplikasi.

  &nbsp;
  
Back-end developers dapat memilih dari sekian banyak bahasa pemrograman dan framework, tetapi itu semua tergantung pada jenis aplikasi apa yang dibuat.

![image_2022-11-12_144055365](https://user-images.githubusercontent.com/80299731/201463250-6d11b31f-7af7-431b-83d8-4b21f91a78ba.png)

Server adalah sebuah jaringan komputer yang menyediakan jenis layanan tertentu (service) pada komputer lain.
Komputer server biasanya didukung dengan prosesor yang bersifat scalable dan RAM yang besar.
Server juga dilengkapi dengan sistem operasi khusus, yang disebut sebagai Sistem Operasi Jaringan/Network Operating System.
Secara sederhana, server bekerja atas permintaan dari sebuah klien.

  &nbsp;

Database dapat didefinisikan sebagai kumpulan data yang disimpan secara sistematis di dalam komputer yang dapat diolah dan dimanipulasi.

  &nbsp;
  
API adalah sekumpulan instruksi program dan protokol yang digunakan untuk membangun aplikasi perangkat lunak.
REST API bertugas sebagai penghubung/perantara antara Front-End dan Back-end untuk saling bertukar informasi(request dan response).

  &nbsp;
  
MERN adalah salah satu kombinasi teknologi antara front-end dan back-end untuk membuat aplikasi website. 
MERN adalah singkatan dari MongoDB, Express, React, dan NodeJS. Teknologi Full-stack yang menggunakan 1 bahasa yaitu Javascript.

   &nbsp;
   
Mengapa MERN Stack?
- Segala kegiatan pengembangan menggunakan bahasa Javascript
- Mendukung arsitektur MVC (Model View Controller) untuk membuat proses pengembangan lebih lancar dan terstruktur.
- Dengan semua teknologi menggunakan Javascript, maka developer hanya perlu menguasai Javascript dan JSON.
- Open source framework dengan dukungan komunitas yang besar dan baik.


## MySQL Lanjutan

tipe-tipe relations pada MySQL

- One to Many
    - Paling Sering Digunakan
    - Satu baris dalam tabel dapat memiliki beberapa baris di table relasinya
    
 ![image_2022-11-12_152107353](https://user-images.githubusercontent.com/80299731/201465361-896c57cf-f4b2-4b8f-8459-b9209b6d51da.png)

- Many to Many
    - Digunakan ketika kedua tabel yang berelasi dapat memiliki beberapa baris di tabel relasinya.
    
![image_2022-11-12_152155672](https://user-images.githubusercontent.com/80299731/201465386-d6ed2103-f40f-4ab9-8303-945d910a16f0.png)

- One to One
    - Sangat jarang digunakan
    - Diimplementasikan dengan cara yang sama seperti One to Many tetapi dengan kondisi tambahan (foreign key merupakan primary key)

![image_2022-11-12_152244892](https://user-images.githubusercontent.com/80299731/201465414-b3b447c5-9bf6-4b3d-bbad-f322e10436bf.png)

- Pengertian Database Normalization
Merupakan teknik analisis data yang mengorganisasikan atribut-atribut data dengan cara mengelompokkan sehingga terbentuk entitas yang non-redundant, stabil, dan fleksible.

- Tujuan Database Normalization
Menghilangkan redundan data pada database.
Memudahkan juka ada perubahan struktur table database.
Memperkecil pengaruh jika ada perubahan dari struktur table database.

- Efek Jika Tidak Melakukan Database Normalization
  - INSERT Anomali : Situasi dimana tidak memungkinkan memasukkan beberapa jenis data secara langsung di database.
  - DELETE Anomali : Penghapusan data yang tidak sesuai dengan yang diharapkan, artinya data yang harusnya tidak terhapus mungkin ikut terhapus.
  - UPDATE Anomali : Situasi dimana nilai yang diubah menyebabkan inkonsistensi database, dalam artian data yang diubah tidak sesuai dengan yang diperintahkan atau yang diinginkan.

- Bentuk Database Normalization
  - First Normal Form (1NF)
  - Menghilangkan multiple value pada sebuah kolom table database
  - Sebuah table memenuhi kaidah 1NF jika :
      Setiap kolom bernilai tunggal (single value)
      Setiap kolom memiliki nama yang unik
      Urutan penyimpanan data tidak menjadi masalah
      
- Second Normal Form (2NF)
    - Harus sudah dalam bentuk 1NF untuk mendapatkan 2NF
    - Menghapus beberapa subset data yang ada pada tabel dan menempatkan mereka pada tabel terpisah.

- Third Normal Form (3NF)
    - Menghilangkan seluruh atribut atau field yang tidak berhubungan dengan primary key. Dengan demikian tidak ada ketergantungan transitif pada setiap kandidat key.

- Masih ada banyak bentuk database normalisasi, diantaranya :
    - EKNF
    - BCNF
    - 4NF
    - 5NF
    - DKNF
    - 6NF

- Keys di SQL
  - Super Key
    - Kumpulan dari satu atau lebih dari satu key yang dapat digunakan untuk mengidentifikasi record secara unik dalam sebuah tabel.
    - Super Key adalah superset dari Candidate Key.
  - Candidate Key
    - kumpulan satu atau lebih fields/columns yang dapat mengidentifikasi record secara unik dalam tabel.
    - Bisa jadi ada beberapa Candidate Keys di dalam satu tabel
    - Setiap Candidate Key bisa digunakan sebagai Primary Key.
    - Candidate Key adalah super key yang tidak mempunyai value yang berulang
   - Primary Key
     - kumpulan satu atau lebih fields/columns dari sebuah tabel yang secara unik mengidentifikasi sebuah record dalam tabel database.
     - Valuenya tidak boleh berupa null ataupun duplicate value.
     - Hanya boleh salah satu Candidate Key yang bisa menjadi Primary Key.
    - Alternate Key
     - key yang bisa digunakan menjadi primary key.
     - Pada dasarnya, Key ini merupakan candidate key yang tidak dijadikan  primary key.
   - Unique Key
      - Kumpulan dari satu atau lebih fields/columns di sebuah table database yang secara unik mengidentifikasi sebuah record dalam table database tersebut.
      - Hampir sama dengan Primary key, namun value dari Unique Key bisa berupa satu buah null value di dalam sebuah table database, dan Unique Key tidak bisa memiliki duplicate values
   - Foreign Key
      - Field di sebuah table database yang menjadi Primary Key di table database lain.
      - Value dari Foreign key bisa menerima multiple null dan duplicate values.


- INNER JOIN
  - Semua baris akan diambil dari kedua table yang akan di JOIN, selama columns cocok dengan kondisi yang sudah di tentukan.
  - Memungkinkan baris dari salah satu tabel muncul di hasil jika dan hanya jika kedua tabel memenuhi kondisi yang ditentukan dalam klausa ON.
- LEFT JOIN
  - Pada JOIN ini, semua records dari table di sisi kiri JOIN statement akan di pilih.
  - Jika record yang di pilih dari table kiri tidak memiliki record yang cocok pada table JOIN yang kanan, maka record tersebut masih dipilih, dan kolom pada table yang kanan akan bernilai NULL. 
- RIGHT JOIN
  - Pada JOIN ini, semua records dari table di sisi kiri JOIN statement akan di pilih, bahkan jika table di sebelah kiri tidak memiliki record yang cocok.
- Aggregate Functions
Mengambil satu nilai setelah melakukan perhitungan pada sekumpulan nilai
  - Type of Aggregate Functions
    - MAX
      fungsi mengembalikan nilai terbesar dari kolom yang dipilih.
  - Type of Aggregate Functions
    - MIN
      fungsi mengembalikan nilai terkecil dari kolom yang dipilih.
  - Type of Aggregate Functions
    - SUM
      fungsi mengembalikan jumlah total kolom numerik.
  - Type of Aggregate Functions
     - COUNT
      fungsi mengembalikan jumlah baris yang cocok dengan kriteria yang ditentukan.
  - Type of Aggregate Functions
     - AVG
      fungsi mengembalikan nilai rata-rata kolom numerik
- UNION
    - Digunakan untuk menggabungkan kumpulan hasil dari dua atau lebih pernyataan SELECT.
    - Setiap pernyataan SELECT dalam UNION harus memiliki jumlah kolom yang sama
    - Kolom juga harus memiliki tipe data yang serupa
    - Kolom dalam setiap pernyataan SELECT juga harus dalam urutan yang sama
- GROUP BY
    - Mengelompokkan baris yang memiliki nilai yang sama ke dalam baris ringkasan
    - Sering digunakan dengan fungsi agregat untuk mengelompokkan kumpulan hasil dengan satu atau lebih kolom.
- HAVING
    - HAVING ditambahkan ke SQL karena kata kunci WHERE tidak dapat digunakan dengan aggregate functions.
- LIKE & Wildcards
    - Operator LIKE digunakan dalam klausa WHERE untuk mencari pola tertentu dalam kolom.
    - Karakter wildcard digunakan untuk menggantikan satu atau lebih karakter dalam sebuah string.
- Wildcard Characters di SQL
   -  % Mewakili nol atau lebih karakter.
    Contoh : %ja% akan cocok dengan belajar, javascript, & jangan
- Wildcard Characters di SQL
    - Mewakili satu karakter.
      Contoh : m_ster akan cocok dengan master & mister

## Authentication & Authorization in Express, JavaScript Authentication

Authentication adalah verifikasi siapa Anda.
Misalnya, katakanlah Anda pergi ke konser. Di pintu depan, penjaga keamanan meminta untuk melihat tiket dan ID Anda untuk memverifikasi bahwa nama di ID Anda cocok dengan nama di tiket Anda.

Otentikasi yang bergantung pada satu faktor, seperti kombinasi nama pengguna/sandi sederhana, disebut Otentikasi Satu Faktor, dan menjadi semakin tidak aman

  &nbsp;
  
Authorization adalah verifikasi atas apa yang boleh Anda lakukan.

Kembali ke contoh konser kami, setelah satpam mengautentikasi Anda, Anda kemudian memberikan tiket Anda ke satpam lain yang kemudian hanya mengizinkan Anda untuk masuk ke Penerimaan Umum (bukan bagian VIP).
  
  &nbsp;
  
Authorization sangat penting untuk keamanan web, dan bertanggung jawab atas segala hal mulai dari mencegah pengguna memodifikasi akun satu sama lain, melindungi aset back-end dari penyerang, hingga memberikan akses terbatas ke layanan eksternal.

  &nbsp;
  
Salah satu alat inti untuk menegakkan otentikasi dan otorisasi adalah enkripsi. Enkripsi adalah proses mengubah data menjadi format yang tidak dapat dibaca kecuali Anda memiliki kunci yang benar untuk mendekripsinya. Enkripsi datang dalam dua jenis utama:

- Symmetric encryption
- Asymmetric encryption

Tanggapan terhadap prompt autentikasi dapat dikategorikan menjadi:

- Knowledge-Based: “Something You Know”
- Possession-Based: “Something You Have”
- Inherence-Based: “Something You Are”

Web Session

Web Session mengacu pada serangkaian interaksi pengguna selama jangka waktu tertentu. Data sesi disimpan di sisi server dan dikaitkan dengan ID sesi.

Pikirkan sesi sebagai memori jangka pendek untuk aplikasi web. Pada latihan berikutnya, kami akan menjelaskan di mana pengidentifikasi sesi ini disimpan sehingga browser (klien) dapat terus mengambil data sesi yang sama di antara pemuatan halaman yang berbeda.

![image_2022-11-12_214039382](https://user-images.githubusercontent.com/80299731/201479332-ddf28013-d9b7-43d7-b649-5e27ef020a6b.png)

![image_2022-11-12_214123847](https://user-images.githubusercontent.com/80299731/201479371-7256f39b-7ca8-4394-8466-e3e82d8984fc.png)

Token Web JSON adalah objek JSON mandiri yang secara kompak dan aman mengirimkan informasi antara dua pihak. Mereka aman karena ditandatangani secara digital menggunakan pasangan kunci rahasia atau publik/pribadi.

   &nbsp;

Sebagai pengingat, JSON, atau Notasi Objek JavaScript, pada dasarnya adalah versi yang sedikit lebih ketat dari objek Javascript.
Objek JSON harus diapit oleh kurung kurawal dan dapat berisi satu atau lebih pasangan nilai kunci

![image_2022-11-12_214621180](https://user-images.githubusercontent.com/80299731/201479596-bd8a8100-25f0-451e-8ef1-ff3ef2680348.png)

Components of a JWT
A JWT is made up of three components:

- Header
- Payload
- Signature

  &nbsp;

 JWT Header berisi jenis token yang kami buat dan algoritma penandatanganan yang akan digunakan.

Jenis: Jenis token ini akan selalu "JWT". Internet Assigned Numbers Authority, atau IANA, mengoordinasikan sumber daya protokol internet di seluruh dunia. Jenis "JWT" ​​sejajar dengan jenis media "application/jwt".

Algoritma: Penandatanganan, atau hashing, algoritma yang digunakan mungkin berbeda. Beberapa algoritma yang umum digunakan adalah HMAC-SHA256, diwakili oleh "HS256", RSA dengan SHA-256, diwakili oleh "RW256", dan ECDSA dengan SHA-256, diwakili oleh "ES256".

  &nbsp;

JWT Payload berisi klaim tentang suatu entitas. Klaim adalah pernyataan atau potongan informasi dan entitas sering kali merupakan pengguna.

![image_2022-11-12_215215164](https://user-images.githubusercontent.com/80299731/201479841-b0847c8a-2f7c-4a31-b05e-23a832868072.png)

JWT Signature digunakan untuk memverifikasi bahwa JWT tidak dirusak atau diubah. Itu dapat dibuat dengan mengambil tajuk yang disandikan, muatan yang disandikan, rahasia, dan menggunakan algoritma hashing untuk membuat hash dari elemen-elemen itu.

Rahasianya adalah kunci simetris yang diketahui oleh pengirim dan penerima token ini.

![image_2022-11-12_215618188](https://user-images.githubusercontent.com/80299731/201480000-2f030a66-6aa4-4f88-9e52-af486ff3cc86.png)


## Sequelize

Sequelize adalah ORM (Object Relational Mapping) Node JS yang berbasis promise. Sequelize mendukung sebagian besar relational Database seperti MySQL, PostgresQL, MariaDB, SQLite dan Miscrosoft SQL Server.
Dengan fitur fitur di Sequelize, kita bisa mengelola dan mengatur data di database kita dengan cepat, dan efisien.

  &nbsp;
  
ORM adalah suatu metode/teknik pemrograman yang digunakan untuk mengkonversi data dari lingkungan bahasa pemrograman berorientasi objek (OOP) dengan lingkungan database relational.  

- Install Sequelize-cli
  Kita perlu menginstall sequelize cli agar dapat menjalankan generator menggunakan terminal sehingga lebih mudah.

                      NPM install -g Sequelize-cli
                      
- Install Sequelize
  Ketika kita melakukan inisiasi project kita pertama perlu menginstall sequelize menggunakan npm install sequelize dan perlu menginstall driver sql yang kita butuhkan
          
                    installing by npm
                    npm install --save sequelize
                    install driver database
                    npm install --save mysql
                    
Sequelize init
Pertama kita perlu melakukan inisialisasi di project kita terlebih dahulu agar dapat melakukan generate code

![image_2022-11-12_221141099](https://user-images.githubusercontent.com/80299731/201480667-aaf8d965-727a-4f0a-bafd-780a0b625777.png)

Generate Model
Mari kita membuat table todo dengan field seperti gambar di bawah

![image_2022-11-12_221245834](https://user-images.githubusercontent.com/80299731/201480700-a22baa20-f04e-48a2-bac7-7efadc31996f.png)

Generate Model
Kita bisa melihat datanya menjadi sebuat class (OOP) dan dapat kita gunakan untuk membuat Rest API menggunakan express atau dapat memberikan behaviour di statenya

  Setelah Model tersedia, maka model tersebut bisa kita gunakan untuk membuat CRUD.

Beberapa endpoint RESTFul :


Get All Todos
Get Todo Detail By Id
Create New Todo
Update Todo By Id
Delete Todo


Generate Model
Akhirnya kita dapat menggunakan generate dan kita bisa mengecek ke database sehingga dapat kita gunakan untuk penimpanan DB

![image_2022-11-12_221538827](https://user-images.githubusercontent.com/80299731/201480798-ad619f96-b474-4ccd-8889-1aa6dca74feb.png)


Jika ada yang salah, kita bisa mengembalikan (undo) menggunakan :

![image_2022-11-12_221608406](https://user-images.githubusercontent.com/80299731/201480822-8825d293-68a1-40f2-8a9d-daee4faa27e3.png)

Generate Seed
Seed adalah data awal yang bisa kita gunakan untuk mengisi data di database untuk keperluan awal project menggunakan sequelize

![image_2022-11-12_221726484](https://user-images.githubusercontent.com/80299731/201480902-ad9fc71d-a856-4083-9507-16d5dc4c39b2.png)

Membuat CRUD Dengan Express dan Sequelize

   &nbsp;

Setelah Model tersedia, maka model tersebut bisa kita gunakan untuk membuat CRUD.
Beberapa endpoint RESTFul :

- Get All Todos
- Get Todo Detail By Id
- Create New Todo
- Update Todo By Id
- Delete Todo

- Get All Todo
   Untuk Kita akan membuat sebuah routing entuk get all todo dengan syntax berikut 
   
![image_2022-11-12_222042742](https://user-images.githubusercontent.com/80299731/201481050-fce3a046-9327-4caa-8dfc-01b8c8340749.png)
                                                        
- Get Todo Detail By Id
Untuk Kita akan membuat sebuah routing entuk get detail todo berdasarkan Id todo dengan syntax berikut

![image_2022-11-12_222330337](https://user-images.githubusercontent.com/80299731/201481156-bf99deea-1d80-4e01-b016-28c26258a6a0.png)

- Create New Todo
Untuk Kita akan membuat sebuah routing entuk create new todo dengan syntax berikut

![image_2022-11-12_222510278](https://user-images.githubusercontent.com/80299731/201481213-765f57eb-b528-43b0-98c5-c09f8a38ac8a.png)

- Update Todo By Id
Untuk Kita akan membuat sebuah routing entuk update todo by Id dengan syntax berikut

![image_2022-11-12_222607519](https://user-images.githubusercontent.com/80299731/201481249-502e2efd-0536-47d9-a65d-28343279aacd.png)

- Delete Todo By Id
Untuk Kita akan membuat sebuah routing entuk delete todo by Id dengan syntax berikut
![image_2022-11-12_222716083](https://user-images.githubusercontent.com/80299731/201481298-ec072db4-6a92-4ce3-aeae-1f30fb048cff.png)
                   
