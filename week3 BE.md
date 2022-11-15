# **Rangkuman Week3 BE**
## Sequelize

Installing

              npm install --save sequelize
      
menginstal driver secara manual untuk database:
One of the following:
- $ npm install --save pg pg-hstore # Postgres
- $ npm install --save mysql2
- $ npm install --save mariadb
- $ npm install --save sqlite3
- $ npm install --save tedious # Microsoft SQL Server
- $ npm install --save oracledb # Oracle Database


Untuk terhubung ke database, Anda harus membuat instance Sequelize. Ini dapat dilakukan dengan melewatkan parameter koneksi secara terpisah ke konstruktor Sequelize atau dengan mengirimkan URI koneksi tunggal:

                      const { Sequelize } = require('sequelize');

                      // Option 1: Passing a connection URI
                      const sequelize = new Sequelize('sqlite::memory:') // Example for sqlite
                      const sequelize = new Sequelize('postgres://user:pass@example.com:5432/dbname') // Example for postgres

                      // Option 2: Passing parameters separately (sqlite)
                      const sequelize = new Sequelize({
                        dialect: 'sqlite',
                        storage: 'path/to/database.sqlite'
                      });

                      // Option 3: Passing parameters separately (other dialects)
                      const sequelize = new Sequelize('database', 'username', 'password', {
                        host: 'localhost',
                        dialect: 
                      });
                      
                      
Testing the connection

                     try {
                      await sequelize.authenticate();
                      console.log('Connection has been established successfully.');
                    } catch (error) {
                      console.error('Unable to connect to the database:', error);
                    }
                    
Sequelize akan membuat koneksi tetap terbuka secara default, dan menggunakan koneksi yang sama untuk semua kueri. Jika Anda perlu menutup koneksi, panggil sequelize.close() (yang asinkron dan mengembalikan Promise).

Tip untuk membaca dokumen
Anda dianjurkan untuk menjalankan contoh kode secara lokal saat membaca dokumen Sequelize. Ini akan membantu Anda belajar lebih cepat. Cara termudah untuk melakukannya adalah dengan menggunakan dialek SQLite:

                      const { Sequelize, Op, Model, DataTypes } = require("sequelize");
                      const sequelize = new Sequelize("sqlite::memory:");

## MongoDB

MongoDB adalah salah satu database open source NoSQL yang cukup populer digunakan. MongoDB sering dipakai untuk aplikasi berbasis Cloud, Big Data maupun Grid COmputing. Jika SQL menyimpan data menggunakan relasi tabel, MongoDB menggunakan dokumen dengan format JSON

- Apa itu SQL?
SQL atau Structured Query Language yang merupakan suatu bahasa yang digunakan utuk mengelolah data di dalam database relasional.

- Apa itu NoSQL?
NoSQL atau biasa disebut Not Only SQL, menyediakan mekanisme penyimpanan dan pengambilan data yang tidak terstruktur.

- NoSQL adalah Not Only SQL
Artinya kita bisa mengolah database dengan fleksibel dan tidak membutuhkan Query

 Kelebihan  MongoDB sebagai salah satu NoSQL
- Sistem tidak membutuhkan Tabel
- Tidak perlu menggunakan Tabel yang terstruktur
- By Default sudah menggunakan JSON(JavaScript Object Notation), sehingga memudahkan integrasi dengan JavaScript
- Performa lebih cepat dengan kemampuan menampung banyak data yang bervariasi

 Kekurangan MongoDB sebagai salah satu NoSQL
- Tidak mendukung transaksi
- Masalah konsistensi data
- Menggunakan banyak memory
- Hanya bisa menampung maksimal 16MB disetiap document


Cara Install MongoDB di Windows
- Pertama, anda dapat mendownload MongoDB pada situs resmi -nya.
- Selanjutnya, melakukan proses instalasi dengan mengikuti panduan dalam installer yang tersedia. Setelah berhasil terpasang, anda perlu melakukan konfigurasi terkait MongoDB Environment dengan cara membuat folder data untuk menyimpan database. Jangan lupa untuk mendaftarkan dalam “path” juga.
- Untuk dapat menjalankan MongoDB, anda perlu masuk pada fitur CMD (Command Prompt) Windows dengan mengetikkan “C:\mongodb\bin\mongod.exe”. Perintah tersebut bertujuan untuk menjalankan server milik MongoDB.
- Dan langkah selanjutnya, untuk menghubungkan dengan MongoDB, anda dapat menjalankan file “mongo.exe” dan menekan perintah “connecting to: test”. Apabila telah muncul tampilan shell -nya, maka anda telah berhasil terhubung dengan server MongoDB.

Cara Kerja MongoDB
- Mengkoneksikan dengan MongoDB
- Membuat Database Baru
- Membuat Dokumen Baru
- Melakukan Query Find
- Menggunakan Query Update dan Remove

