# **Rangkuman Week4**
## JavaScript Intermediate - Asynchronous - Fetch

                  const verseChoose = document.querySelector('select');
                  const poemDisplay = document.querySelector('pre');

                  verseChoose.addEventListener('change', () => {
                    const verse = verseChoose.value;
                    updateDisplay(verse);
                  });
                  
                  
Mari kita definisikan fungsi updateDisplay() kita. Pertama-tama, letakkan kode berikut di bawah blok kode Anda sebelumnya — ini adalah cangkang kosong dari fungsi tersebut.

                    function updateDisplay(verse) {

                    }
                    

## JavaScript Intermdiate - Asynchronous - Async Await
JavaScript asinkron
Dalam modul ini, kita melihat JavaScript asinkron, mengapa itu penting, dan bagaimana itu dapat digunakan untuk menangani operasi pemblokiran potensial secara efektif, seperti mengambil sumber daya dari server.


                    // ============== Menampilkan data digimon pada web ============

                    // belum pakai fetch.......................
                    // pakai data dummy
                    let listDigimonNonFetch = document.getElementById("list-digimon-non-fetch")
                    let digimons = ["Agumon", "Gabumon", "Patamon"]

                    digimons.forEach(item => {
                      console.log(item)
                      listDigimonNonFetch.innerHTML += `<h3>${item}</h3>`

                      // alternative
                      // let textDigimon = document.createElement("h3")
                      // textDigimon.innerText = item
                      // containerDigimon.append(textDigimon)
                    })

                    // sesudah pakai fetch......................
                    // async await
                    listDigimon = document.getElementById("list-digimon")

                    let getDataDigimon = async () => {
                      let URL = "https://digimon-api.vercel.app/api/digimon"
                      let response = await fetch(URL)
                      let digimons = await response.json()

                      // menampilkan 10 data digimon
                      digimons.slice(0, 10).forEach((item, index) => {
                          listDigimon.innerHTML += 
                          `<div>
                            <img src="${item.img}" alt="" width="200">
                            <h3>${item.name}</h3>
                          </div>`
                      })
                    }

                    getDataDigimon()

## Git & Github Lanjutan
### cara berkolaborasi kelompok di Github
**<div align="justify">Team Leader**
  <div align="justify">Buat Organization
  <div align="justify">1. Team lead membuat organization
  <div align="justify">2. Invite anggota tim jadikan owner
  
  &nbsp;
  
 Buat Repo di organization 
 1. team lead but repo untuk yang akan dibuat
 2. Repo dibuat public, dan ceklis REadmi
 3. buat branch benama dev 
    
 Mengecek pull request
 1. setiap ada pull request, team lead akan mengeceknya
 2. jika pull request belum sesuai, bisa dikasih komen atau beri kabar anggota yang melakukan pull request tersebut
 3. jika sudah selesai lakukan merge 
    &nbsp;
    
 Tahap yang dilakukan seluruh anggota 
 1. masing masing anggota lakukan clone pada repo yang sudah dibuat 
 2. bagi tugas pada masing masing anggota kelompok 
 3. sebelum ngoding lakukan git full untuk update kode terbaru 
 4. anggota membuat branch dari dev
 5. lakukan pengerjaan didalam branch yang dibuat
 6. jika fitur sudah selesai code dari dev lakukan commit seperti biasa 
 7. sebelum push, lakukan git marge dev untuk menghindari confict di github
 8. jika sudah confict, berskan semuahnya 
 9. jika sudah aman, commit lalu push branch ke git hub
 10. lakukan pull request untuk marge ke branch dev
 11. tunggu pull request di acc team lead

## Responsive Web Design
apa yang dimaksud responsive web disain 
adalah membuat desain website yang dapat di akses dalam device manapun, device yang umum digunakan adalah laptop/pc, smartphone dan tablet     

    CONTOH di html 
                    <!DOCTYPE html>
                    <html lang="en">
                      <head>
                        <meta charset="UTF-8" />
                        <meta http-equiv="X-UA-Compatible" content="IE=edge" />
                        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
                        <title>Document</title>

                        <link rel="stylesheet" href="style.css">
                      </head>
                      <body>

                        <nav>
                          <div>
                            <h1>Zan</h1>
                          </div>

                          <div class="toggle-menu"></div>
                          <ul class="menu">
                            <li><a href="">Home</a></li>
                            <li><a href="">About</a></li>
                            <li><a href="">Contact</a></li>
                          </ul>
                        </nav>

                        <div class="container">
                          <img src="https://img.freepik.com/premium-vector/meadows-landscape-with-mountains-hill_104785-943.jpg?w=2000" alt="">
                        </div>

                        <div class="container">
                          <p class="rem">hallo ini dari rem</p>
                        </div>

                        <div class="container">
                          <p class="em">hallo ini dari em</p>
                        </div>

                      </body>
                    </html>
    
 
  Contoh di css 
 
    
                      * {
                    font-style: none;
                    list-style: none;
                  }

                  nav {
                    display: flex;
                    justify-content: space-between;
                  }

                  .menu {
                    display: flex;
                    justify-content: space-around;
                  }

                  .menu li {
                    margin: 0 2rem;
                  }

                  .container {
                    font-size: 20px;
                    width: 500px;
                    background-color: bisque;
                  }

                  /* font-size dari root 16px */
                  .rem {
                    font-size: 2rem;
                  }

                  .em {
                    font-size: 2em;
                  } 

                  img {
                    /* width: 50vw; */
                    /* height: 50vh; */
                    width: 80%;
                  }

                  @media (max-width: 600px ) {
                    .menu {
                      display: none;
                    }

                    .toggle-menu {
                      width: 40px;
                      height: 40px;
                      background: url(./menu.svg);
                      background-position: center;
                      background-repeat: no-repeat;
                      background-size: 30px;
                      background-repeat: no-repeat;
                    }
                  }
    
