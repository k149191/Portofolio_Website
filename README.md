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
  - Kode <nav class="navbar navbar-expand-lg navbar-dark custom-navbar py-3"> digunakan untuk membuat navigation bar yang responsif menggunakan Bootstrap 5. Navbar akan tampil penuh di layar besar dan collapse di layar kecil.
  - Bagian logo menggunakan <a class="navbar-brand logo-circle"> yang menampilkan teks “K.a” sebagai identitas website. Class logo-circle pada CSS membuat logo berbentuk lingkaran.
  - Menu navigasi dibuat dengan <ul class="navbar-nav flex-row gap-5 fw-semibold nav-center"> yang berfungsi menyusun menu secara horizontal, memberi jarak antar menu, serta membuat teks menu lebih tebal.
  - Setiap menu (Home, About Me, Certificate) menggunakan anchor link (#home, #about, #certificate) sehingga pengguna dapat berpindah ke section terkait dengan cepat.
  - Tombol hamburger dengan class navbar-toggler dan menu-circle digunakan untuk tampilan mobile agar menu dapat dibuka dan ditutup pada layar kecil.
  - Pada CSS, class .custom-navbar mengatur warna background navbar menjadi ungu gelap dan menambahkan garis bawah sebagai aksen.
  - Class .nav-center .nav-link mengatur warna teks menu menjadi putih, font lebih elegan, serta ukuran lebih besar, sedangkan efek hover dibuat lebih transparan agar terlihat interaktif.
  - Class .logo-circle dan .menu-circle digunakan untuk membuat logo dan tombol hamburger berbentuk lingkaran sehingga tampilan navbar terlihat lebih modern dan konsisten.

  ## 2. Section Home

  ```
kode
```
  
  ## 3. Section About Me

  ```
kode
```
  
  ## 4. Section My Certificate

  ```
kode
```

# D. Teknologi Yang Digunakan
