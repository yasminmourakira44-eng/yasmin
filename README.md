<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Jang Wonyoung — Fã Site</title>
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href=https://rare-gallery.com/mocahbig/5433145-wonyoung-jang-won-young-ive-i-am-kpop.jpg rel="stylesheet">
  <style>
    :root{
      --bg:#0f1115;--bg-soft:#151923;--card:#1b2130;--text:#e9eef6;--muted:#b7c2d0;--acc:#7c9cf3;
      --shadow:0 10px 25px rgba(0,0,0,.25);
    }
    .light{--bg:#f7f9fc;--bg-soft:#ffffff;--card:#ffffff;--text:#0f1115;--muted:#4a5568;--acc:#3b82f6}
    *{box-sizing:border-box}
    html{scroll-behavior:smooth}
    body{margin:0;background:var(--bg);color:var(--text);font-family:Poppins,system-ui,-apple-system,Segoe UI,Roboto,Arial,sans-serif;line-height:1.6}
    a{color:var(--acc);text-decoration:none}
    img{max-width:100%;display:block}

    /* NAV */
    header{position:sticky;top:0;z-index:50;background:linear-gradient(0deg,rgba(0,0,0,.0),rgba(0,0,0,.25)) var(--bg-soft)}
    nav{max-width:1100px;margin:0 auto;display:flex;align-items:center;justify-content:space-between;padding:14px 20px}
    .brand{font-weight:700;letter-spacing:.5px}
    .brand span{color:var(--acc)}
    .nav-links{display:flex;gap:18px;align-items:center}
    .nav-links a{padding:8px 10px;border-radius:10px}
    .nav-links a:hover{background:rgba(124,156,243,.12)}
    #theme{border:0;background:transparent;color:var(--text);font-size:20px;cursor:pointer}

    /* HERO */
    .hero{position:relative;display:grid;place-items:center;min-height:75vh;padding:100px 20px 60px;background:
        radial-gradient(1200px 500px at 80% 0%, rgba(124,156,243,.18), transparent 60%),
        radial-gradient(900px 400px at 0% 20%, rgba(124,156,243,.12), transparent 55%)}
    .hero-inner{max-width:1100px;display:grid;grid-template-columns:1.1fr .9fr;gap:28px;align-items:center}
    .tag{display:inline-block;background:rgba(124,156,243,.15);color:var(--acc);border:1px solid rgba(124,156,243,.35);padding:6px 10px;border-radius:999px;font-size:12px;margin-bottom:10px}
    .title{font-size:clamp(28px,5vw,46px);line-height:1.15;margin:6px 0 10px}
    .subtitle{color:var(--muted);max-width:48ch}
    .cta{display:flex;gap:12px;margin-top:18px}
    .btn{padding:10px 16px;border-radius:12px;font-weight:600;border:1px solid transparent;cursor:pointer;transition:.2s}
    .btn.primary{background:var(--acc);color:white}
    .btn.primary:hover{filter:brightness(1.05)}
    .btn.ghost{background:transparent;border-color:rgba(124,156,243,.35);color:var(--acc)}
    .hero-card{background:var(--card);border:1px solid rgba(255,255,255,.06);border-radius:18px;box-shadow:var(--shadow);overflow:hidden}
    .hero-card img{aspect-ratio:4/5;object-fit:cover}

    /* SECTIONS */
    section{padding:64px 20px}
    .container{max-width:1100px;margin:0 auto}
    .section-title{font-size:clamp(24px,3.5vw,34px);margin:0 0 8px}
    .section-sub{color:var(--muted);margin:0 0 28px}

    /* SOBRE */
    .about{display:grid;grid-template-columns:1fr 1fr;gap:24px}
    .about p{margin:0}
    .stat-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:14px;margin-top:18px}
    .stat{background:var(--card);border:1px solid rgba(255,255,255,.06);padding:14px;border-radius:14px;text-align:center}
    .stat strong{display:block;font-size:20px}

    /* DESTAQUES */
    .grid{display:grid;grid-template-columns:repeat(3,1fr);gap:18px}
    .card{background:var(--card);border:1px solid rgba(255,255,255,.06);border-radius:16px;overflow:hidden;transition:transform .35s ease, box-shadow .35s ease;will-change:transform}
    .card:hover{transform:translateY(-6px) rotateZ(-.25deg);box-shadow:0 16px 40px rgba(0,0,0,.25)}
    .card img{aspect-ratio:16/9;object-fit:cover}
    .card .content{padding:14px}
    .pill{display:inline-block;background:rgba(124,156,243,.15);color:var(--acc);padding:4px 8px;border-radius:999px;font-size:12px;border:1px solid rgba(124,156,243,.35)}

    /* TIMELINE */
    .timeline{position:relative;margin-top:10px}
    .timeline:before{content:"";position:absolute;left:11px;top:0;bottom:0;width:2px;background:rgba(124,156,243,.35)}
    .tl-item{position:relative;padding-left:34px;margin:16px 0}
    .tl-item:before{content:"";position:absolute;left:5px;top:6px;width:14px;height:14px;border-radius:50%;background:var(--acc);box-shadow:0 0 0 4px rgba(124,156,243,.2)}
    .tl-item h4{margin:0}
    .tl-item p{margin:6px 0 0;color:var(--muted)}

    /* GALERIA */
    .gallery{display:grid;grid-template-columns:repeat(4,1fr);gap:10px}
    .gallery img{border-radius:12px;aspect-ratio:3/4;object-fit:cover;border:1px solid rgba(255,255,255,.08)}

    /* FOOTER */
    footer{padding:40px 20px;border-top:1px solid rgba(255,255,255,.06);background:var(--bg-soft);color:var(--muted)}
    .footer-inner{max-width:1100px;margin:0 auto;display:flex;justify-content:space-between;align-items:center;gap:16px}

    /* UTIL */
    .muted{color:var(--muted)}
    .hide{display:none}

    /* RESPONSIVO */
    @media (max-width: 980px){
      .hero-inner{grid-template-columns:1fr}
      .about{grid-template-columns:1fr}
      .grid{grid-template-columns:1fr 1fr}
      .gallery{grid-template-columns:1fr 1fr 1fr}
    }
    @media (max-width: 640px){
      nav{padding:12px 16px}
      .nav-links{gap:10px}
      .grid{grid-template-columns:1fr}
      .gallery{grid-template-columns:1fr 1fr}
    }
  </style>
