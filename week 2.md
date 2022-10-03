# **Rangkuman Week2**

## Js Dasar-Scope

- ### Function
 <div align="justify">Function adalah sebuah blok kode dalam sebuah grup untuk menyelesaikan 1 task/1 fitur. Saat kita membutuhkan fitur tersebut nantinya, kita bisa kembali menggunakannya.
 &nbsp;
 
 - Jenis-jenis Function
  - Function Declaration
 <div align="justify">Function Declaration dibuat menggunakan kata kunci function diikuti dengan nama fungsi (wajib), lalu parameter di dalam sepasang kurung lengkung (parameter1, parameter2, ..., parameterN), diakhiri dengan kurung kurawal {...} untuk membatasi badan fungsi.
  
   <div align="justify">Sintaks :
 
 ```
    function name(param) {
  statements;
}
 ```
  Keterangan:

 <div align="justify">1. name: nama fungsi.
 <div align="justify">2. param (opsional): parameter atau nama untuk nilai argumen yang diteruskan ke fungsi, batas parameter bergantung pada mesin, jika                             parameter lebih dari satu dipisahkan dengan koma.
 <div align="justify">3. statements (opsional): statement atau pernyataan termasuk ekspresi, logika, perulangan dan sebagainya.
  
<div align="justify"> Contoh   
  
```
  function apakahGenap(num) {
  return num % 2 === 0;
}

apakahGenap(1); // false
apakahGenap(2); // true
``` 
function apakahGenap(num) { ... } adalah Function Declaration, kita mendeklarasikan fungsi bernama apakahGenap untuk menentukan apakah suatu bilangan genap. 
 
- Function Expression
  <div align="justify">Mirip seperti Function Declaration, Function Expression dibuat menggunakan kata kunci function, diikuti dengan nama fungsi (opsional), lalu parameter di dalam kurung lengkung (param1, param2, ..., paramN), diakhiri dengan kurung kurawan { ... } sebagai pembatas badan fungsi.
   
    <div align="justify">Sintaks :
```
     function name(param) {
  statements;
}
```
 Keterangan:

<div align="justify">1. name (opsional): nama fungsi, biasanya dibuat tanpa nama.
<div align="justify">2. param (opsional): parameter atau nama untuk nilai argumen yang diteruskan ke fungsi, batas parameter bergantung pada mesin, jika                             parameter lebih dari satu dipisahkan dengan koma.
<div align="justify">3. statements (opsional): statement atau pernyataan termasuk ekspresi, logika, perulangan dan sebagainya.

- ### Scope
<div align="justify">Scope adalah konsep dalam flow data variabel. Untuk menentukan suatu variabel bisa diakses pada scope tertentu atau tidak.

 <div align="justify">Sintaks :
 ``` 
 // dibagian ini variabel 'makanan' tidak dapat diakses
function simpleFunction(){
  var makanan = "Bakso";
  // jika variabel 'makanan' ditaruh di dalam sini maka variabel 'makanan' dapat diakses
}
```
  - Global Scope berarti variabel yang kita buat dapat diakses dimanapun dalam suatu file. Agar menjadi Global Scope, suatu variabel harus dideklarasikan     diluar Blocks.
 
<div align="justify"> sintaks : 

```
 var makanan = "Bakso";  
// disini kamu bisa menggunakan variabel 'makanan'
function simpleFunction() {   
// disini kamu bisa menggunakan variabel 'makanan'
}
```
 
  - Local scope berarti kita mendeklarasikan variabel didalam blocks seperti function, conditional, dan looping.Maka variabel hanya bisa diakses didalam blocks saja. Tidak bisa diakses diluar blocks.
 


