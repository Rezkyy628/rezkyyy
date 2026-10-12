never forget who made you successful


<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#080b0a">
<title>REZKY ADITYA | Personal Website</title>

<style>
:root {
  --bg: #080b0a;
  --card: #111714;
  --green: #9dff65;
  --text: #f4f7f4;
  --muted: #9ba69e;
  --border: #26312a;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

html {
  scroll-behavior: smooth;
  scroll-padding-top: 85px;
}

body {
  font-family: Arial, Helvetica, sans-serif;
  background: var(--bg);
  color: var(--text);
  line-height: 1.6;
  overflow-x: hidden;
}

a {
  color: inherit;
  text-decoration: none;
}

button, input {
  font: inherit;
}

button {
  cursor: pointer;
}

.container {
  width: min(1100px, 90%);
  margin: auto;
}

header {
  position: sticky;
  top: 0;
  z-index: 100;
  background: rgba(8, 11, 10, .94);
  backdrop-filter: blur(12px);
  border-bottom: 1px solid var(--border);
}

.navbar {
  min-height: 70px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 20px;
}

.logo {
  color: var(--green);
  font-weight: 900;
  letter-spacing: 1px;
  font-size: 19px;
}

.nav-links {
  display: flex;
  align-items: center;
  gap: 22px;
}

.nav-links a {
  color: #d3dbd5;
  font-size: 13px;
  transition: .2s;
}

.nav-links a:hover {
  color: var(--green);
}

.hero {
  min-height: 85vh;
  display: grid;
  grid-template-columns: 1.2fr .8fr;
  align-items: center;
  gap: 50px;
  padding: 70px 0;
}

.tag {
  display: inline-block;
  padding: 7px 13px;
  color: var(--green);
  border: 1px solid #3d5d35;
  background: #142015;
  border-radius: 30px;
  font-size: 12px;
  margin-bottom: 20px;
}

.hero h1 {
  font-size: clamp(38px, 7vw, 68px);
  line-height: 1.1;
  margin-bottom: 20px;
  overflow-wrap: anywhere;
}

.hero h1 span {
  color: var(--green);
}

.hero p {
  color: var(--muted);
  max-width: 520px;
  font-size: 15px;
}

.hero-buttons {
  display: flex;
  flex-wrap: wrap;
  gap: 12px;
  margin-top: 28px;
}

.btn {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  gap: 9px;
  border: 1px solid var(--border);
  border-radius: 10px;
  padding: 12px 17px;
  font-weight: bold;
  font-size: 13px;
  transition: .2s;
}

.btn-primary {
  background: var(--green);
  color: #10170d;
  border-color: var(--green);
}

.btn-secondary {
  background: var(--card);
  color: white;
}

.btn:hover {
  transform: translateY(-3px);
}

.profile-frame {
  width: min(100%, 340px);
  aspect-ratio: 4 / 5;
  margin: auto;
  padding: 10px;
  border: 1px solid #47683e;
  border-radius: 24px;
  background: linear-gradient(145deg, #1c3020, #0b100d);
  box-shadow: 0 0 55px #9dff6510;
}

.profile-frame img {
  width: 100%;
  height: 100%;
  display: block;
  object-fit: cover;
  border-radius: 17px;
}

.section {
  padding: 75px 0;
}

.section-title {
  font-size: clamp(26px, 4vw, 38px);
  margin-bottom: 10px;
}

.section-title span {
  color: var(--green);
}

.section-desc {
  color: var(--muted);
  font-size: 14px;
  margin-bottom: 32px;
}

.about-card {
  background: var(--card);
  border: 1px solid var(--border);
  border-radius: 18px;
  padding: 28px;
}

.about-card p {
  color: #c2ccc4;
  margin-bottom: 22px;
}

.info-grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 13px;
}

.info-item {
  background: #0b100d;
  border: 1px solid var(--border);
  padding: 15px;
  border-radius: 12px;
  min-width: 0;
}

.info-label {
  color: var(--muted);
  font-size: 12px;
  display: block;
  margin-bottom: 4px;
}

.info-value {
  font-size: 14px;
  font-weight: bold;
  overflow-wrap: anywhere;
}

.info-value a:hover {
  color: var(--green);
}

.hobby-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 9px;
  margin-top: 23px;
}

