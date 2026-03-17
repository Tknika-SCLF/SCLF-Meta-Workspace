---
layout: default
title: SCLF Meta-Workspace
---

<style>
  :root {
    --primary: #00d2ff;
    --secondary: #3a7bd5;
    --bg-dark: #0f172a;
    --card-bg: rgba(30, 41, 59, 0.7);
    --text-main: #f1f5f9;
    --text-dim: #94a3b8;
  }

  body {
    background-color: var(--bg-dark) !important;
    color: var(--text-main) !important;
    font-family: 'Outfit', sans-serif !important;
    margin: 0;
    padding: 0;
  }

  /* Force layout width */
  .container-lg, .wrapper, .inner {
    max-width: 1200px !important;
    margin: 0 auto !important;
    padding: 2rem !important;
    width: 95% !important;
  }

  header { background: transparent !important; border: none !important; display: none !important; }

  h1, h2, h3 { color: var(--primary) !important; border-bottom: none !important; }

  .banner-container {
    width: 100vw;
    position: relative;
    left: 50%;
    right: 50%;
    margin-left: -50vw;
    margin-right: -50vw;
    margin-bottom: 3rem;
    overflow: hidden;
    line-height: 0;
  }

  .banner-container img {
    width: 100%;
    height: auto;
    max-height: 450px;
    object-fit: cover;
    filter: brightness(0.8) contrast(1.1);
  }

  .hero-section {
    text-align: center;
    padding: 3rem 1rem;
    background: linear-gradient(180deg, rgba(0,210,255,0.15) 0%, transparent 100%);
    border-radius: 24px;
    margin-bottom: 4rem;
    border: 1px solid rgba(0, 210, 255, 0.1);
  }

  .grid-container {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
    gap: 2rem;
    margin-top: 2rem;
  }

  .card {
    background: var(--card-bg);
    backdrop-filter: blur(12px);
    -webkit-backdrop-filter: blur(12px);
    border: 1px solid rgba(255, 255, 255, 0.08);
    border-radius: 20px;
    padding: 2rem;
    transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    height: 100%;
    display: flex;
    flex-direction: column;
  }

  .card:hover {
    transform: translateY(-10px);
    box-shadow: 0 20px 40px rgba(0, 210, 255, 0.25);
    border-color: var(--primary);
    background: rgba(30, 41, 59, 0.9);
  }

  .card h3 {
    margin-top: 0;
    display: flex;
    align-items: center;
    gap: 12px;
    font-size: 1.4rem;
    margin-bottom: 1.5rem;
  }

  .card ul {
    list-style: none;
    padding: 0;
    margin: 0;
    flex-grow: 1;
  }

  .card li {
    margin-bottom: 1.5rem;
    position: relative;
    padding-left: 5px;
  }

  .card a {
    color: var(--primary);
    text-decoration: none;
    font-weight: 600;
    font-size: 1.1rem;
    transition: all 0.3s;
    display: inline-block;
  }

  .card a:hover { 
    color: #fff; 
    transform: translateX(5px);
    text-shadow: 0 0 10px var(--primary);
  }

  .card i {
    display: block;
    font-size: 0.9rem;
    color: var(--text-dim);
    font-style: normal;
    margin-top: 0.4rem;
    line-height: 1.4;
  }

  .status-badges {
    display: flex;
    justify-content: center;
    gap: 12px;
    flex-wrap: wrap;
    margin: 2rem 0;
  }

  .status-badges img {
    height: 28px;
    transition: transform 0.2s;
  }

  .status-badges img:hover {
    transform: scale(1.05);
  }

  .install-box {
    background: rgba(0, 0, 0, 0.3);
    border-radius: 12px;
    padding: 1.5rem;
    border-left: 4px solid var(--primary);
    margin: 2rem 0;
    font-family: 'Fira Code', 'Cascadia Code', monospace;
  }

  .footer {
    text-align: center;
    margin-top: 6rem;
    padding: 3rem;
    border-top: 1px solid rgba(255, 255, 255, 0.1);
    color: var(--text-dim);
    font-size: 0.95rem;
  }

  @media (max-width: 768px) {
    .inner, .wrapper, .container-lg {
      padding: 1rem !important;
      width: 100% !important;
    }
    .hero-section { padding: 2rem 1rem; }
    .banner-container img { max-height: 250px; }
  }
</style>

<div class="banner-container">
  <img src="assets/banner.png" alt="SCLF Platform Banner" />
</div>