- ### Blocks
<div align="justify">Blocks adalah code yang berada didalam curly braces {}. Conditional, function, dan  looping menggunakan blocks.
 
 
## Data Type Built in Prototype & Method
- ### Data Type
   - **String**
      <div align="justify"> String digunakan untuk mewakili dan memanipulasi urutan karakter, String berguna untuk menyimpan data yang dapat direpresentasikan dalam bentuk teks. Secara umum, ada dua jenis tipe data, yaitu tipe string yang mendominasi karakter atau huruf, dan tipe string yang mendominasi angka.
   
   - **Number**
       <div align="justify">Number adalah objek pembungkus primitif yang digunakan untuk mewakili dan memanipulasi angka seperti 37 atau -9,25.
       <div align="justify">Nilai dari tipe lain dapat dikonversi ke angka menggunakan fungsi Number().
       
   - **Math**
       <div align="justify">Math adalah objek bawaan yang memiliki properti dan metode untuk konstanta dan fungsi matematika. Ini bukan objek fungsi.
        
   - **Primitive & Non Primitive**
        - Primitive
        <div align="justify">Tipe data primitif menentukan ukuran dan tipe nilai variabel, dan tidak memiliki metode tambahan.
         
        - Non Primitive
         <div align="justify">Tipe data non-primitif disebut tipe referensi karena mereka merujuk ke objek
          
        - Perbedaan utama antara tipe data primitif dan non-primitif adalah:

          - Jenis primitif sudah ditentukan sebelumnya (sudah ditentukan) di Java. Tipe non-primitif dibuat oleh programmer dan tidak ditentukan oleh Java                (kecuali untuk String).
          - Tipe non-primitif bisa digunakan untuk memanggil metode untuk melakukan operasi tertentu, sedangkan tipe primitif tidak bisa.
          - Tipe primitif selalu memiliki nilai, sedangkan tipe non-primitif bisa null.
          - Tipe primitif dimulai dengan huruf kecil, sedangkan tipe non-primitif dimulai dengan huruf besar.
          - Ukuran tipe primitif bergantung pada tipe datanya, sedangkan tipe non-primitif memiliki ukuran yang sama.
        
        - **Primitive**
            <div align="justify">1. Numbers
            <div align="justify">2. Strings
            <div align="justify">3. Booleans
            <div align="justify">4. undefined
            <div align="justify">5. null
             
        - **Non-Primitive** (referred to collectively as Objects)
            <div align="justify">1. Objects
            <div align="justify">2. Arrays
            <div align="justify">3. Functions
             
             
            - contoh bagaimana Primitif disimpan:
             
  ```
  let a = 5
  let b = a
  console.log(a) // 5
  console.log(b) // 5
  console.log(a === b) // true
  a = 10
  console.log(a) // 10
  console.log(b) // 5
  console.log(a === b) // false 
  ```
             
  - contoh            
  ```           
  var title = "Belajar Pemrograman Javascript";
  ```
Pada contoh di atas, kita membuat variabel bernama title dengan nilai berupa teks (string): "Belajar Pemrograman Javascript".

 - contoh let 
```            
 // membuat variabel dengan kata kunci let
let price = 15000;

// membuat variabel tanpa awalan apapun
stock = 12
```
Apa bedanya yang menggunakan var, let dan yang tanpa awalan?
Perbedaannya terletak pada jangkauan dan penggunaannya. Nanti kita akan bahas lebih dalam lagi.
             
-  Menampilkan isi Variabel
 <div align="justify">Fungsi console.log() menampilkan output ke console javascript;
 <div align="justify">Fungsi document.write() menampilkan output ke dokumen HTML;
 <div align="justify">dan Fungsi alert() menampilkan output ke jendela dialog.