.hobby-tag {
  background: #19251a;
  border: 1px solid #344d30;
  color: var(--green);
  border-radius: 30px;
  padding: 8px 12px;
  font-size: 12px;
}

/* INSTAGRAM-STYLE POSTS */
.posts-grid {
  display: grid;
  grid-template-columns: repeat(3, minmax(0, 1fr));
  gap: 20px;
  align-items: start;
}

.post {
  background: #101411;
  border: 1px solid var(--border);
  border-radius: 15px;
  overflow: hidden;
  min-width: 0;
}

.post-header {
  display: flex;
  align-items: center;
  gap: 10px;
  padding: 13px;
}

.avatar {
  width: 38px;
  height: 38px;
  flex-shrink: 0;
  border-radius: 50%;
  object-fit: cover;
  border: 2px solid var(--green);
}

.post-user {
  font-size: 13px;
  font-weight: bold;
}

.post-location {
  font-size: 11px;
  color: var(--muted);
}

.post-image {
  width: 100%;
  aspect-ratio: 4 / 4.5;
  display: block;
  object-fit: cover;
  background: #1a211c;
  cursor: pointer;
  transition: transform .25s;
}

.post-image:active {
  transform: scale(.99);
}

.post-actions {
  display: flex;
  align-items: center;
  gap: 17px;
  padding: 12px 13px 3px;
}

.action-btn {
  display: inline-flex;
  align-items: center;
  gap: 6px;
  border: none;
  color: #f4f7f4;
  background: transparent;
  font-size: 13px;
  padding: 2px 0;
}

.action-btn svg {
  width: 24px;
  height: 24px;
  stroke: currentColor;
  fill: none;
  stroke-width: 1.8;
  stroke-linecap: round;
  stroke-linejoin: round;
}

.action-btn:hover {
  color: var(--green);
}

.like-btn.liked {
  color: #ff526c;
}

.like-btn.liked svg {
  fill: #ff526c;
  stroke: #ff526c;
}

.share-btn {
  margin-left: auto;
}

.post-likes {
  padding: 5px 13px 0;
  font-size: 12px;
  font-weight: bold;
}

.post-caption {
  padding: 5px 13px 10px;
  font-size: 12px;
  color: #d4dcd5;
  overflow-wrap: anywhere;
}

.post-caption strong {
  color: white;
  margin-right: 5px;
}

.comment-list {
  padding: 0 13px 8px;
  font-size: 12px;
  overflow-wrap: anywhere;
}

.comment {
  margin-top: 6px;
  color: #cbd4cd;
}

.comment strong {
  color: white;
  margin-right: 5px;
}

.comment-form {
  display: flex;
  gap: 7px;
  padding: 10px 12px;
  border-top: 1px solid #222b24;
}

.comment-form input {
  width: 100%;
  min-width: 0;
  background: transparent;
  color: white;
  border: none;
  outline: none;
  font-size: 12px;
}

.comment-form input::placeholder {
  color: #849087;
}

.comment-form button {
  background: transparent;
  color: var(--green);
  border: none;
  font-weight: bold;
  font-size: 12px;
}

