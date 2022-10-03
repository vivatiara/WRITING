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
             
  ```html
  let a = 5
let b = a
console.log(a) // 5
console.log(b) // 5
console.log(a === b) // true
a = 10
console.log(a) // 10
console.log(b) // 5
console.log(a === b) // false ```

 
