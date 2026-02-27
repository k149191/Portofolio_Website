# Portofolio Website
## Nama: Khairunisa Aprilia
## Kelas: B Sistem Informasi 24
## NIM: 2409116060

# A. Deskripsi Website
Website ini merupakan portfolio pribadi Khairunisa Aprilia yang menampilkan informasi profil, kemampuan, serta sertifikat yang dimiliki. Website dibuat dengan tampilan modern, responsif, dan mudah dinavigasi menggunakan Bootstrap 5 dan CSS kustom. Tujuan utama website ini adalah sebagai media personal branding.

# B. Tampilan Website
  ## 1. Section Navigaation Bar
  Section Navigation Bar berada di bagian paling atas website dan berfungsi sebagai menu navigasi utama.
  
  <p align="center">
  <img width="1919" height="111" alt="image" src="https://github.com/user-attachments/assets/db05fb3a-a356-4230-83d0-ea0a5c0abfc8" />
  </p>

  <p align="center">
  <img width="1132" height="111" alt="image" src="https://github.com/user-attachments/assets/b41b41c5-0275-4665-92ed-de4a591584ba" />
  </p>
  
  Isi:
  - Logo “K.a”
  - Menu Home
  - Menu About Me
  - Menu Certificate
  - Responsive hamburger menu

  ## 2. Section Home
  Section Home merupakan hero section yang menjadi tampilan pembuka website yang berisi deskripsi/informasi singkat .
  
  <p align="center">
  <img width="1919" height="869" alt="image" src="https://github.com/user-attachments/assets/b025962c-da3e-461b-901d-b6abcbd472bc" />
  </p>

  <p align="center">
  <img width="1011" height="996" alt="image" src="https://github.com/user-attachments/assets/1e1e1608-8d96-4de1-b402-68248bf84342" />
  </p>

  Isi:
  - Sapaan “Hello, I’m Kai”
  - Deskripsi singkat sebagai mahasiswa Sistem Informasi
  - Informasi kontak (telepon & email)
  - Foto profil berbentuk lingkaran
  
  ## 3. Section About Me
  Section About Me berisi deskripsi diri dan skill menggunakan tools/aplikasi. Section ini menunjukkan latar belakang serta level kemampuan yang dimiliki.

  <p align="center">
  <img width="1919" height="981" alt="image" src="https://github.com/user-attachments/assets/6cf5c532-6382-4607-9d61-5d080b36c81c" />
  </p>

  <p align="center">
  <img width="909" height="1004" alt="image" src="https://github.com/user-attachments/assets/1168454b-ddd1-4bc4-97b8-be3bbd7694bd" />
  </p>

  Isi:
  - Paragraf perkenalan diri
  - Judul “My Learning Journey”
  - Progress bar kemampuan bahasa dan tools

  ## 4. Section My Certificate
  Section My Certificate menampilkan daftar sertifikat dalam bentuk grid card. Section ini berfungsi sebagai bukti pengalaman dan pencapaian.
  
  <p align="center">
  <img width="1907" height="1015" alt="image" src="https://github.com/user-attachments/assets/c7dd2e22-4021-436b-a84f-42ad8125a6b7" />
  </p>

  Isi:
  - Judul section
  - Card sertifikat
  - Gambar sertifikat
  - Nama kegiatan
  - Tanggal
  

# C. Penjelasan Code
  ## 1. Section Navigaation Bar
  HTML:
  ```
<!--Navbar-->
<nav class="navbar navbar-expand-lg navbar-dark custom-navbar py-3">
  <div class="container position-relative">
    <a class="navbar-brand logo-circle" href="K:\Semester_4\PBW\portofolio_website\material\K.png">K.a</a>
    <div class="mx-auto d-none d-lg-block">
      <ul class="navbar-nav flex-row gap-5 fw-semibold nav-center">
        <li class="nav-item"><a class="nav-link active" href="#home">Home</a></li>
        <li class="nav-item"><a class="nav-link" href="#about">About Me</a></li>
        <li class="nav-item"><a class="nav-link" href="#certificate">Certificate</a></li>
      </ul>
    </div>
    <button class="menu-circle navbar-toggler border-0" type="button" data-bs-toggle="collapse" data-bs-target="#navMobile">
      <span class="navbar-toggler-icon"></span>
    </button>
  </div>
</nav>
```

  Penjelasan: 
