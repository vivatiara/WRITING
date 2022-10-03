# **Rangkuman Week2**

## Js Dasar-Scope

- ### Function
 <div align="justify">Function adalah sebuah blok kode dalam sebuah grup untuk menyelesaikan 1 task/1 fitur. Saat kita membutuhkan fitur tersebut nantinya, kita bisa kembali menggunakannya.
 &nbsp;

- ### Scope
<div align="justify">Scope adalah konsep dalam flow data variabel. Untuk menentukan suatu variabel bisa diakses pada scope tertentu atau tidak.

  - Global Scope berarti variabel yang kita buat dapat diakses dimanapun dalam suatu file. Agar menjadi Global Scope, suatu variabel harus dideklarasikan     diluar Blocks.

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


   
            
             

 