.contact-card {
  background: linear-gradient(145deg, #142016, #101411);
  border: 1px solid #344d30;
  padding: 30px;
  border-radius: 18px;
  text-align: center;
}

.contact-card p {
  color: var(--muted);
  margin: 10px auto 22px;
  max-width: 480px;
  font-size: 14px;
}

.contact-buttons {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  gap: 12px;
}

.social-icon {
  width: 20px;
  height: 20px;
  flex-shrink: 0;
  display: inline-block;
}

.social-icon svg {
  width: 100%;
  height: 100%;
  display: block;
  fill: currentColor;
}

footer {
  border-top: 1px solid var(--border);
  padding: 23px 0;
  color: var(--muted);
  text-align: center;
  font-size: 12px;
}

footer span {
  color: var(--green);
}

@media (max-width: 760px) {
  .nav-links {
    gap: 12px;
  }

  .nav-links a {
    font-size: 11px;
  }

  .hero {
    grid-template-columns: 1fr;
    text-align: center;
    gap: 35px;
    padding: 65px 0;
  }

  .hero p {
    margin: auto;
  }

  .hero-buttons {
    justify-content: center;
  }

  .profile-frame {
    width: min(75%, 300px);
  }

  .posts-grid {
    grid-template-columns: 1fr;
    max-width: 480px;
    margin: auto;
    gap: 24px;
  }

  .post-image {
    aspect-ratio: 1 / 1;
  }
}

@media (max-width: 380px) {
  .container {
    width: 92%;
  }

  .navbar {
    min-height: 62px;
  }

  .logo {
    font-size: 15px;
  }

  .nav-links {
    gap: 9px;
  }

  .nav-links a {
    font-size: 10px;
  }

  .info-grid {
    grid-template-columns: 1fr;
  }

  .about-card,
  .contact-card {
    padding: 20px;
  }
}
</style>
</head>

<body>

<header>
  <div class="container navbar">
    <a class="logo" href="#home">REZKY<span> ADITYA.</span></a>

    <nav class="nav-links">
      <a href="#home">Home</a>
      <a href="#tentang">Tentang</a>
      <a href="#hobi">Hobi</a>
      <a href="#kontak">Kontak</a>
    </nav>
  </div>
</header>

<main>
  <!-- HOME -->
  <section class="container hero" id="home">
    <div>
      <span class="tag">PERSONAL WEBSITE</span>

      <h1>Halo, Saya<br><span>REZKY ADITYA</span></h1>

      <p>
        Selamat datang di website pribadi saya.
        Di sini kamu bisa mengenal saya lebih dekat,
        melihat hobi saya, dan menghubungi saya melalui
        media sosial.
      </p>

      <div class="hero-buttons">
        <a class="btn btn-primary" href="#tentang">Tentang Saya</a>

        <a class="btn btn-secondary"
           href="https://wa.me/6283897256809"
           target="_blank" rel="noopener noreferrer">

          <span class="social-icon" aria-hidden="true">
            <svg viewBox="0 0 24 24">
              <path d="M20.5 3.5A11.8 11.8 0 0 0 12.1 0C5.6 0 .3 5.3.3 11.8c0 2.1.6 4.2 1.6 6L0 24l6.4-1.7a12 12 0 0 0 5.7 1.4h.1c6.5 0 11.8-5.3 11.8-11.8 0-3.2-1.2-6.2-3.5-8.4ZM12.1 21.7c-1.8 0-3.5-.5-5-1.4l-.4-.2-3.8 1 1-3.7-.3-.4a9.8 9.8 0 1 1 8.5 4.7Zm5.4-7.3c-.3-.2-1.8-.9-2.1-1-.3-.1-.5-.2-.7.2-.2.3-.8 1-1 1.2-.2.2-.4.2-.7.1-.3-.2-1.3-.5-2.5-1.5-.9-.8-1.5-1.8-1.7-2.1-.2-.3 0-.5.1-.7l.5-.6c.2-.2.2-.3.3-.6.1-.2 0-.4 0-.6-.1-.2-.7-1.7-.9-2.3-.3-.6-.5-.5-.7-.5h-.6c-.2 0-.6.1-.9.4-.3.3-1.2 1.2-1.2 2.8s1.2 3.2 1.4 3.4c.2.2 2.4 3.7 5.8 5.1.8.4 1.5.6 2 .7.8.3 1.6.2 2.2.1.7-.1 1.8-.7 2-1.4.3-.7.3-1.3.2-1.4-.1-.2-.3-.3-.6-.4Z"/>
            </svg>
          </span>
          WhatsApp
        </a>
      </div>
    </div>

    <div class="profile-frame">
      <img src="foto.jpg"
           alt="Foto profil REZKY ADITYA"
           onerror="this.onerror=null;this.src='https://placehold.co/600x750/111714/9dff65?text=FOTO+REZKY';">
    </div>
  </section>

  <!-- TENTANG SAYA -->
  <section class="section" id="tentang">
    <div class="container">
      <h2 class="section-title">Tentang <span>Saya</span></h2>
      <p class="section-desc">Sedikit informasi tentang diri saya.</p>

      <div class="about-card">
        <p>
          Halo! Saya <strong>REZKY ADITYA</strong>.
          Saya adalah siswa kelas XII TKJ 1.
          Saya suka melakukan berbagai kegiatan,
          terutama bermain bola, jalan-jalan, dan menonton Formula 1.
        </p>

        <div class="info-grid">
          <div class="info-item">
            <span class="info-label">Nama Lengkap</span>
            <span class="info-value">REZKY ADITYA</span>
          </div>

          <div class="info-item">
            <span class="info-label">Kelas</span>
            <span class="info-value">XII TKJ 1</span>
          </div>

          <div class="info-item">
            <span class="info-label">WhatsApp</span>
            <span class="info-value">
              <a href="https://wa.me/6283897256809"
                 target="_blank" rel="noopener noreferrer">
                0838-9725-6809
              </a>
            </span>
          </div>

          <div class="info-item">
            <span class="info-label">Instagram</span>
            <span class="info-value">
              <a href="https://instagram.com/kyy_cavalry"
                 target="_blank" rel="noopener noreferrer">
                @kyy_cavalry
              </a>
            </span>
          </div>
        </div>

        <div class="hobby-tags">
          <span class="hobby-tag">⚽ Bermain Bola</span>
          <span class="hobby-tag">🌄 Jalan jalan</span>
          <span class="hobby-tag">🏎️ Menonton Formula 1</span>
        </div>
      </div>
    </div>
  </section>

  <!-- POSTINGAN HOBI -->
  <section class="section" id="hobi">
    <div class="container">
      <h2 class="section-title">Hal yang <span>Saya Suka</span></h2>
      <p class="section-desc">
        Beberapa hobi saya dalam tampilan seperti postingan Instagram.
      </p>

      <div class="posts-grid">

        <!-- POST 1: SEPAK BOLA -->
        <article class="post" data-id="bola">
          <div class="post-header">
            <img class="avatar" src="foto.jpg" alt="Foto profil"
                 onerror="this.onerror=null;this.src='https://placehold.co/100x100/111714/9dff65?text=R';">
            <div>
              <div class="post-user">kyy_cavalry</div>
              <div class="post-location">⚽ Sepak Bola</div>
            </div>
          </div>

          <img class="post-image"
               src="bola.jpg"
               alt="Foto hobi bermain bola"
               onerror="this.onerror=null;this.src='https://placehold.co/600x700/111714/9dff65?text=FOTO+SEPAK+BOLA';">

          <div class="post-actions">
            <button class="action-btn like-btn" aria-label="Like postingan">
              <svg viewBox="0 0 24 24">
                <path d="M20.8 4.6a5.5 5.5 0 0 0-7.8 0L12 5.7l-1.1-1.1a5.5 5.5 0 0 0-7.8 7.8l1.1 1.1L12 21l7.8-7.5 1.1-1.1a5.5 5.5 0 0 0-.1-7.8Z"/>
              </svg>
            </button>

            <button class="action-btn comment-focus" aria-label="Komentar">
              <svg viewBox="0 0 24 24">
                <path d="M21 11.5a8.4 8.4 0 0 1-.9 3.8 8.5 8.5 0 0 1-7.6 4.7 8.4 8.4 0 0 1-3.8-.9L3 21l1.9-5.7a8.4 8.4 0 0 1-.9-3.8 8.5 8.5 0 0 1 4.7-7.6 8.4 8.4 0 0 1 3.8-.9h.5a8.5 8.5 0 0 1 8 8v.5Z"/>
              </svg>
            </button>

            <button class="action-btn share-btn" aria-label="Bagikan postingan">
              <svg viewBox="0 0 24 24">
                <path d="m22 2-7 20-4-9-9-4Z"/>
                <path d="M22 2 11 13"/>
              </svg>
            </button>
          </div>

          <div class="post-likes">0 suka</div>
          <div class="post-caption">
            <strong>kyy_cavalry</strong>
            Bermain bola adalah salah satu hobi favorit saya! ⚽🔥
          </div>
          <div class="comment-list"></div>

          <form class="comment-form">
            <input type="text" placeholder="Tambahkan komentar..."
                   aria-label="Tulis komentar" maxlength="300">
            <button type="submit">Kirim</button>
          </form>
        </article>

        <!-- POST 2: JALAN-JALAN -->
        <article class="post" data-id="jalan">
          <div class="post-header">
            <img class="avatar" src="foto.jpg" alt="Foto profil"
                 onerror="this.onerror=null;this.src='https://placehold.co/100x100/111714/9dff65?text=R';">
            <div>
              <div class="post-user">kyy_cavalry</div>
              <div class="post-location">🌄 Jalan-jalan</div>
            </div>
          </div>

          <img class="post-image"
               src="jalan.jpg"
               alt="Foto hobi jalan-jalan"
               onerror="this.onerror=null;this.src='https://placehold.co/600x700/111714/9dff65?text=FOTO+JALAN-JALAN';">

          <div class="post-actions">
            <button class="action-btn like-btn" aria-label="Like postingan">
              <svg viewBox="0 0 24 24">
                <path d="M20.8 4.6a5.5 5.5 0 0 0-7.8 0L12 5.7l-1.1-1.1a5.5 5.5 0 0 0-7.8 7.8l1.1 1.1L12 21l7.8-7.5 1.1-1.1a5.5 5.5 0 0 0-.1-7.8Z"/>
              </svg>
            </button>

            <button class="action-btn comment-focus" aria-label="Komentar">
              <svg viewBox="0 0 24 24">
                <path d="M21 11.5a8.4 8.4 0 0 1-.9 3.8 8.5 8.5 0 0 1-7.6 4.7 8.4 8.4 0 0 1-3.8-.9L3 21l1.9-5.7a8.4 8.4 0 0 1-.9-3.8 8.5 8.5 0 0 1 4.7-7.6 8.4 8.4 0 0 1 3.8-.9h.5a8.5 8.5 0 0 1 8 8v.5Z"/>
              </svg>
            </button>

            <button class="action-btn share-btn" aria-label="Bagikan postingan">
              <svg viewBox="0 0 24 24">
                <path d="m22 2-7 20-4-9-9-4Z"/>
                <path d="M22 2 11 13"/>
              </svg>
            </button>
          </div>

          <div class="post-likes">0 suka</div>
          <div class="post-caption">
            <strong>kyy_cavalry</strong>
            Menjelajahi tempat baru dan menikmati pemandangan. 🌄✨
          </div>
          <div class="comment-list"></div>

          <form class="comment-form">
            <input type="text" placeholder="Tambahkan komentar..."
                   aria-label="Tulis komentar" maxlength="300">
            <button type="submit">Kirim</button>
          </form>
        </article>

        <!-- POST 3: FORMULA 1 -->
        <article class="post" data-id="f1">
          <div class="post-header">
            <img class="avatar" src="foto.jpg" alt="Foto profil"
                 onerror="this.onerror=null;this.src='https://placehold.co/100x100/111714/9dff65?text=R';">
            <div>
              <div class="post-user">kyy_cavalry</div>
              <div class="post-location">🏎️ Formula 1</div>
            </div>
          </div>

          <img class="post-image"
               src="f1.jpg"
               alt="Foto hobi menonton Formula 1"
               onerror="this.onerror=null;this.src='https://placehold.co/600x700/111714/9dff65?text=FOTO+FORMULA+1';">

          <div class="post-actions">
            <button class="action-btn like-btn" aria-label="Like postingan">
              <svg viewBox="0 0 24 24">
                <path d="M20.8 4.6a5.5 5.5 0 0 0-7.8 0L12 5.7l-1.1-1.1a5.5 5.5 0 0 0-7.8 7.8l1.1 1.1L12 21l7.8-7.5 1.1-1.1a5.5 5.5 0 0 0-.1-7.8Z"/>
              </svg>
            </button>

            <button class="action-btn comment-focus" aria-label="Komentar">
              <svg viewBox="0 0 24 24">
                <path d="M21 11.5a8.4 8.4 0 0 1-.9 3.8 8.5 8.5 0 0 1-7.6 4.7 8.4 8.4 0 0 1-3.8-.9L3 21l1.9-5.7a8.4 8.4 0 0 1-.9-3.8 8.5 8.5 0 0 1 4.7-7.6 8.4 8.4 0 0 1 3.8-.9h.5a8.5 8.5 0 0 1 8 8v.5Z"/>
              </svg>
            </button>

            <button class="action-btn share-btn" aria-label="Bagikan postingan">
              <svg viewBox="0 0 24 24">
                <path d="m22 2-7 20-4-9-9-4Z"/>
                <path d="M22 2 11 13"/>
              </svg>
            </button>
          </div>

          <div class="post-likes">0 suka</div>
          <div class="post-caption">
            <strong>kyy_cavalry</strong>
            Kecepatan, strategi, dan persaingan seru di Formula 1! 🏁🔥
          </div>
          <div class="comment-list"></div>

          <form class="comment-form">
            <input type="text" placeholder="Tambahkan komentar..."
                   aria-label="Tulis komentar" maxlength="300">
            <button type="submit">Kirim</button>
          </form>
        </article>

      </div>
    </div>
  </section>

  <!-- KONTAK -->
  <section class="section" id="kontak">
    <div class="container">
      <div class="contact-card">
        <h2 class="section-title">Hubungi <span>Saya</span></h2>
        <p>
          Ingin menyapa atau mengobrol? Silakan hubungi saya
          melalui WhatsApp atau kunjungi Instagram saya.
        </p>

        <div class="contact-buttons">
          <a class="btn btn-primary"
             href="https://wa.me/6283897256809"
             target="_blank" rel="noopener noreferrer">

            <span class="social-icon" aria-hidden="true">
              <svg viewBox="0 0 24 24">
                <path d="M20.5 3.5A11.8 11.8 0 0 0 12.1 0C5.6 0 .3 5.3.3 11.8c0 2.1.6 4.2 1.6 6L0 24l6.4-1.7a12 12 0 0 0 5.7 1.4h.1c6.5 0 11.8-5.3 11.8-11.8 0-3.2-1.2-6.2-3.5-8.4ZM12.1 21.7c-1.8 0-3.5-.5-5-1.4l-.4-.2-3.8 1 1-3.7-.3-.4a9.8 9.8 0 1 1 8.5 4.7Zm5.4-7.3c-.3-.2-1.8-.9-2.1-1-.3-.1-.5-.2-.7.2-.2.3-.8 1-1 1.2-.2.2-.4.2-.7.1-.3-.2-1.3-.5-2.5-1.5-.9-.8-1.5-1.8-1.7-2.1-.2-.3 0-.5.1-.7l.5-.6c.2-.2.2-.3.3-.6.1-.2 0-.4 0-.6-.1-.2-.7-1.7-.9-2.3-.3-.6-.5-.5-.7-.5h-.6c-.2 0-.6.1-.9.4-.3.3-1.2 1.2-1.2 2.8s1.2 3.2 1.4 3.4c.2.2 2.4 3.7 5.8 5.1.8.4 1.5.6 2 .7.8.3 1.6.2 2.2.1.7-.1 1.8-.7 2-1.4.3-.7.3-1.3.2-1.4-.1-.2-.3-.3-.6-.4Z"/>
              </svg>
            </span>
            WhatsApp
          </a>

          <a class="btn btn-secondary"
             href="https://instagram.com/kyy_cavalry"
             target="_blank" rel="noopener noreferrer">

            <span class="social-icon" aria-hidden="true">
              <svg viewBox="0 0 24 24">
                <path d="M7 2h10a5 5 0 0 1 5 5v10a5 5 0 0 1-5 5H7a5 5 0 0 1-5-5V7a5 5 0 0 1 5-5Zm0 2.2A2.8 2.8 0 0 0 4.2 7v10A2.8 2.8 0 0 0 7 19.8h10a2.8 2.8 0 0 0 2.8-2.8V7A2.8 2.8 0 0 0 17 4.2H7ZM12 7a5 5 0 1 1 0 10 5 5 0 0 1 0-10Zm0 2.2a2.8 2.8 0 1 0 0 5.6 2.8 2.8 0 0 0 0-5.6ZM17.5 5.5a1.2 1.2 0 1 1 0 2.4 1.2 1.2 0 0 1 0-2.4Z"/>
              </svg>
            </span>
            Instagram
          </a>
        </div>
      </div>
    </div>
  </section>
</main>

<footer>
  <div class="container">
    © 2026 <span>REZKY ADITYA</span> · Dibuat dengan semangat.
  </div>
</footer>

<script>
const USERNAME = "kyy_cavalry";
const STORAGE_KEY = "rezky_aditya_instagram_posts_v1";

function loadPosts() {
  try {
    return JSON.parse(localStorage.getItem(STORAGE_KEY)) || {};
  } catch (error) {
    return {};
  }
}

function savePosts(data) {
  try {
    localStorage.setItem(STORAGE_KEY, JSON.stringify(data));
  } catch (error) {
    console.log("Penyimpanan browser tidak tersedia.");
  }
}

let postsData = loadPosts();

function getPostData(id) {
  if (!postsData[id]) {
    postsData[id] = {
      liked: false,
      likes: 0,
      comments: []
    };
  }

  if (!Array.isArray(postsData[id].comments)) {
    postsData[id].comments = [];
  }

  return postsData[id];
}

function renderPost(post) {
  const id = post.dataset.id;
  const data = getPostData(id);

  const likeButton = post.querySelector(".like-btn");
  const likesText = post.querySelector(".post-likes");
  const commentList = post.querySelector(".comment-list");

  likeButton.classList.toggle("liked", data.liked);
  likeButton.setAttribute("aria-pressed", String(data.liked));
  likesText.textContent = data.likes + (data.likes === 1 ? " suka" : " suka");

  commentList.replaceChildren();

  data.comments.forEach(function(comment) {
    const line = document.createElement("div");
    line.className = "comment";

    const author = document.createElement("strong");
    author.textContent = comment.author;

    const message = document.createElement("span");
    message.textContent = comment.text;

    line.append(author, message);
    commentList.appendChild(line);
  });
}

document.querySelectorAll(".post").forEach(function(post) {
  const id = post.dataset.id;
  const data = getPostData(id);

  renderPost(post);

  post.querySelector(".like-btn").addEventListener("click", function() {
    const current = getPostData(id);

    if (current.liked) {
      current.liked = false;
      current.likes = Math.max(0, current.likes - 1);
    } else {
      current.liked = true;
      current.likes += 1;
    }

    savePosts(postsData);
    renderPost(post);
  });

  post.querySelector(".post-image").addEventListener("dblclick", function() {
    const current = getPostData(id);

    if (!current.liked) {
      current.liked = true;
      current.likes += 1;
      savePosts(postsData);
      renderPost(post);
    }
  });

  post.querySelector(".comment-focus").addEventListener("click", function() {
    post.querySelector(".comment-form input").focus();
  });

  post.querySelector(".comment-form").addEventListener("submit", function(event) {
    event.preventDefault();

    const input = this.querySelector("input");
    const message = input.value.trim();

    if (!message) {
      input.focus();
      return;
    }

    const current = getPostData(id);
    current.comments.push({
      author: USERNAME,
      text: message
    });

    savePosts(postsData);
    renderPost(post);
    input.value = "";
  });

  post.querySelector(".share-btn").addEventListener("click", async function() {
    const shareText = "Lihat hobi " + USERNAME + " di website REZKY ADITYA!";
    const shareUrl = window.location.href.split("#")[0];

    try {
      if (navigator.share) {
        await navigator.share({
          title: "REZKY ADITYA",
          text: shareText,
          url: shareUrl
        });
      } else if (navigator.clipboard && window.isSecureContext) {
        await navigator.clipboard.writeText(shareText + "\n" + shareUrl);
        alert("Teks dan tautan website berhasil disalin!");
      } else {
        window.prompt("Salin teks dan tautan ini:", shareText + "\n" + shareUrl);
      }
    } catch (error) {
      if (error.name !== "AbortError") {
        alert("Fitur berbagi tidak tersedia. Coba salin tautan website secara manual.");
      }
    }
  });
});
</script>

</body>
</html>
