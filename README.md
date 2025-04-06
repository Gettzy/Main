<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Alkatani Group</title>
  <style>
    body {
      font-family: sans-serif;
      margin: 0;
      padding: 0;
    }

    /* Sidebar */
    .sidebar {
      height: 100%;
      width: 250px;
      position: fixed;
      top: 0;
      left: -250px;
      background-color: #1e3a8a;
      padding-top: 60px;
      transition: 0.3s;
      z-index: 1000;
    }

    .sidebar a {
      display: block;
      color: white;
      padding: 1rem 1.5rem;
      text-decoration: none;
    }

    .sidebar a:hover {
      background-color: #2563eb;
    }

    /* Hamburger button */
    .hamburger {
      position: fixed;
      top: 15px;
      left: 15px;
      z-index: 1100;
      cursor: pointer;
      background: none;
      border: none;
      font-size: 24px;
      color: #1e3a8a;
    }

    main {
      margin-left: 0;
      padding: 2rem;
      transition: margin-left 0.3s;
    }

    .logo-container {
      display: flex;
      align-items: center;
      gap: 1rem;
      padding: 1rem;
    }

    .logo-container img {
      width: 40px;
    }

    h2 {
      color: #1e40af;
    }

    .logo-row {
      display: flex;
      justify-content: center;
      gap: 2rem;
      margin-bottom: 1rem;
    }

    .contact-form input, .contact-form textarea {
      width: 100%;
      margin-bottom: 1rem;
      padding: 0.5rem;
      border: 1px solid #ccc;
      border-radius: 5px;
    }

    .contact-form button {
      background-color: #2563eb;
      color: white;
      padding: 0.5rem 1rem;
      border: none;
      border-radius: 5px;
    }

    /* Overlay */
    .overlay {
      display: none;
      position: fixed;
      top: 0;
      left: 0;
      height: 100vh;
      width: 100vw;
      background: rgba(0, 0, 0, 0.4);
      z-index: 900;
    }
  </style>
</head>
<body>
  <!-- Hamburger Button -->
  <button class="hamburger" onclick="toggleSidebar()">☰</button>

  <!-- Sidebar -->
  <div id="sidebar" class="sidebar">
    <div class="logo-container">
      <img src="Image/AlkataniGroup.jpg" alt="Alkatani Group" />
      <h3 style="color:white; margin: 0;">Alkatani Group</h3>
    </div>
    <a href="#beranda">Beranda</a>
    <a href="#tentang">Tentang Kami</a>
    <a href="#visi-misi">Visi & Misi</a>
    <a href="#berita">Berita</a>
    <a href="#kontak">Kontak</a>
  </div>

  <!-- Overlay -->
  <div id="overlay" class="overlay" onclick="toggleSidebar()"></div>

  <!-- Main Content -->
  <main id="main">
    <section id="beranda" style="text-align: center;">
      <h2>Selamat Datang di Alkatani Group</h2>
      <p>Inovasi dan Kolaborasi untuk Masa Depan Berkelanjutan.</p>
      <button onclick="alert('Fitur ini masih dalam pengembangan')">Pelajari Lebih Lanjut</button>
    </section>

    <section id="tentang">
      <h2>Tentang Kami</h2>
      <p>Alkatani Group adalah perusahaan yang bergerak di bidang agribisnis, teknologi, dan industri kreatif. Kami membangun merek, komunitas, dan solusi berkelanjutan untuk masa depan.</p>
    </section>

    <section id="visi-misi">
      <h2>Visi & Misi</h2>
      <h3>Visi</h3>
      <p>Menjadi perusahaan berbasis inovasi yang berdampak global dan membangun masa depan yang berkelanjutan.</p>
      <h3>Misi</h3>
      <ul>
        <li>Mengembangkan produk dan layanan berbasis potensi lokal.</li>
        <li>Mendukung ekosistem esports, olahraga, dan komunitas kreatif.</li>
        <li>Mendorong transformasi digital dan pemberdayaan ekonomi hijau.</li>
      </ul>
    </section>

    <section id="berita">
      <h2>Berita Terbaru</h2>
      <div>
        <h3>Peluncuran Resmi Team Yama Esport</h3>
        <p><small>6 April 2025</small></p>
        <p>Team Yama Esport resmi diluncurkan sebagai bagian dari Alkatani Group, membawa semangat baru dalam dunia kompetitif Free Fire dan Mobile Legends.</p>
      </div>
      <div>
        <h3>Produk Skincare Berbasis Lidah Buaya Segera Hadir</h3>
        <p><small>30 Maret 2025</small></p>
        <p>Alkatani Group sedang mengembangkan lini skincare alami dengan bahan utama lidah buaya dan vanili. Produk ini akan mengusung merek Lydaluxe atau Veranuque.</p>
      </div>
    </section>

    <section id="kontak">
      <h2>Hubungi Kami</h2>
      <p>Kirim pertanyaan atau kerja sama lewat formulir ini.</p>
      <form class="contact-form">
        <input type="text" name="user_name" placeholder="Nama Anda" required />
        <input type="email" name="user_email" placeholder="Email Anda" required />
        <textarea name="message" rows="4" placeholder="Tulis pesan..." required></textarea>
        <button type="submit">Kirim</button>
      </form>
    </section>
  </main>

<footer>
  <div class="logo-row">
    <img src="Image/AlkataniGroup.jpg" alt="Logo Alkatani" width="40" height="40" />
    <img src="Image/Team-Yama-GG.png" alt="Logo Team Yama" width="40" height="50" />
    <img src="Image/SundaraLebakFC.png" alt="Logo Sundara Lebak FC" width="40" height="40" />
    <img src="Image/SundaraVC.png" alt="Logo Sundara VC" width="40" height="40" />
    <img src="Image/Lydaluxe.png" alt="Logo Lydaluxe" width="40" height="40" />
  </div>

  <div style="margin: 1rem 0; text-align: center;">
<!-- Media Sosial -->
<div class="logo-row" style="margin-top: 1rem;">
  <a href="https://www.instagram.com/alkatani.pazri?igsh=ZG00Nm1tcG85amZw" target="_blank">
    <img src="Image/Instagram.png" alt="Instagram" width="32" height="32" />
  </a>
  <a href="https://Wa.me/6285718244652" target="_blank">
    <img src="Image/Whatsapp.png" alt="Whatsapp" width="32" height="32" />
  </a>
</div>

  <p style="text-align: center;">&copy; 2025 Alkatani Group. All rights reserved.</p>
</footer>

  <script>
    function toggleSidebar() {
      const sidebar = document.getElementById("sidebar");
      const overlay = document.getElementById("overlay");
      if (sidebar.style.left === "0px") {
        sidebar.style.left = "-250px";
        overlay.style.display = "none";
      } else {
        sidebar.style.left = "0px";
        overlay.style.display = "block";
      }
    }
  </script>
</body>
</html>