<div class="inner">
  <div class="hero-section">
    <h1>🌌 SCLF Meta-Workspace</h1>
    <p style="font-size: 1.25rem; color: var(--text-dim);">Tknika-ko Smart Collaborative Learning Factory-a</p>

    <div class="status-badges">
      <a href="https://github.com/AiotR"><img src="https://img.shields.io/badge/Erakundea-AiotR-blue?style=for-the-badge&logo=github" alt="Erakundea" /></a>
      <a href="https://github.com/AiotR/SCLF-Meta-Workspace"><img src="https://img.shields.io/badge/Egoera-Aktibo-success?style=for-the-badge" alt="Egoera" /></a>
      <img src="https://img.shields.io/badge/Hizkuntza-Euskara-red?style=for-the-badge" alt="Hizkuntza" />
      <img src="https://img.shields.io/badge/Lizentzia-MIT-yellow?style=for-the-badge" alt="Lizentzia" />
    </div>
  </div>

  <section>
    <h2>🚀 Ikuspegi Orokorra</h2>
    <p style="font-size: 1.1rem; line-height: 1.6;">
      Gordailu honek **SCLF** (Smart Collaborative Learning Factory) plataformako osagai guztiak zentralizatzen ditu. 
      **Git Submodules** erabiltzen ditu modulu bakoitza era independentean kudeatzeko, sistemaren ikuspegi global bat mantenduz.
    </p>
  </section>

  <hr style="opacity: 0.1; margin: 4rem 0;">

  <section>
    <h2>🛠️ Sistemaren Moduluak</h2>
    <div class="grid-container">
      <div class="card">
        <h3>🤖 Produktuak</h3>
        <ul>
          <li>
            <a href="https://github.com/AiotR/SCLF_Gripper_v1.0">🦾 SCLF Gripper</a>
            <i>Aktuatzaileen eta matxarda robotikoen kontrola.</i>
          </li>
          <li>
            <a href="https://github.com/AiotR/sclf-drone">🛸 SCLF Drone</a>
            <i>Tripulatu gabeko aire-sistemak.</i>
          </li>
          <li>
            <a href="https://github.com/AiotR/sclf-quadruped-robot">🐕 SCLF Quadruped</a>
            <i>Lau hanka dituen plataforma robotikoa.</i>
          </li>
        </ul>
      </div>

      <div class="card">
        <h3>📊 Prozesua</h3>
        <ul>
          <li>
            <a href="https://github.com/AiotR/sclf-bom-registry">📋 BOM Erregistroa</a>
            <i>Materialen eta osagaien kudeaketa.</i>
          </li>
          <li>
            <a href="https://github.com/AiotR/pruebaDocker">🏭 IkasMES</a>
            <i>Manufacturing Execution System.</i>
          </li>
          <li>
            <a href="https://github.com/AiotR/sclf-manufacturing-processes">⚙️ Fabrikazio Prozesuak</a>
            <i>Industria prozesuen definizioa.</i>
          </li>
        </ul>
      </div>

      <div class="card">
        <h3>📚 Formakuntza</h3>
        <ul>
          <li>
            <a href="https://github.com/AiotR/sclf-educational-content">📖 Hezkuntza Edukia</a>
            <i>Material didaktikoa eta tutorialak.</i>
          </li>
          <li>
            <a href="https://github.com/AiotR/sclf-tknika-project-hub">🏠 Proiektu Hub-a</a>
            <i>Tknikako koordinazio zentroa.</i>
          </li>
        </ul>
      </div>

      <div class="card">
        <h3>✅ Estandarrak</h3>
        <ul>
          <li>
            <a href="https://github.com/AiotR/sclf-quality">🛡️ Kalitatea</a>
            <i>Kalitate kontrola eta araudiak.</i>
          </li>
          <li>
            <a href="https://github.com/AiotR/sclf-templates">📄 Txantiloiak</a>
            <i>Diseinu eta dokumentazio txantiloiak.</i>
          </li>
        </ul>
      </div>
    </div>
  </section>

  <section style="margin-top: 5rem;">
    <h2>📥 Ingurunearen Konfigurazioa</h2>
    <p>Ekosistema osoarekin lanean hasteko, klonatu gordailu hau `--recursive` flag-a erabiliz:</p>
    
    <div class="install-box">
      <code>git clone --recursive https://github.com/AiotR/SCLF-Meta-Workspace.git</code>
    </div>

    <h3>💡 Komando Erabilgarriak</h3>
    <ul>
      <li><strong>Dena eguneratu:</strong> <code>git submodule update --remote --merge</code></li>
      <li><strong>Modulu berria gehitu:</strong> <code>git submodule add [URL] [izena]</code></li>
    </ul>
  </section>

  <div class="footer">
    <p><b>Antigravity AI</b>-k maitasunez garatua <b>AiotR</b> lantaldearentzat</p>
    <p>© 2024 SCLF Ecosystem | Tknika</p>
  </div>
</div>
