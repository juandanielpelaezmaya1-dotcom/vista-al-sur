<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="description" content="Vista al Sur Inmobiliaria — Propiedades premium en Pasto, Nariño. Asesoría personalizada para encontrar el inmueble que buscas.">
<title>Vista al Sur Inmobiliaria — Pasto, Nariño</title>
<style>
  :root {
    --verde: #105a41;
    --verde-claro: #c4ffa5;
    --gris: #d9d9d9;
    --blanco: #ffffff;
    --texto: #1a1a1a;
    --texto-suave: #555;
    --fondo: #f7f7f5;
    --font: 'Segoe UI', system-ui, -apple-system, sans-serif;
  }

  * { box-sizing: border-box; margin: 0; padding: 0; }
  html { scroll-behavior: smooth; }
  body { font-family: var(--font); color: var(--texto); background: var(--blanco); }

  /* ── NAV ── */
  nav {
    position: sticky; top: 0; z-index: 100;
    background: rgba(255,255,255,0.97);
    backdrop-filter: blur(8px);
    border-bottom: 1px solid var(--gris);
    padding: 0 2rem;
    display: flex; align-items: center; justify-content: space-between;
    height: 68px;
  }
  .nav-logo { display: flex; align-items: center; gap: .75rem; text-decoration: none; }
  .nav-logo svg { height: 38px; width: auto; }
  .nav-logo-text { display: flex; flex-direction: column; line-height: 1; }
  .nav-logo-text .brand { font-size: 17px; font-weight: 800; color: var(--verde); letter-spacing: .5px; }
  .nav-logo-text .sub { font-size: 10px; letter-spacing: 2px; color: var(--texto-suave); text-transform: uppercase; }
  .nav-links { display: flex; align-items: center; gap: 1.75rem; }
  .nav-links a { text-decoration: none; color: var(--texto-suave); font-size: 14px; font-weight: 500; transition: color .2s; }
  .nav-links a:hover { color: var(--verde); }
  .btn-nav {
    background: var(--verde); color: var(--blanco);
    padding: 9px 20px; border-radius: 8px;
    font-size: 14px; font-weight: 600; text-decoration: none;
    transition: background .2s, transform .1s;
    display: flex; align-items: center; gap: .4rem;
  }
  .btn-nav:hover { background: #0d4a35; transform: translateY(-1px); }
  .hamburger { display: none; flex-direction: column; gap: 5px; cursor: pointer; padding: 4px; }
  .hamburger span { display: block; width: 22px; height: 2px; background: var(--verde); border-radius: 2px; transition: all .3s; }

  /* ── HERO ── */
  .hero {
    background: linear-gradient(160deg, #0d3d2d 0%, #105a41 60%, #1a7a58 100%);
    color: var(--blanco);
    padding: 5rem 2rem 4rem;
    text-align: center;
    position: relative;
    overflow: hidden;
  }
  .hero::before {
    content: '';
    position: absolute; inset: 0;
    background: url("data:image/svg+xml,%3Csvg width='60' height='60' viewBox='0 0 60 60' xmlns='http://www.w3.org/2000/svg'%3E%3Cg fill='none' fill-rule='evenodd'%3E%3Cg fill='%23ffffff' fill-opacity='0.03'%3E%3Cpath d='M36 34v-4h-2v4h-4v2h4v4h2v-4h4v-2h-4zm0-30V0h-2v4h-4v2h4v4h2V6h4V4h-4zM6 34v-4H4v4H0v2h4v4h2v-4h4v-2H6zM6 4V0H4v4H0v2h4v4h2V6h4V4H6z'/%3E%3C/g%3E%3C/g%3E%3C/svg%3E");
    opacity: .4;
  }
  .hero-inner { position: relative; max-width: 720px; margin: 0 auto; }
  .hero-badge {
    display: inline-block;
    background: rgba(196,255,165,.15);
    border: 1px solid rgba(196,255,165,.4);
    color: var(--verde-claro);
    font-size: 12px; font-weight: 600; letter-spacing: 1.5px;
    text-transform: uppercase;
    padding: 5px 14px; border-radius: 20px;
    margin-bottom: 1.5rem;
  }
  .hero h1 {
    font-size: clamp(2rem, 5vw, 3rem);
    font-weight: 800; line-height: 1.15;
    margin-bottom: 1.25rem;
  }
  .hero h1 em { font-style: normal; color: var(--verde-claro); }
  .hero p {
    font-size: 1.1rem; color: rgba(255,255,255,.8);
    max-width: 520px; margin: 0 auto 2.5rem;
    line-height: 1.7;
  }
  .hero-ctas { display: flex; gap: 1rem; justify-content: center; flex-wrap: wrap; }
  .btn-primary {
    background: var(--verde-claro); color: var(--verde);
    font-weight: 700; font-size: 15px;
    padding: 14px 28px; border-radius: 10px;
    text-decoration: none; display: flex; align-items: center; gap: .5rem;
    transition: transform .15s, box-shadow .15s;
    box-shadow: 0 4px 20px rgba(196,255,165,.3);
  }
  .btn-primary:hover { transform: translateY(-2px); box-shadow: 0 6px 24px rgba(196,255,165,.45); }
  .btn-secondary {
    background: transparent; color: var(--blanco);
    font-weight: 600; font-size: 15px;
    padding: 14px 28px; border-radius: 10px;
    border: 1.5px solid rgba(255,255,255,.35);
    text-decoration: none; display: flex; align-items: center; gap: .5rem;
    transition: border-color .2s, background .2s;
  }
  .btn-secondary:hover { border-color: rgba(255,255,255,.7); background: rgba(255,255,255,.07); }
  .hero-stats {
    display: flex; justify-content: center; gap: 3rem;
    margin-top: 3.5rem; padding-top: 2.5rem;
    border-top: 1px solid rgba(255,255,255,.12);
    flex-wrap: wrap;
  }
  .stat-item { text-align: center; }
  .stat-num { font-size: 1.75rem; font-weight: 800; color: var(--verde-claro); display: block; }
  .stat-label { font-size: 12px; color: rgba(255,255,255,.6); text-transform: uppercase; letter-spacing: .8px; }

  /* ── SECCIONES ── */
  section { padding: 5rem 2rem; }
  .container { max-width: 1100px; margin: 0 auto; }
  .section-label { font-size: 12px; font-weight: 700; letter-spacing: 2px; text-transform: uppercase; color: var(--verde); margin-bottom: .5rem; }
  .section-title { font-size: clamp(1.6rem, 3vw, 2.1rem); font-weight: 800; margin-bottom: .75rem; line-height: 1.2; }
  .section-sub { color: var(--texto-suave); font-size: 1rem; max-width: 500px; line-height: 1.7; }

  /* ── POR QUÉ ── */
  .porqué { background: var(--fondo); }
  .porqué-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 2rem; align-items: center; margin-top: 3rem; }
  .porqué-items { display: flex; flex-direction: column; gap: 1.25rem; }
  .porqué-item {
    display: flex; gap: 1rem; align-items: flex-start;
    background: var(--blanco); border: 1px solid var(--gris);
    border-radius: 12px; padding: 1.25rem;
    transition: border-color .2s, box-shadow .2s;
  }
  .porqué-item:hover { border-color: var(--verde); box-shadow: 0 4px 16px rgba(16,90,65,.08); }
  .porqué-icon {
    width: 44px; height: 44px; border-radius: 10px;
    background: rgba(16,90,65,.08);
    display: flex; align-items: center; justify-content: center;
    flex-shrink: 0; font-size: 20px;
  }
  .porqué-item h3 { font-size: 15px; font-weight: 700; margin-bottom: .25rem; }
  .porqué-item p { font-size: 13px; color: var(--texto-suave); line-height: 1.6; }
  .porqué-visual {
    background: linear-gradient(135deg, #105a41, #1a7a58);
    border-radius: 16px; padding: 2.5rem;
    color: var(--blanco); text-align: center;
  }
  .porqué-visual .big-icon { font-size: 4rem; margin-bottom: 1rem; display: block; }
  .porqué-visual h3 { font-size: 1.3rem; font-weight: 700; margin-bottom: .5rem; }
  .porqué-visual p { font-size: 14px; opacity: .8; line-height: 1.6; }
  .porqué-visual .highlight { color: var(--verde-claro); font-weight: 700; }

  /* ── PORTAFOLIO ── */
  .portafolio-header { display: flex; align-items: flex-end; justify-content: space-between; gap: 1rem; margin-bottom: 2.5rem; flex-wrap: wrap; }
  .propiedades-grid { display: grid; grid-template-columns: repeat(3, 1fr); gap: 1.5rem; }
  .propiedad-card {
    border-radius: 14px; overflow: hidden;
    border: 1px solid var(--gris);
    background: var(--blanco);
    transition: transform .2s, box-shadow .2s;
  }
  .propiedad-card:hover { transform: translateY(-4px); box-shadow: 0 12px 32px rgba(0,0,0,.1); }
  .propiedad-img {
    height: 200px;
    background: linear-gradient(135deg, var(--gris) 0%, #c0c0c0 100%);
    position: relative;
    display: flex; align-items: center; justify-content: center;
    overflow: hidden;
  }
  .propiedad-img img { width: 100%; height: 100%; object-fit: cover; }
  .propiedad-img .placeholder-img {
    display: flex; flex-direction: column; align-items: center; gap: .5rem;
    color: #888; font-size: 13px; text-align: center; padding: 1rem;
  }
  .propiedad-img .placeholder-img span { font-size: 2.5rem; }
  .badge-tipo {
    position: absolute; top: 12px; left: 12px;
    background: var(--verde); color: var(--blanco);
    font-size: 11px; font-weight: 700; letter-spacing: .5px;
    padding: 3px 10px; border-radius: 6px;
    text-transform: uppercase;
  }
  .badge-destacado {
    position: absolute; top: 12px; right: 12px;
    background: var(--verde-claro); color: var(--verde);
    font-size: 11px; font-weight: 700;
    padding: 3px 10px; border-radius: 6px;
  }
  .propiedad-body { padding: 1.25rem; }
  .propiedad-zona { font-size: 11px; color: var(--texto-suave); text-transform: uppercase; letter-spacing: .8px; margin-bottom: .25rem; }
  .propiedad-nombre { font-size: 16px; font-weight: 700; margin-bottom: .75rem; }
  .propiedad-specs { display: flex; gap: 1rem; margin-bottom: 1rem; flex-wrap: wrap; }
  .spec { font-size: 12px; color: var(--texto-suave); display: flex; align-items: center; gap: .3rem; }
  .propiedad-precio { font-size: 1.2rem; font-weight: 800; color: var(--verde); }
  .propiedad-precio small { font-size: 12px; font-weight: 400; color: var(--texto-suave); }
  .propiedad-footer { display: flex; align-items: center; justify-content: space-between; margin-top: 1rem; padding-top: 1rem; border-top: 1px solid var(--gris); }
  .btn-ver {
    background: var(--verde); color: var(--blanco);
    font-size: 13px; font-weight: 600;
    padding: 8px 16px; border-radius: 8px;
    text-decoration: none; transition: background .2s;
  }
  .btn-ver:hover { background: #0d4a35; }
  .ver-mas-wrap { text-align: center; margin-top: 2.5rem; }
  .btn-outline {
    display: inline-flex; align-items: center; gap: .5rem;
    border: 2px solid var(--verde); color: var(--verde);
    font-weight: 700; font-size: 14px;
    padding: 12px 28px; border-radius: 10px;
    text-decoration: none; transition: all .2s;
  }
  .btn-outline:hover { background: var(--verde); color: var(--blanco); }

  /* ── PROCESO ── */
  .proceso { background: var(--fondo); }
  .proceso-grid { display: grid; grid-template-columns: repeat(4, 1fr); gap: 1.5rem; margin-top: 3rem; }
  .proceso-step { text-align: center; padding: 1.5rem 1rem; }
  .proceso-num {
    width: 48px; height: 48px; border-radius: 50%;
    background: var(--verde); color: var(--blanco);
    font-size: 18px; font-weight: 800;
    display: flex; align-items: center; justify-content: center;
    margin: 0 auto 1rem;
  }
  .proceso-step h3 { font-size: 15px; font-weight: 700; margin-bottom: .5rem; }
  .proceso-step p { font-size: 13px; color: var(--texto-suave); line-height: 1.6; }

  /* ── CONTACTO ── */
  .contacto { background: var(--verde); color: var(--blanco); text-align: center; }
  .contacto .section-label { color: var(--verde-claro); }
  .contacto .section-title { color: var(--blanco); }
  .contacto .section-sub { color: rgba(255,255,255,.75); margin: 0 auto 2.5rem; }
  .contacto-form {
    background: var(--blanco); border-radius: 16px;
    padding: 2.5rem; max-width: 580px; margin: 0 auto;
    text-align: left;
  }
  .form-row { display: grid; grid-template-columns: 1fr 1fr; gap: 1rem; }
  .form-group { margin-bottom: 1.25rem; }
  .form-group label { display: block; font-size: 13px; font-weight: 600; color: var(--texto); margin-bottom: .4rem; }
  .form-group input,
  .form-group select,
  .form-group textarea {
    width: 100%; padding: 11px 14px;
    border: 1.5px solid var(--gris);
    border-radius: 8px; font-size: 14px;
    font-family: var(--font);
    color: var(--texto);
    transition: border-color .2s;
    outline: none;
  }
  .form-group input:focus,
  .form-group select:focus,
  .form-group textarea:focus { border-color: var(--verde); }
  .form-group textarea { height: 100px; resize: vertical; }
  .btn-submit {
    width: 100%; background: var(--verde); color: var(--blanco);
    font-size: 15px; font-weight: 700; padding: 14px;
    border: none; border-radius: 10px; cursor: pointer;
    display: flex; align-items: center; justify-content: center; gap: .5rem;
    transition: background .2s, transform .1s;
  }
  .btn-submit:hover { background: #0d4a35; transform: translateY(-1px); }
  .form-note { font-size: 12px; color: var(--texto-suave); text-align: center; margin-top: 1rem; }

  /* ── WHATSAPP FLOTANTE ── */
  .whatsapp-float {
    position: fixed; bottom: 24px; right: 24px; z-index: 999;
    width: 58px; height: 58px; border-radius: 50%;
    background: #25d366;
    display: flex; align-items: center; justify-content: center;
    box-shadow: 0 4px 20px rgba(37,211,102,.4);
    text-decoration: none;
    animation: pulse-wa 2.5s infinite;
    transition: transform .2s;
  }
  .whatsapp-float:hover { transform: scale(1.1); }
  .whatsapp-float svg { width: 30px; height: 30px; fill: white; }
  @keyframes pulse-wa {
    0%, 100% { box-shadow: 0 4px 20px rgba(37,211,102,.4); }
    50% { box-shadow: 0 4px 32px rgba(37,211,102,.7); }
  }

  /* ── FOOTER ── */
  footer {
    background: #0a2a1e; color: rgba(255,255,255,.6);
    padding: 3rem 2rem 2rem;
  }
  .footer-inner { max-width: 1100px; margin: 0 auto; }
  .footer-top { display: grid; grid-template-columns: 1.5fr 1fr 1fr; gap: 3rem; margin-bottom: 2.5rem; }
  .footer-brand .brand-name { font-size: 18px; font-weight: 800; color: var(--blanco); margin-bottom: .25rem; }
  .footer-brand .brand-sub { font-size: 11px; letter-spacing: 2px; text-transform: uppercase; color: var(--verde-claro); margin-bottom: .75rem; }
  .footer-brand p { font-size: 13px; line-height: 1.7; }
  .footer-col h4 { font-size: 13px; font-weight: 700; color: var(--blanco); margin-bottom: 1rem; text-transform: uppercase; letter-spacing: .5px; }
  .footer-col a { display: block; font-size: 13px; color: rgba(255,255,255,.55); text-decoration: none; margin-bottom: .5rem; transition: color .2s; }
  .footer-col a:hover { color: var(--verde-claro); }
  .footer-bottom { border-top: 1px solid rgba(255,255,255,.08); padding-top: 1.5rem; display: flex; justify-content: space-between; align-items: center; flex-wrap: gap; font-size: 12px; }
  .footer-social { display: flex; gap: 1rem; }
  .footer-social a { color: rgba(255,255,255,.5); text-decoration: none; font-size: 13px; transition: color .2s; }
  .footer-social a:hover { color: var(--verde-claro); }

  /* ── RESPONSIVE ── */
  @media (max-width: 900px) {
    .propiedades-grid { grid-template-columns: repeat(2, 1fr); }
    .proceso-grid { grid-template-columns: repeat(2, 1fr); }
    .porqué-grid { grid-template-columns: 1fr; }
    .footer-top { grid-template-columns: 1fr 1fr; }
  }
  @media (max-width: 640px) {
    .propiedades-grid { grid-template-columns: 1fr; }
    .proceso-grid { grid-template-columns: 1fr 1fr; }
    .form-row { grid-template-columns: 1fr; }
    .footer-top { grid-template-columns: 1fr; }
    .nav-links { display: none; }
    .hamburger { display: flex; }
    .hero { padding: 3.5rem 1.5rem 3rem; }
    .hero-stats { gap: 1.5rem; }
    section { padding: 3.5rem 1.25rem; }
  }
</style>
</head>
<body>

<!-- WHATSAPP FLOTANTE -->
<a class="whatsapp-float" href="https://wa.me/573218604753?text=Hola%2C%20me%20interesa%20conocer%20sus%20propiedades%20disponibles" target="_blank" rel="noopener" aria-label="Escribir por WhatsApp">
  <svg viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
    <path d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347z"/>
    <path d="M12 0C5.373 0 0 5.373 0 12c0 2.124.558 4.118 1.532 5.845L.057 23.492a.5.5 0 0 0 .614.644l5.939-1.56A11.945 11.945 0 0 0 12 24c6.627 0 12-5.373 12-12S18.627 0 12 0zm0 21.818a9.806 9.806 0 0 1-5.034-1.389l-.36-.214-3.733.98.998-3.648-.235-.374A9.808 9.808 0 0 1 2.182 12C2.182 6.57 6.57 2.182 12 2.182c5.43 0 9.818 4.388 9.818 9.818 0 5.43-4.388 9.818-9.818 9.818z"/>
  </svg>
</a>

<!-- NAV -->
<nav>
  <a href="#" class="nav-logo">
    <!-- Logo SVG recreado con la paleta de marca -->
    <svg viewBox="0 0 120 60" xmlns="http://www.w3.org/2000/svg" aria-label="Vista al Sur Inmobiliaria">
      <!-- Sol -->
      <circle cx="60" cy="18" r="7" fill="#105a41"/>
      <!-- Rayos del sol -->
      <g stroke="#105a41" stroke-width="2" stroke-linecap="round">
        <line x1="60" y1="7" x2="60" y2="4"/>
        <line x1="69" y1="10" x2="71" y2="8"/>
        <line x1="72" y1="18" x2="75" y2="18"/>
        <line x1="51" y1="10" x2="49" y2="8"/>
        <line x1="48" y1="18" x2="45" y2="18"/>
        <line x1="69" y1="26" x2="71" y2="28"/>
        <line x1="51" y1="26" x2="49" y2="28"/>
      </g>
      <!-- Montaña derecha -->
      <polygon points="50,44 72,44 61,22" fill="#105a41"/>
      <!-- Montaña izquierda -->
      <polygon points="30,44 58,44 44,26" fill="#105a41" opacity=".7"/>
      <!-- Montaña extrema izquierda -->
      <polygon points="14,44 46,44 30,30" fill="#105a41" opacity=".5"/>
    </svg>
    <div class="nav-logo-text">
      <span class="brand">VISTA AL SUR</span>
      <span class="sub">Inmobiliaria</span>
    </div>
  </a>

  <div class="nav-links">
    <a href="#portafolio">Portafolio</a>
    <a href="#proceso">Cómo trabajamos</a>
    <a href="#contacto">Contacto</a>
    <a class="btn-nav" href="https://wa.me/573218604753?text=Hola%2C%20quiero%20asesor%C3%ADa%20inmobiliaria" target="_blank" rel="noopener">
      <svg width="16" height="16" viewBox="0 0 24 24" fill="currentColor"><path d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347z"/><path d="M12 0C5.373 0 0 5.373 0 12c0 2.124.558 4.118 1.532 5.845L.057 23.492a.5.5 0 0 0 .614.644l5.939-1.56A11.945 11.945 0 0 0 12 24c6.627 0 12-5.373 12-12S18.627 0 12 0zm0 21.818a9.806 9.806 0 0 1-5.034-1.389l-.36-.214-3.733.98.998-3.648-.235-.374A9.808 9.808 0 0 1 2.182 12C2.182 6.57 6.57 2.182 12 2.182c5.43 0 9.818 4.388 9.818 9.818 0 5.43-4.388 9.818-9.818 9.818z"/></svg>
      Escribir ahora
    </a>
  </div>
  <div class="hamburger" onclick="toggleMenu(this)">
    <span></span><span></span><span></span>
  </div>
</nav>

<!-- HERO -->
<section class="hero">
  <div class="hero-inner">
    <span class="hero-badge">Pasto, Nariño · Colombia</span>
    <h1>Encuentra la propiedad<br>que <em>realmente</em> buscas</h1>
    <p>Asesoría personalizada, propiedades de calidad en las mejores zonas de Pasto. Te acompañamos en cada paso hasta cerrar el negocio.</p>
    <div class="hero-ctas">
      <a class="btn-primary" href="#portafolio">
        Ver propiedades disponibles
      </a>
      <a class="btn-secondary" href="https://wa.me/573218604753?text=Hola%2C%20me%20interesa%20una%20asesor%C3%ADa" target="_blank" rel="noopener">
        <svg width="16" height="16" viewBox="0 0 24 24" fill="currentColor"><path d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347z"/><path d="M12 0C5.373 0 0 5.373 0 12c0 2.124.558 4.118 1.532 5.845L.057 23.492a.5.5 0 0 0 .614.644l5.939-1.56A11.945 11.945 0 0 0 12 24c6.627 0 12-5.373 12-12S18.627 0 12 0zm0 21.818a9.806 9.806 0 0 1-5.034-1.389l-.36-.214-3.733.98.998-1.648-.235-.374A9.808 9.808 0 0 1 2.182 12C2.182 6.57 6.57 2.182 12 2.182c5.43 0 9.818 4.388 9.818 9.818 0 5.43-4.388 9.818-9.818 9.818z"/></svg>
        Hablar con un asesor
      </a>
    </div>
    <div class="hero-stats">
      <div class="stat-item">
        <span class="stat-num">100%</span>
        <span class="stat-label">Asesoría personalizada</span>
      </div>
      <div class="stat-item">
        <span class="stat-num">Nariño</span>
        <span class="stat-label">Especialistas locales</span>
      </div>
      <div class="stat-item">
        <span class="stat-num">Premium</span>
        <span class="stat-label">Solo propiedades de calidad</span>
      </div>
    </div>
  </div>
</section>

<!-- POR QUÉ NOSOTROS -->
<section class="porqué">
  <div class="container">
    <p class="section-label">Por qué elegirnos</p>
    <h2 class="section-title">No vendemos cualquier propiedad.<br>Solo las que valen la pena.</h2>

    <div class="porqué-grid">
      <div class="porqué-items">
        <div class="porqué-item">
          <div class="porqué-icon">🏆</div>
          <div>
            <h3>Solo propiedades seleccionadas</h3>
            <p>Trabajamos únicamente con inmuebles de calidad y bien ubicados en Pasto. Si no cumple el estándar, no lo ofrecemos.</p>
          </div>
        </div>
        <div class="porqué-item">
          <div class="porqué-icon">⚡</div>
          <div>
            <h3>Respuesta en minutos</h3>
            <p>Te atendemos rápido, siempre. Sin esperas ni formularios interminables. Un mensaje de WhatsApp es suficiente.</p>
          </div>
        </div>
        <div class="porqué-item">
          <div class="porqué-icon">🤝</div>
          <div>
            <h3>Asesoría de principio a fin</h3>
            <p>Desde que nos contactas hasta que firmas. Te guiamos en cada paso del proceso, sin letra pequeña.</p>
          </div>
        </div>
        <div class="porqué-item">
          <div class="porqué-icon">📍</div>
          <div>
            <h3>Conocemos Pasto</h3>
            <p>Somos locales. Sabemos qué zonas crecen, qué barrios convienen y dónde está el verdadero valor.</p>
          </div>
        </div>
      </div>

      <div class="porqué-visual">
        <span class="big-icon">🏔️</span>
        <h3>Tu propiedad ideal<br>existe en Pasto</h3>
        <p>Déjanos encontrarla. Cuéntanos qué buscas y en <span class="highlight">menos de 24 horas</span> te mostramos opciones que realmente se ajustan a lo que necesitas.</p>
        <br>
        <a class="btn-primary" href="https://wa.me/573218604753?text=Hola%2C%20busco%20una%20propiedad%20en%20Pasto" target="_blank" rel="noopener" style="justify-content:center; margin-top:.5rem;">
          Cuéntanos qué buscas
        </a>
      </div>
    </div>
  </div>
</section>

<!-- PORTAFOLIO -->
<section id="portafolio">
  <div class="container">
    <div class="portafolio-header">
      <div>
        <p class="section-label">Portafolio</p>
        <h2 class="section-title">Propiedades disponibles</h2>
        <p class="section-sub">Inmuebles verificados, bien ubicados y listos para cerrar negocio.</p>
      </div>
      <a class="btn-outline" href="https://wa.me/573218604753?text=Hola%2C%20quiero%20ver%20todas%20las%20propiedades%20disponibles" target="_blank" rel="noopener">
        Ver portafolio completo →
      </a>
    </div>

    <div class="propiedades-grid">

      <!-- PROPIEDAD 1 — REEMPLAZAR -->
      <div class="propiedad-card">
        <div class="propiedad-img">
          <!-- Reemplaza esta sección con: <img src="foto-propiedad-1.jpg" alt="Nombre propiedad"> -->
          <div class="placeholder-img">
            <span>🏠</span>
            <p>Agregar foto de la propiedad</p>
          </div>
          <span class="badge-tipo">Casa</span>
          <span class="badge-destacado">Destacada</span>
        </div>
        <div class="propiedad-body">
          <p class="propiedad-zona">📍 Zona Norte · Pasto</p>
          <h3 class="propiedad-nombre">Casa Sector Niza — 3 habitaciones</h3>
          <div class="propiedad-specs">
            <span class="spec">🛏 3 hab.</span>
            <span class="spec">🚿 2 baños</span>
            <span class="spec">📐 120 m²</span>
            <span class="spec">🚗 Garaje</span>
          </div>
          <p class="propiedad-precio">$350.000.000 <small>COP</small></p>
          <div class="propiedad-footer">
            <span style="font-size:12px; color:var(--texto-suave)">Escrituras al día</span>
            <a class="btn-ver" href="https://wa.me/573218604753?text=Hola%2C%20me%20interesa%20la%20Casa%20Sector%20Niza" target="_blank" rel="noopener">Consultar</a>
          </div>
        </div>
      </div>

      <!-- PROPIEDAD 2 — REEMPLAZAR -->
      <div class="propiedad-card">
        <div class="propiedad-img">
          <div class="placeholder-img">
            <span>🏢</span>
            <p>Agregar foto de la propiedad</p>
          </div>
          <span class="badge-tipo">Apartamento</span>
        </div>
        <div class="propiedad-body">
          <p class="propiedad-zona">📍 Centro · Pasto</p>
          <h3 class="propiedad-nombre">Apto. Edificio Madrigal — Piso 4</h3>
          <div class="propiedad-specs">
            <span class="spec">🛏 2 hab.</span>
            <span class="spec">🚿 2 baños</span>
            <span class="spec">📐 85 m²</span>
            <span class="spec">🌇 Vista ciudad</span>
          </div>
          <p class="propiedad-precio">$220.000.000 <small>COP</small></p>
          <div class="propiedad-footer">
            <span style="font-size:12px; color:var(--texto-suave)">Piso 4 · Ascensor</span>
            <a class="btn-ver" href="https://wa.me/573218604753?text=Hola%2C%20me%20interesa%20el%20Apto%20Edificio%20Madrigal" target="_blank" rel="noopener">Consultar</a>
          </div>
        </div>
      </div>

      <!-- PROPIEDAD 3 — REEMPLAZAR -->
      <div class="propiedad-card">
        <div class="propiedad-img">
          <div class="placeholder-img">
            <span>🏡</span>
            <p>Agregar foto de la propiedad</p>
          </div>
          <span class="badge-tipo">Lote</span>
        </div>
        <div class="propiedad-body">
          <p class="propiedad-zona">📍 Sur de Pasto</p>
          <h3 class="propiedad-nombre">Lote Urbanizable — Sector Las Cuadras</h3>
          <div class="propiedad-specs">
            <span class="spec">📐 200 m²</span>
            <span class="spec">🛣 Vía principal</span>
            <span class="spec">⚡ Servicios</span>
          </div>
          <p class="propiedad-precio">$180.000.000 <small>COP</small></p>
          <div class="propiedad-footer">
            <span style="font-size:12px; color:var(--texto-suave)">Escrituras limpias</span>
            <a class="btn-ver" href="https://wa.me/573218604753?text=Hola%2C%20me%20interesa%20el%20Lote%20Las%20Cuadras" target="_blank" rel="noopener">Consultar</a>
          </div>
        </div>
      </div>

    </div>

    <div class="ver-mas-wrap">
      <a class="btn-outline" href="https://wa.me/573218604753?text=Hola%2C%20quiero%20ver%20todas%20las%20propiedades%20disponibles" target="_blank" rel="noopener">
        Ver todas las propiedades disponibles →
      </a>
    </div>
  </div>
</section>

<!-- PROCESO -->
<section class="proceso" id="proceso">
  <div class="container">
    <p class="section-label">Cómo trabajamos</p>
    <h2 class="section-title">Del primer contacto al cierre</h2>
    <p class="section-sub">Un proceso claro, sin sorpresas.</p>

    <div class="proceso-grid">
      <div class="proceso-step">
        <div class="proceso-num">1</div>
        <h3>Nos cuentas qué buscas</h3>
        <p>Por WhatsApp o el formulario de contacto. Zona, presupuesto, tipo de inmueble. Sin rodeos.</p>
      </div>
      <div class="proceso-step">
        <div class="proceso-num">2</div>
        <h3>Te mostramos opciones reales</h3>
        <p>En menos de 24 horas te enviamos propiedades que se ajustan exactamente a lo que necesitas.</p>
      </div>
      <div class="proceso-step">
        <div class="proceso-num">3</div>
        <h3>Visitamos la propiedad</h3>
        <p>Agendamos la visita en el momento que te quede bien. Te acompañamos y resolvemos todas tus dudas.</p>
      </div>
      <div class="proceso-step">
        <div class="proceso-num">4</div>
        <h3>Cerramos el negocio</h3>
        <p>Te asesoramos en la negociación, trámites y documentos hasta que la propiedad sea tuya.</p>
      </div>
    </div>
  </div>
</section>

<!-- CONTACTO -->
<section class="contacto" id="contacto">
  <div class="container">
    <p class="section-label">Contáctanos</p>
    <h2 class="section-title">¿Tienes una propiedad en mente?</h2>
    <p class="section-sub">Déjanos tus datos y un asesor te contacta en menos de 24 horas.</p>

    <div class="contacto-form">
      <div class="form-row">
        <div class="form-group">
          <label for="nombre">Nombre completo</label>
          <input type="text" id="nombre" placeholder="Tu nombre">
        </div>
        <div class="form-group">
          <label for="telefono">WhatsApp / Teléfono</label>
          <input type="tel" id="telefono" placeholder="+57 300 000 0000">
        </div>
      </div>
      <div class="form-group">
        <label for="tipo">¿Qué tipo de inmueble buscas?</label>
        <select id="tipo">
          <option value="">Seleccionar...</option>
          <option>Casa</option>
          <option>Apartamento</option>
          <option>Lote</option>
          <option>Local comercial</option>
          <option>Finca / rural</option>
          <option>Otro</option>
        </select>
      </div>
      <div class="form-group">
        <label for="presupuesto">Presupuesto aproximado</label>
        <select id="presupuesto">
          <option value="">Seleccionar...</option>
          <option>Menos de $150 millones COP</option>
          <option>$150M – $300M COP</option>
          <option>$300M – $500M COP</option>
          <option>Más de $500 millones COP</option>
        </select>
      </div>
      <div class="form-group">
        <label for="mensaje">¿Algo más que debamos saber?</label>
        <textarea id="mensaje" placeholder="Zona preferida, características importantes, etc."></textarea>
      </div>
      <button class="btn-submit" onclick="enviarPorWhatsApp()">
        <svg width="18" height="18" viewBox="0 0 24 24" fill="currentColor"><path d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347z"/><path d="M12 0C5.373 0 0 5.373 0 12c0 2.124.558 4.118 1.532 5.845L.057 23.492a.5.5 0 0 0 .614.644l5.939-1.56A11.945 11.945 0 0 0 12 24c6.627 0 12-5.373 12-12S18.627 0 12 0zm0 21.818a9.806 9.806 0 0 1-5.034-1.389l-.36-.214-3.733.98.998-3.648-.235-.374A9.808 9.808 0 0 1 2.182 12C2.182 6.57 6.57 2.182 12 2.182c5.43 0 9.818 4.388 9.818 9.818 0 5.43-4.388 9.818-9.818 9.818z"/></svg>
        Enviar consulta por WhatsApp
      </button>
      <p class="form-note">También puedes escribirnos directamente a <strong>+57 321 860 4753</strong></p>
    </div>
  </div>
</section>

<!-- FOOTER -->
<footer>
  <div class="footer-inner">
    <div class="footer-top">
      <div class="footer-brand">
        <div class="brand-name">VISTA AL SUR</div>
        <div class="brand-sub">Inmobiliaria</div>
        <p>Propiedades de calidad en las mejores zonas de Pasto, Nariño. Asesoría honesta y personalizada.</p>
      </div>
      <div class="footer-col">
        <h4>Navegación</h4>
        <a href="#portafolio">Portafolio</a>
        <a href="#proceso">Cómo trabajamos</a>
        <a href="#contacto">Contacto</a>
      </div>
      <div class="footer-col">
        <h4>Contacto</h4>
        <a href="https://wa.me/573218604753" target="_blank" rel="noopener">+57 321 860 4753</a>
        <a href="https://instagram.com/vistaalsur_inmobiliaria" target="_blank" rel="noopener">@vistaalsur_inmobiliaria</a>
        <a href="#">Pasto, Nariño · Colombia</a>
      </div>
    </div>
    <div class="footer-bottom">
      <span>© 2026 Vista al Sur Inmobiliaria. Todos los derechos reservados.</span>
      <div class="footer-social">
        <a href="https://instagram.com/vistaalsur_inmobiliaria" target="_blank" rel="noopener">Instagram</a>
        <a href="https://wa.me/573218604753" target="_blank" rel="noopener">WhatsApp</a>
      </div>
    </div>
  </div>
</footer>

<script>
  function enviarPorWhatsApp() {
    const nombre = document.getElementById('nombre').value.trim();
    const telefono = document.getElementById('telefono').value.trim();
    const tipo = document.getElementById('tipo').value;
    const presupuesto = document.getElementById('presupuesto').value;
    const mensaje = document.getElementById('mensaje').value.trim();

    if (!nombre || !telefono) {
      alert('Por favor completa tu nombre y teléfono.');
      return;
    }

    let texto = `Hola, me interesa una asesoría inmobiliaria.\n\n`;
    texto += `*Nombre:* ${nombre}\n`;
    texto += `*Teléfono:* ${telefono}\n`;
    if (tipo) texto += `*Tipo de inmueble:* ${tipo}\n`;
    if (presupuesto) texto += `*Presupuesto:* ${presupuesto}\n`;
    if (mensaje) texto += `*Mensaje:* ${mensaje}`;

    const url = `https://wa.me/573218604753?text=${encodeURIComponent(texto)}`;
    window.open(url, '_blank');
  }

  function toggleMenu(btn) {
    const links = document.querySelector('.nav-links');
    links.style.display = links.style.display === 'flex' ? 'none' : 'flex';
    links.style.flexDirection = 'column';
    links.style.position = 'absolute';
    links.style.top = '68px';
    links.style.left = '0';
    links.style.right = '0';
    links.style.background = 'white';
    links.style.padding = '1rem 2rem';
    links.style.borderBottom = '1px solid #d9d9d9';
    links.style.gap = '1rem';
  }
</script>

</body>
</html>