```
•	Tag <nav class='navbar navbar-expand-lg navbar-dark custom-navbar py-3'> digunakan untuk membuat navigation bar responsif dengan Bootstrap. Navbar akan melebar di layar besar dan collapse di layar kecil.
•	Elemen <div class='container position-relative'> berfungsi sebagai pembungkus agar isi navbar terpusat dan rapi.
•	Tag <a class='navbar-brand logo-circle'>K.a</a> menampilkan logo website. Class logo-circle digunakan untuk membuat logo berbentuk lingkaran.
•	Menu navigasi menggunakan <ul class='navbar-nav flex-row gap-5 fw-semibold nav-center'> sehingga item menu tersusun horizontal, memiliki jarak antar menu, dan teks terlihat lebih tegas.
•	Setiap <a class='nav-link' href='#home'>, <a href='#about'>, dan <a href='#certificate'> berfungsi sebagai anchor link untuk berpindah ke section terkait.
•	Tombol <button class='menu-circle navbar-toggler'> digunakan sebagai hamburger menu pada tampilan mobile untuk membuka dan menutup menu.
```

  CSS:
```
.custom-navbar {
  background: #2b0b6f;
  border-bottom: 4px solid #d9d9d9;
}

.nav-center .nav-link {
  color: #ffffff;
  font-family: 'Playfair Display', serif;
  font-size: 22px;
}

.nav-center .nav-link:hover {
  opacity: 0.8;
}

.logo-circle {
  background: #ffffff;
  color: #000;
  width: 48px;
  height: 48px;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  font-weight: 600;
}

.menu-circle {
  background: #ffffff;
  border-radius: 50%;
  width: 48px;
  height: 48px;
}

.menu-circle .navbar-toggler-icon {
  filter: invert(1);
}
```

  Penjelasan:
```
•	Class .custom-navbar mengatur warna background navbar menjadi ungu gelap dan menambahkan garis bawah sebagai aksen.
•	Class .nav-center .nav-link mengatur warna teks menu menjadi putih, menggunakan font Playfair Display, dan memperbesar ukuran teks.
•	Selector .nav-center .nav-link:hover memberikan efek transparansi saat kursor diarahkan ke menu agar terlihat interaktif.
•	Class .logo-circle membuat logo berbentuk lingkaran dengan ukuran tetap serta posisi teks berada di tengah.
•	Class .menu-circle membuat tombol hamburger berbentuk lingkaran agar konsisten dengan desain.
•	Selector .menu-circle .navbar-toggler-icon menggunakan filter invert untuk membalik warna ikon hamburger agar tetap terlihat jelas.
```

  ## 2. Section Home

  HTML:
  ```
<!--Homw-->
<section id="home" class="hero-section">
  <div class="container">
    <div class="row align-items-center">
      <div class="col-lg-6 text-center text-lg-start">
        <h1 class="fw-bold">Hello, I’m Kai</h1>
        <p class="subtitle">A Information System Student in Mulawarman University.</p>
        <div class="contact">
          <p class="mb-1">📞 089693416561</p>
          <p>✉️ khaiairilia@gmail.com</p>
        </div>
      </div>
      <div class="col-lg-6 text-center">
      <div class="profile-wrapper">
        <img src="K:\Semester_4\PBW\portofolio_website\material\PDH KAI - NO BG.png" alt="profile" class="profile-img">
      </div>
    </div>
    </div>
  </div>
</section>
  ```
  Penjelasan:
  ```
•	Tag <section id='home' class='hero-section'> merupakan hero section sebagai tampilan pembuka.
•	Grid Bootstrap (row dan col-lg-6) membagi layout menjadi dua kolom antara teks dan gambar.
•	Judul dan subtitle menampilkan perkenalan singkat pengguna.
•	Class profile-wrapper membungkus foto agar tampil dalam frame lingkaran.

  ```
  CSS:
  ```
.hero-section {
  padding: 80px 0;
}

.subtitle {
  color: #555;
}

.profile-wrapper {
  position: relative;
  width: 360px;
  height: 360px;
  margin: auto;
  border-radius: 50%;
  background: #dcdce2;
  display: flex;
  align-items: flex-end;
  justify-content: center;
  overflow: hidden;
}

.profile-wrapper::before {
  content: "";
  position: absolute;
  width: 290px;
  height: 290px;
  border-radius: 50%;
  background: #cfcfd6;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}

.profile-img {
  position: relative;
  width: 300px;
  height: auto;       
  object-fit: contain; 
  z-index: 2;
}

  ```
  Penjelasan:
  ```
•	Class .hero-section memberi jarak vertikal pada hero.
•	Class .profile-wrapper dan .profile-img mengatur tampilan foto profil agar berada dalam frame lingkaran.
  ```

  ## 3. Section About Me

  HTML:
  ```
<!--About Me-->
<section id="about" class="about-section">
  <div class="container">
    <div class="about-card mx-auto text-center">
      <p>
        My name is Khairunisa Aprilia, an Information Systems student at Mulawarman
        University. I am currently focusing on developing my skills in web development,
        data visualization, and database design through academic and personal projects.
        I enjoy learning step by step and turning ideas into structured and useful digital
        solutions. I am continuously improving both my technical and writing skills as I
        grow in the technology field.
      </p>
    </div>

    <h3 class="text-center mt-5 mb-4">My Learning Journey</h3>
    <div class="row g-4">

      <div class="col-md-6">
        <label>Indonesian Language - Native</label>
        <div class="progress">
          <div class="progress-bar" style="width:92%"></div>
        </div>
      </div>
      <div class="col-md-6">
        <label>English - Beginner</label>
        <div class="progress">
          <div class="progress-bar" style="width:40%"></div>
        </div>
      </div>
      <div class="col-md-6">
        <label>Canva</label>
        <div class="progress">
          <div class="progress-bar" style="width:97%"></div>
        </div>
      </div>
      <div class="col-md-6">
        <label>Figma</label>
        <div class="progress">
          <div class="progress-bar" style="width:40%"></div>
        </div>
      </div>
      <div class="col-md-6">
        <label>Affinity</label>
        <div class="progress">
          <div class="progress-bar" style="width:50%"></div>
        </div>
      </div>
      <div class="col-md-6">
        <label>HTML</label>
        <div class="progress">
          <div class="progress-bar" style="width:20%"></div>
        </div>
      </div>
    </div>
  </div>
</section>

```
  Penjelasan:
  ```
•	Tag <section id='about' class='about-section'> digunakan untuk bagian profil dan skill.
•	Class about-card menampilkan deskripsi diri dalam bentuk card.
•	Judul My Learning Journey memperkenalkan bagian skill.
•	Komponen progress dan progress-bar digunakan untuk menampilkan persentase kemampuan.

```
  CSS:
  ```
.about-section {
  background: #e9e9ed;
  padding: 70px 0;
}

.about-card {
  background: #2b0b6f;
  color: white;
  padding: 30px;
  border-radius: 15px;
  max-width: 800px;
}

.progress {
  height: 10px;
  background-color: #cfcfd6;
}

.progress-bar {
  background: #2b0b6f;
}
```
  Penjelasan:
  ```
•	Class .about-section dan .about-card mengatur tampilan section About.
•	Class .progress dan .progress-bar mengatur tampilan bar kemampuan.
```
  
  ## 4. Section My Certificate