```
  <!DOCTYPE html>
<html lang="en">
<head>
    <title>Belajar Variabel dalam Javascript</title>
    <script>
        // membuat variabel
        var name = "Petani Kode";
        var visitorCount = 50322;
        var isActive = true;
        var url = "https://www.petanikode.com";

        // menampilkan variabel ke jendela dialog (alert)
        alert("Selamat datang di " + name);
    
        // menampilkan variabel ke dalam HTML
        document.write("Nama Situs: " + name + "<br>");
        document.write("Jumlah Pengunjung: " + visitorCount + "<br>");
        document.write("Status Aktif: " + isActive + "<br>");
        document.write("Alamat URL: " + url + "<br>");
    </script>
</head>
<body>
    

</body>
</html>
```
  
  Hasilnya di browser
  
  ![image_2022-10-03_225458541](https://user-images.githubusercontent.com/80299731/193622467-d58c2e32-1657-4b73-ba53-7a60fc85c8dd.png)
             
 ## DOM
 - ### Apa itu DOM
   <div align="justify">DOM merupakan singkatan dari Document Object Model. Artinya, dokumen (HTML) yang dimodelkan dalam sebuah objek. Objek dari dokumen ini menyediakan sekumpulan fungsi dan atribut/data yang bisa kita manfaatkan dalam membuat program Javascript. Inilah yang disebut API (Application Programming Interface). DOM tidak hanya untuk dokumen HTML saja. DOM juga bisa digunakan untuk dokumen XML dan SVG. DOM juga tidak hanya ada di Javascript saja, DOM juga ada pada bahasa pemrograman lain.
    
- ### Bagaimana Cara Menggunakan DOM?
  <div align="justify">Objek DOM di javascript bernama **Document** Objek ini berisi segala hal yang kita butuhkan untuk memanipulasi HTML. Jika kita coba ketik document pada console Javascript, maka yang akan tampil adalah kode HTML.
   
   - Sebagai contoh fungsi documen.write().
   
   ```
   document.write("Hello World");
   document.write("<h2>Saya Sedang Belajar Javascript</h2>");
   
   ```
    Hasilnya di browser
   
     ![Capture](https://user-images.githubusercontent.com/80299731/193601105-f14c5c1e-85bc-4434-9715-2cdc67678922.JPG)
   
   -  Apabila kita ingin mengakses elemen yang spesifik, terdapat beberapa fungsi yang bisa digunakan:
   
      - **getElementById()** fungsi untuk memilih elemen berdasarkan atribut id.
      - **getElementByName()** fungsi untuk memilih elemen berdasarkan atribut name.
      - **getElementByClassName()** fungsi untuk memilih elemen berdasarkan atribut class.
      - **getElementByTagName()** fungsi untuk memilih elemen berdasarkan nama tag.
      - **getElementByTagNameNS()** fungsi untuk memilih elemen berdasarkan nama tag.
      - **querySelector()** fungsi untuk memilih elemen berdasarkan query.
      - **querySelectorAll()** fungsi untuk memilih elemen berdasarkan query.
      dan lain-lain.
   
   - Contoh Misalkan kita punya kode HTML seperti ini:
    
   ```
   <div id="tutorial"></div>
   ```
   
   Maka untuk memilih element tersebut di Javascript, kita bisa gunakan fungsi getElementByI() seperti ini:
   
   ```
   // memilih elemen dengan id 'tutorial'
   var tutorial = document.getElementById('tutorial');
   ```
   
   Variabel tutorial akan menjadi sebuah objek DOM dari elemen yang kita pilih.
   
 ```
   <!DOCTYPE html>
<html>
<head>
    <title>Memilih Elemen Berdasarkan ID</title>
</head>
<body>

    <!-- Elemen div yang akan kita pilih dari JS -->
    <div id="tutorial"></div>


    <script type="text/javascript">
        // mengakses elemen tutorial
        var tutorial = document.getElementById("tutorial");

        // mengisi teks ke dalam elemen
        tutorial.innerText = "Tutorial Javascript";

        // memberikan CSS ke elemen
        tutorial.style.backgroundColor = "gold";
        tutorial.style.padding = "10px";

    </script>

</body>
</html>
   
```
  
   Hasilnya di browser
   
   ![image_2022-10-03_213709113](https://user-images.githubusercontent.com/80299731/193604657-0f112adf-94df-4be4-805e-d46a9510bc11.png)
   
     - EventListener
       <div align="justify">Dengan cara Element.addEventListener(“event”)
         - Bisa dihilangkan
         - Bisa ada beberapa event listener yang sama untuk 1 element
         - Memiliki argument tambahan { options }

   - EventListener - Click
     <div align="justify">Misalkan kita mempunyai element <input id=”user-input” />  dan <button id=”alert-button”>show</button>. Kita ingin menampilkan pop        up box yang berisi teks di dalam input tadi.

   - EventListener - Blur
     <div align="justify"> Blur”, lawan dari “focus”, adalah event di mana sebuah element kehilangan fokus dari user (misal user klk mouse di luar element          tersebut atau user klik tab untuk berpindah element), Misalkan kita ingin memvalidasi isi dari <input id=”username” /> agar panjangnya minimal 6       karakter

   - EventListener - Form Submission
     <div align="justify"> Misalkan kita mempunyai element beberapa input dalam sebuah form <input name=”email /> dan <input type=”password” name=”password”/>. Bagaimana caranya  kita mendapatkan isi dari kedua input tersebut saat submit form?






   
            
             

 