</head>
<body>
  <header>
    <nav>
      <div class="brand">Wonyoung<span>.fan</span></div>
      <div class="nav-links">
        <a href="#sobre">Sobre</a>
        <a href="#destaques">Destaques</a>
        <a href="#timeline">Linha do tempo</a>
        <a href="#galeria">Galeria</a>
        <a href="#links">Links</a>
        <button id="theme" aria-label="Alternar tema" title="Alternar tema">🌙</button>
      </div>
    </nav>
  </header>

  <section class="hero">
    <div class="hero-inner">
      <div>
        <span class="tag">Fã Site • K‑pop</span>
        <h1 class="title">Jang Wonyoung</h1>
        <p class="subtitle">Cantora, modelo e apresentadora sul‑coreana. Conhecida por sua presença de palco elegante, carisma e visuais icônicos. Esta é uma página de fã, feita para celebrar sua trajetória e conquistas.</p>
        <div class="cta">
          <a class="btn primary" href="#destaques">Ver destaques</a>
          <a class="btn ghost" href="#links">Links oficiais</a>
        </div>
      </div>
      <div class="hero-card">
        <!-- Substitua o src por uma foto sua/permitida -->
        <img src=https://www.fativa.id/wp-content/uploads/2024/03/3-4.jpg" alt=https://www.fativa.id/wp-content/uploads/2024/03/3-4.jpg />
      </div>
    </div>
  </section>

  <section id="sobre">
    <div class="container about">
      <div>
        <h2 class="section-title">Sobre</h2>
        <p>Jang Wonyoung (장원영) é uma artista da 4ª geração do K‑pop, admirada por sua versatilidade: além de cantora, atua como modelo de campanhas globais e apresentadora de programas musicais. Seu estilo combina elegância, frescor e performance confiante.</p>
        <p class="muted" style="margin-top:10px">Nota: este site é um projeto de fã, sem afiliação oficial. Informações podem ser resumidas para fins de demonstração.</p>
      </div>
      <div>
        <h3 style="margin:0 0 6px">Curiosidades rápidas</h3>
        <div class="stat-grid">
          <div class="stat"><strong>Altura</strong><span class="muted">≈ 1,73 m</span></div>
          <div class="stat"><strong>Posições</strong><span class="muted">Vocal • Visual</span></div>
          <div class="stat"><strong>Estilo</strong><span class="muted">Elegante & fresh</span></div>
        </div>
      </div>
    </div>
  </section>

  <section id="destaques">
    <div class="container">
      <h2 class="section-title">Destaques</h2>
      <p class="section-sub">Momentos e trabalhos que marcaram a carreira.</p>
      <div class="grid">
        <article class="card">
          <img src="https://www.fativa.id/wp-content/uploads/2024/03/3-4.jpg alt="Microfone no palco" />
          <div class="content">
            <span class="pill">Performance</span>
            <h3>Stages icônicos</h3>
            <p class="muted">Apresentações marcadas por vocais limpos, presença elegante e figurinos memoráveis.</p>
          </div>
        </article>
        <article class="card">
          <img src="https://tse2.mm.bing.net/th/id/OIP.Jox2WSWb8e0Wf9f9P-Bl9wHaJ3?rs=1&pid=ImgDetMain&o=7&rm=" alt="Close de editorial de moda" />
          <div class="content">
            <span class="pill">Moda</span>
            <h3>Campanhas & editoriais</h3>
            <p class="muted">Rosto de marcas de luxo e capas de revistas, definindo tendências na 4ª geração.</p>
          </div>
        </article>
        <article class="card">
          <img src="https://images.unsplash.com/photo-1511512578047-dfb367046420?q=80&w=1200&auto=format&fit=crop" alt="Apresentadora em estúdio" />
          <div class="content">
            <span class="pill">MC</span>
            <h3>Apresentações em TV</h3>
            <p class="muted">Carisma como MC em programas musicais, entrevistas e eventos especiais.</p>
          </div>
        </article>
      </div>
    </div>
  </section>

  <section id="timeline">
    <div class="container">
      <h2 class="section-title">Linha do tempo</h2>
      <div class="timeline">
        <div class="tl-item">
          <h4>Estreia e primeiros passos</h4>
          <p>Ganha destaque na cena de K‑pop e inicia atividades promocionais e de performance.</p>
        </div>
        <div class="tl-item">
          <h4>Reconhecimento em moda</h4>
          <p>Começa a assinar campanhas e editoriais, tornando-se referência de estilo.</p>
        </div>
        <div class="tl-item">
          <h4>MC e prêmios</h4>
          <p>Consolida imagem pública com aparições na TV, prêmios e grandes palcos.</p>
        </div>
      </div>
    </div>
  </section>

  <section id="galeria">
    <div class="container">
      <h2 class="section-title">Galeria</h2>
      <p class="section-sub">Substitua as imagens pelos seus favoritos (use fotos com permissão de uso).</p>
      <div class="gallery">
        <img src="https://images.unsplash.com/photo-1503342452485-86ff0a3b82dd?q=80&w=1200&auto=format&fit=crop" alt="Editorial 1" />
        <img src="https://images.unsplash.com/photo-1511660932688-5bab3b1eb498?q=80&w=1200&auto=format&fit=crop" alt="Editorial 2" />
        <img src="https://images.unsplash.com/photo-1489326920423-276a1d8a091b?q=80&w=1200&auto=format&fit=crop" alt="Editorial 3" />
        <img src="https://images.unsplash.com/photo-1503342394128-c104d54dba01?q=80&w=1200&auto=format&fit=crop" alt="Editorial 4" />
        <img src="https://images.unsplash.com/photo-1506377247377-2a5b3b417ebb?q=80&w=1200&auto=format&fit=crop" alt="Stage 1" />
        <img src="https://images.unsplash.com/photo-1489424731084-a5d8b219a5bb?q=80&w=1200&auto=format&fit=crop" alt="Stage 2" />
        <img src="https://images.unsplash.com/photo-1515165562835-c3b8c2e43358?q=80&w=1200&auto=format&fit=crop" alt="Fashion 1" />
        <img src="https://images.unsplash.com/photo-1520975600240-3a7c02aab7f2?q=80&w=1200&auto=format&fit=crop" alt="Fashion 2" />
      </div>
    </div>
  </section>

  <section id="links">
    <div class="container">
      <h2 class="section-title">Links & recursos</h2>
      <p class="section-sub">Acompanhe canais oficiais e comunidades de fãs.</p>
      <div class="grid">
        <article class="card">
          <div class="content">
            <span class="pill">Oficial</span>
            <h3>Agência / Grupo</h3>
            <p class="muted">Siga os perfis oficiais para notícias, teasers e anúncios.</p>
            <p><a href="#" target="_blank" rel="noopener">Website oficial</a></p>
          </div>
        </article>
        <article class="card">
          <div class="content">
            <span class="pill">Social</span>
            <h3>Perfis</h3>
            <p class="muted">Adicione links para Instagram, YouTube, TikTok e mais.</p>
            <p><a href="#" target="_blank" rel="noopener">Adicionar Instagram</a></p>
          </div>
        </article>
        <article class="card">
          <div class="content">
            <span class="pill">Fandom</span>
            <h3>Guia rápido</h3>
            <p class="muted">Lightstick, cores, slogans e projetos de fãs — personalize como quiser.</p>
            <p><a href="#" target="_blank" rel="noopener">Comunidade</a></p>
          </div>
        </article>
      </div>
    </div>
  </section>

  <footer>
    <div class="footer-inner">
      <small>Projeto de fã • Feito com ❤ • <span id="year"></span></small>
      <a href="#" class="muted" onclick="window.scrollTo({top:0,behavior:'smooth'})">Voltar ao topo ↑</a>
    </div>
  </footer>

  <script>
    // Tema claro/escuro com persistência
    const body = document.body;
    const stored = localStorage.getItem('theme');
    if(stored === 'light'){ body.classList.add('light'); }
    document.getElementById('theme').addEventListener('click',()=>{
      body.classList.toggle('light');
      localStorage.setItem('theme', body.classList.contains('light') ? 'light':'dark');
    });

    // Ano automático
    document.getElementById('year').textContent = new Date().getFullYear();
  </script>
</body>
</html>
