# **Rangkuman Week6**

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
## Sequelize