HTML:
  ```
<!--Certificate-->
<section id="certificate" class="certificate-section">
  <div class="container">
    <h2 class="text-center mb-5">My Certificate</h2>
    <div class="row g-4">
      <div class="col-md-6 col-lg-4">
        <div class="cert-card">
          <img src="K:\Semester_4\PBW\portofolio_website\material\INFORSA.png" alt="certificate" class="cert-img img-fluid">
          <h6>Information System Association</h6>
          <small>30 December 2025</small>
        </div>
      </div>
      <div class="col-md-6 col-lg-4">
        <div class="cert-card">
          <img src="K:\Semester_4\PBW\portofolio_website\material\MAKRAB TAROT.png" alt="certificate" class="cert-img img-fluid">
          <h6>Malam Keakraban</h6>
          <small>13 December 2024</small>
        </div>
      </div>
      <div class="col-md-6 col-lg-4">
        <div class="cert-card">
          <img src="K:\Semester_4\PBW\portofolio_website\material\PUBDIG.png" alt="certificate" class="cert-img img-fluid">
          <h6>Public Digital</h6>
          <small>13 September 2025</small>
        </div>
      </div>
    </div>
  </div>
</section>
```

Penjelasan:
  ```
•	Tag <section id='certificate' class='certificate-section'> menampilkan daftar sertifikat.
•	Grid Bootstrap digunakan agar card sertifikat responsive.
•	Class cert-card membungkus setiap sertifikat.
•	Class cert-img mengatur tampilan gambar sertifikat agar rapi.

```

CSS:
  ```
.certificate-section {
  padding: 80px 0;
}

.cert-card {
  background: #e5e5e5;
  padding: 20px;
  border-radius: 24px;
  transition: transform 0.25s ease, box-shadow 0.25s ease;
}

.cert-img {
  width: 100%;
  aspect-ratio: 1.414 / 1;   
  object-fit: contain;   
  background: #f3f3f7;
  border-radius: 14px;
  padding: 10px;
  margin-bottom: 14px;
}
```

Penjelasan:
  ```
•	Class .certificate-section, .cert-card, dan .cert-img mengatur layout dan tampilan sertifikat.
```

# D. Teknologi Yang Digunakan
Teknologi yang digunakan untuk membuat website portofolio ini adalah:
1. HTML5
2. CSS3
3. Bootstrap

<p align="center">
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white">
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white">
  <img src="https://img.shields.io/badge/Bootstrap-7952B3?style=for-the-badge&logo=bootstrap&logoColor=white">
</p>