Run MongoDB Community Edition from the Command Interpreter
- Create database directory.

          cd C:\
          md "\data\db"
        
 - Start your MongoDB database. To start MongoDB, run exe
         "C:\Program Files\MongoDB\Server\6.0\bin\mongod.exe" --dbpath="c:\data\db"
         
 - Connect to MongoDB.
 Jika Anda belum melakukannya, ikuti petunjuk pemasangan mongosh untuk mengunduh dan menginstal MongoDB Shell (mongosh).

## Mongoose

MongoDB adalah salah satu produk database noSQL Open Source yang menggunakan struktur data JSON untuk menyimpan datanya.
MongoDB sering dipakai untuk aplikasi berbasis Cloud, Grid Computing, atau Big Data.

Contoh NoSQL document

![image_2022-11-15_214655357](https://user-images.githubusercontent.com/80299731/201948866-9aad8995-1860-42b4-b172-d4adc3d28951.png)

Install dotenv untuk menampung variabel environment database. Dan juga install MongoDB

![image_2022-11-15_215017720](https://user-images.githubusercontent.com/80299731/201949688-23030737-e914-41fc-87c6-66279c54cd29.png)

Buat satu file .env untuk menyimpan variabel database

![image_2022-11-15_215108313](https://user-images.githubusercontent.com/80299731/201949873-69660e22-2424-48db-92ef-803795db3c1d.png)




## Docker

Docker adalah software yang menjalankan suatu aplikasi menggunakan container
Docker men-sharing kernel dari host OS, serta meng-container-kan suatu aplikasi agar dapat dijalankan dimana saja dan kapan saja 
Aplikasi yg berjalan di dalam container docker tidak terpengaruh oleh faktor luar karena terisolasi

- Docker berfungsi sebagai penyedia layanan virtual bagi aplikasi yg diinstall pada sebuah host. Docker akan menyediakan hal-hal yang diperlukan untuk aplikasi mulai dari akses file, koneksi internet, hingga port agar aplikasi dapat berjalan dengan mulus

- Menggunakan Docker memungkinkan Anda mengirimkan kode lebih cepat, menstandardisasi operasi aplikasi, memindahkan kode dengan lancar, dan menghemat uang dengan meningkatkan pemanfaatan sumber daya. Dengan Docker, Anda mendapatkan satu objek yang dapat dijalankan di mana saja.

- Definisi Container adalah sejenis software yang mengemas dan mengisolasi applikasi secara virtual untuk mempermudah software deployment. Berbeda dengan konsep traditional Virtual Machine, Container tidak membutuhkan dedicated operating system (OS Kernel) tetapi Container Kernel dapat di pergunakan secara bersamaan.

- Docker-Compose adalah alat untuk mendefinisikan dan menjalankan satu atau beberapa container yang saling terkait dengan sebuah command. 
    - Proses Dasar Penggunaan Docker-Compose :

       - Mendefinisikan environment aplikasi dengan membuat Dockerfile sehingga bisa digunakan kembali dimana saja.
       -  Mendefinisikan service lainnya (termasuk aplikasi kita) di dalam docker-compose.yml sehingga semuanya bisa berjalan bersamaan dalam environment yang terisolasi.
       -  Jalankan command docker compose yaitu : docker-compose build dan docker-compose up melalui command prompt/shell (pastikan anda berada pada path yang sama dengan posisi file docker-compose.yml).

Docker compose Command
- docker-compose build : digunakan untuk mem-build semua service yang telah didefinisikan pada docker-compose.yml, output dari command ini adalah image per service yang siap untuk dijalankan pada sebuah container. Default nama image yang dihasilkan adalah [namafolder-posisi-file_docker-compose.yml]_[nama_service]
- docker-compose up : digunakan untuk menjalankan semua image yang telah di-build ( docker-compose build ), jika tidak terjadi masalah maka image tersebut menjadi running container sedangkan jika terdapat masalah maka biasanya akan terbentuk container yang posisinya berhenti/stop. 
- docker-compose down : Menghentikan (stop) semua container dan me-remove nya (ingat stop tidak otomatis remove) semua container, networks, volumes, dan images yang dihasilkan oleh perintah up
- docker-compose logs : command ini penting jika kita ingin melihat apa yg terjadi pada service tertentu saat dijalankan dalam container.
- ocker-compose config : digunakan untuk mengecek apakah script yang ada pada file docker-compose.yml yang telah kita buat sudah valid atau sudah sesuai dengan referensi dari docker-compose.
- Masih banyak command lain yang bisa digunakan, tetapi pada umumnya command tersebut hampir sama dengan command docker (start, run, kill, ps, dll).