## Bootstrap 5
Bootstrap adalah toolkit frontend yang kuat dan penuh fitur. Bangun apa pun—dari prototipe hingga produksi—dalam hitungan menit.
    
Tujuan dan fungsi Bootstrap adalah untuk membuat website responsive dan mobile-first. Jadi, semua elemen antarmuka website dipastikan bisa bekerja secara optimal di semua ukuran layar, baik desktop maupun perangkat seluler



Dokumentasi Bootstrap yang Lengkap
    
**<div align="justify">Konten** ‒ menyediakan kompilasi source code Bootstrap.
**<div align="justify">Browser dan perangkat** ‒ mencantumkan semua browser web dan mobile yang didukung, serta komponen berbasis seluler.
**<div align="justify">JavaScript** ‒ menguraikan berbagai plugin JS yang dikembangkan berdasarkan jQuery.
**<div align="justify">Tema** ‒ menjelaskan variabel Sass bawaan untuk penyesuaian yang lebih mudah.
**<div align="justify">Alat** ‒ mengajarkan cara menggunakan skrip npm Bootstrap untuk berbagai tindakan.
**<div align="justify">Aksesibilitas** ‒ mencakup fitur dan batasan Bootstrap terkait markup struktural, komponen, kontras warna, visibilitas konten, dan efek 
    
    
                     <!DOCTYPE html>
                    <html lang="en">
                      <head>
                        <meta charset="UTF-8" />
                        <meta http-equiv="X-UA-Compatible" content="IE=edge" />
                        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
                        <title>Document</title>

                        <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.2/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-              Zenh87qX5JnK2Jl0vWa8Ck2rdkQ2Bzep5IDxbcnCeuOxjzrPF/et3URy9Bv1WTRi" crossorigin="anonymous">
                        <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.2.2/dist/js/bootstrap.bundle.min.js" integrity="sha384-OERcA2EqjJCMA+/3y+gxIOqMEjwtxJY7qPCqsdltbNJuaOe923+mo//f6V8Qbsw3" crossorigin="anonymous"></script>

                        <link rel="stylesheet" href="style.css">
                      </head>
                      <body>
                        <nav class="navbar navbar-expand-lg custom-navbar">
                          <div class="container-fluid">
                            <a class="navbar-brand" href="#">Navbar</a>
                            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
                              <span class="navbar-toggler-icon"></span>
                            </button>
                            <div class="collapse navbar-collapse" id="navbarSupportedContent">
                              <ul class="navbar-nav me-auto mb-2 mb-lg-0">
                                <li class="nav-item">
                                  <a class="nav-link active" aria-current="page" href="#">Home</a>
                                </li>
                                <li class="nav-item">
                                  <a class="nav-link" href="#">Link</a>
                                </li>
                                <li class="nav-item dropdown">
                                  <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                                    Dropdown
                                  </a>
                                  <ul class="dropdown-menu">
                                    <li><a class="dropdown-item" href="#">Action</a></li>
                                    <li><a class="dropdown-item" href="#">Another action</a></li>
                                    <li><hr class="dropdown-divider"></li>
                                    <li><a class="dropdown-item" href="#">Something else here</a></li>
                                  </ul>
                                </li>
                                <li class="nav-item">
                                  <a class="nav-link disabled">Disabled</a>
                                </li>
                              </ul>
                              <form class="d-flex" role="search">
                                <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search">
                                <button class="btn btn-outline-success" type="submit">Search</button>
                              </form>
                            </div>
                          </div>
                        </nav>

                        <div class="container mt-5 ">
                          <div class="row align-items-center justify-content-between mb-5">
                            <div class="col-4">
                              <h1>Hai.. I'm Auzan</h1>
                            </div>

                            <div class="col-4">
                              <img src="./me.png" alt="" width="300">
                            </div>
                          </div>

                          <div class="row row-cols-1 row-cols-md-2 g-4">
                            <div class="col">
                              <div class="card">
                                <img src="..." class="card-img-top" alt="...">
                                <div class="card-body">
                                  <h5 class="card-title">Card title</h5>
                                  <p class="card-text">This is a longer card with supporting text below as a natural lead-in to additional content. This content is a little bit longer.</p>
                                </div>
                              </div>
                            </div>
                            <div class="col">
                              <div class="card">
                                <img src="..." class="card-img-top" alt="...">
                                <div class="card-body">
                                  <h5 class="card-title">Card title</h5>
                                  <p class="card-text">This is a longer card with supporting text below as a natural lead-in to additional content. This content is a little bit longer.</p>
                                </div>
                              </div>
                            </div>
                            <div class="col">
                              <div class="card">
                                <img src="..." class="card-img-top" alt="...">
                                <div class="card-body">
                                  <h5 class="card-title">Card title</h5>
                                  <p class="card-text">This is a longer card with supporting text below as a natural lead-in to additional content.</p>
                                </div>
                              </div>
                            </div>
                            <div class="col">
                              <div class="card">
                                <img src="..." class="card-img-top" alt="...">
                                <div class="card-body">
                                  <h5 class="card-title">Card title</h5>
                                  <p class="card-text">This is a longer card with supporting text below as a natural lead-in to additional content. This content is a little bit longer.</p>
                                </div>
                              </div>
                            </div>
                          </div>
                        </div>



                      </body>
                    </html>
    
    
    
    
 contoh di css 
    
              .custom-navbar {
            background-color: aquamarine;
          }
