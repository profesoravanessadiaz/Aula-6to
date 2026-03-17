[index.html](https://github.com/user-attachments/files/26041702/index.html)
<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<!-- ===================== SEO BÁSICO ===================== -->
<title>Aula Matemática 6° Básico | Ejercicios Interactivos Chile</title>
<meta name="description" content="Plataforma gratuita de matemáticas para 6° básico Chile. Ejercicios interactivos, quizzes y práctica de fracciones, decimales, álgebra, geometría, probabilidades y gráficos. Alineada al programa Mineduc 2012.">
<meta name="keywords" content="matemáticas 6° básico, ejercicios matemáticas Chile, fracciones sexto básico, álgebra primaria, geometría 6to básico, probabilidades primaria, Mineduc matemáticas, aula matemática, docentes Chile, recursos educativos matemáticas">
<meta name="author" content="Aula Matemática Chile">
<meta name="robots" content="index, follow">
<meta name="language" content="Spanish">
<meta name="revisit-after" content="7 days">
<link rel="canonical" href="https://www.aulamatematica.cl/">

<!-- ===================== OPEN GRAPH (redes sociales) ===================== -->
<meta property="og:type" content="website">
<meta property="og:url" content="https://www.aulamatematica.cl/">
<meta property="og:title" content="Aula Matemática 6° Básico | Ejercicios Interactivos Chile">
<meta property="og:description" content="Plataforma gratuita con ejercicios interactivos y quizzes de matemáticas para 6° básico, alineada al programa Mineduc. Fracciones, álgebra, geometría, probabilidades y más.">
<meta property="og:locale" content="es_CL">
<meta property="og:site_name" content="Aula Matemática">

<!-- ===================== TWITTER CARD ===================== -->
<meta name="twitter:card" content="summary_large_image">
<meta name="twitter:title" content="Aula Matemática 6° Básico | Ejercicios Interactivos Chile">
<meta name="twitter:description" content="Ejercicios interactivos y quizzes de matemáticas para 6° básico Chile. Gratis, sin registro, alineado al programa Mineduc.">

<!-- ===================== DATOS ESTRUCTURADOS (Schema.org) ===================== -->
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "WebApplication",
  "name": "Aula Matemática 6° Básico",
  "description": "Plataforma educativa gratuita con ejercicios interactivos de matemáticas para 6° básico, alineada al programa de estudio Mineduc Chile 2012.",
  "url": "https://www.aulamatematica.cl/",
  "applicationCategory": "EducationalApplication",
  "educationalLevel": "Primaria",
  "inLanguage": "es-CL",
  "isAccessibleForFree": true,
  "audience": {
    "@type": "EducationalAudience",
    "educationalRole": ["student", "teacher"],
    "educationalLevel": "6° Básico"
  },
  "about": {
    "@type": "Thing",
    "name": "Matemáticas 6° Básico Chile"
  },
  "creator": {
    "@type": "Organization",
    "name": "Aula Matemática Chile"
  }
}
</script>

<!-- ===================== FAVICON (emoji como ícono) ===================== -->
<link rel="icon" href="data:image/svg+xml,<svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 100 100'><text y='.9em' font-size='90'>🧮</text></svg>">
<link rel="apple-touch-icon" href="data:image/svg+xml,<svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 100 100'><text y='.9em' font-size='90'>🧮</text></svg>">

<link href="https://fonts.googleapis.com/css2?family=Syne:wght@400;600;700;800&family=JetBrains+Mono:wght@300;400;500&display=swap" rel="stylesheet">
<style>
  :root {
    --bg: #0a0a0f;
    --surface: #12121a;
    --surface2: #1a1a26;
    --border: #2a2a3e;
    --accent: #6c63ff;
    --accent2: #ff6584;
    --accent3: #43e97b;
    --accent4: #f7971e;
    --text: #e8e8f0;
    --text-muted: #7878a0;
    --glow: 0 0 30px rgba(108,99,255,0.3);
  }

  * { margin: 0; padding: 0; box-sizing: border-box; }

  body {
    font-family: 'Syne', sans-serif;
    background: var(--bg);
    color: var(--text);
    min-height: 100vh;
    overflow-x: hidden;
  }

  /* BG GRID */
  body::before {
    content: '';
    position: fixed;
    inset: 0;
    background-image:
      linear-gradient(rgba(108,99,255,0.04) 1px, transparent 1px),
      linear-gradient(90deg, rgba(108,99,255,0.04) 1px, transparent 1px);
    background-size: 40px 40px;
    pointer-events: none;
    z-index: 0;
  }

  /* ---- HEADER ---- */
  header {
    position: relative;
    z-index: 10;
    padding: 20px 40px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    border-bottom: 1px solid var(--border);
    backdrop-filter: blur(10px);
    background: rgba(10,10,15,0.8);
    position: sticky;
    top: 0;
  }

  .logo {
    font-size: 1.4rem;
    font-weight: 800;
    letter-spacing: -1px;
    background: linear-gradient(135deg, var(--accent), var(--accent2));
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
  }

  .logo span { font-family: 'JetBrains Mono', monospace; font-weight: 300; }

  .score-bar {
    display: flex;
    gap: 20px;
    align-items: center;
  }

  .score-item {
    font-family: 'JetBrains Mono', monospace;
    font-size: 0.85rem;
    color: var(--text-muted);
  }

  .score-item strong {
    color: var(--accent3);
    font-size: 1.1rem;
  }

  /* ---- MAIN ---- */
  main {
    position: relative;
    z-index: 1;
    max-width: 1100px;
    margin: 0 auto;
    padding: 40px 20px;
  }

  /* ---- SCREENS ---- */
  .screen { display: none; }
  .screen.active { display: block; }

  /* ---- HOME ---- */
  .home-hero {
    text-align: center;
    padding: 60px 20px 40px;
  }

  .home-hero h1 {
    font-size: clamp(2.5rem, 6vw, 4.5rem);
    font-weight: 800;
    letter-spacing: -2px;
    line-height: 1.1;
    margin-bottom: 20px;
  }

  .home-hero h1 em {
    font-style: normal;
    background: linear-gradient(135deg, var(--accent), var(--accent2));
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
  }

  .home-hero p {
    font-family: 'JetBrains Mono', monospace;
    color: var(--text-muted);
    font-size: 1rem;
    max-width: 500px;
    margin: 0 auto 50px;
    line-height: 1.7;
  }

  .modules-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 20px;
    margin-top: 20px;
  }

  .module-card {
    background: var(--surface);
    border: 1px solid var(--border);
    border-radius: 16px;
    padding: 30px;
    cursor: pointer;
    transition: all 0.3s ease;
    position: relative;
    overflow: hidden;
    text-align: left;
  }

  .module-card::before {
    content: '';
    position: absolute;
    inset: 0;
    opacity: 0;
    transition: opacity 0.3s;
    border-radius: 16px;
  }

  .module-card:nth-child(1)::before { background: linear-gradient(135deg, rgba(108,99,255,0.1), transparent); }
  .module-card:nth-child(2)::before { background: linear-gradient(135deg, rgba(255,101,132,0.1), transparent); }
  .module-card:nth-child(3)::before { background: linear-gradient(135deg, rgba(67,233,123,0.1), transparent); }

  .module-card:hover::before { opacity: 1; }
  .module-card:hover { transform: translateY(-4px); border-color: var(--accent); box-shadow: var(--glow); }

  .module-icon {
    font-size: 2.5rem;
    margin-bottom: 16px;
    display: block;
  }

  .module-card h3 {
    font-size: 1.2rem;
    font-weight: 700;
    margin-bottom: 8px;
  }

  .module-card p {
    font-family: 'JetBrains Mono', monospace;
    font-size: 0.78rem;
    color: var(--text-muted);
    line-height: 1.6;
    margin-bottom: 20px;
  }

  .tag-row { display: flex; gap: 6px; flex-wrap: wrap; margin-bottom: 20px; }

  .tag {
    font-family: 'JetBrains Mono', monospace;
    font-size: 0.65rem;
    padding: 3px 8px;
    border-radius: 4px;
    border: 1px solid var(--border);
    color: var(--text-muted);
  }

  .btn {
    display: inline-flex;
    align-items: center;
    gap: 8px;
    padding: 10px 20px;
    border-radius: 8px;
    font-family: 'Syne', sans-serif;
    font-weight: 600;
    font-size: 0.85rem;
    cursor: pointer;
    border: none;
    transition: all 0.2s;
  }

  .btn-primary {
    background: var(--accent);
    color: white;
  }
  .btn-primary:hover { background: #8880ff; transform: scale(1.02); }

  .btn-secondary {
    background: var(--surface2);
    color: var(--text);
    border: 1px solid var(--border);
  }
  .btn-secondary:hover { border-color: var(--accent); color: var(--accent); }

  .btn-success {
    background: var(--accent3);
    color: #0a0a0f;
  }

  .btn-danger {
    background: var(--accent2);
    color: white;
  }

  /* ---- LESSON SCREEN ---- */
  .lesson-header {
    display: flex;
    align-items: center;
    gap: 16px;
    margin-bottom: 30px;
  }

  .back-btn {
    background: var(--surface2);
    border: 1px solid var(--border);
    color: var(--text-muted);
    padding: 8px 14px;
    border-radius: 8px;
    cursor: pointer;
    font-family: 'JetBrains Mono', monospace;
    font-size: 0.8rem;
    transition: all 0.2s;
  }
  .back-btn:hover { color: var(--accent); border-color: var(--accent); }

  .lesson-title {
    font-size: 1.6rem;
    font-weight: 800;
    letter-spacing: -1px;
  }

  /* TABS */
  .tabs {
    display: flex;
    gap: 4px;
    background: var(--surface);
    padding: 6px;
    border-radius: 12px;
    border: 1px solid var(--border);
    margin-bottom: 30px;
    width: fit-content;
  }

  .tab {
    padding: 8px 20px;
    border-radius: 8px;
    font-size: 0.85rem;
    font-weight: 600;
    cursor: pointer;
    transition: all 0.2s;
    color: var(--text-muted);
    border: none;
    background: transparent;
    font-family: 'Syne', sans-serif;
  }

  .tab.active {
    background: var(--accent);
    color: white;
  }

  .tab-content { display: none; }
  .tab-content.active { display: block; }

  /* THEORY CONTENT */
  .theory-block {
    background: var(--surface);
    border: 1px solid var(--border);
    border-radius: 16px;
    padding: 30px;
    margin-bottom: 20px;
  }

  .theory-block h3 {
    font-size: 1.1rem;
    font-weight: 700;
    margin-bottom: 16px;
    color: var(--accent);
  }

  .theory-block p {
    font-family: 'JetBrains Mono', monospace;
    font-size: 0.85rem;
    color: var(--text-muted);
    line-height: 1.8;
    margin-bottom: 12px;
  }

  .formula-box {
    background: var(--bg);
    border: 1px solid var(--accent);
    border-radius: 10px;
    padding: 16px 20px;
    font-family: 'JetBrains Mono', monospace;
    font-size: 1rem;
    color: var(--accent);
    margin: 16px 0;
    text-align: center;
    letter-spacing: 0.5px;
  }

  .example-row {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 12px;
    margin-top: 16px;
  }

  .example-item {
    background: var(--bg);
    border: 1px solid var(--border);
    border-radius: 8px;
    padding: 12px 16px;
    font-family: 'JetBrains Mono', monospace;
    font-size: 0.85rem;
  }

  .example-item .ex-label {
    font-size: 0.7rem;
    color: var(--text-muted);
    margin-bottom: 6px;
  }

  .example-item .ex-math { color: var(--accent3); }

  .steps-list {
    list-style: none;
    counter-reset: steps;
  }

  .steps-list li {
    counter-increment: steps;
    display: flex;
    gap: 14px;
    margin-bottom: 12px;
    font-family: 'JetBrains Mono', monospace;
    font-size: 0.82rem;
    color: var(--text-muted);
    line-height: 1.6;
  }

  .steps-list li::before {
    content: counter(steps);
    min-width: 24px;
    height: 24px;
    background: var(--accent);
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 0.75rem;
    color: white;
    font-weight: 700;
    flex-shrink: 0;
  }

  /* EXERCISE */
  .exercise-card {
    background: var(--surface);
    border: 1px solid var(--border);
    border-radius: 16px;
    padding: 36px;
    margin-bottom: 20px;
  }

  .ex-meta {
    display: flex;
    justify-content: space-between;
    margin-bottom: 24px;
    font-family: 'JetBrains Mono', monospace;
    font-size: 0.75rem;
    color: var(--text-muted);
  }

  .difficulty {
    padding: 3px 10px;
    border-radius: 4px;
    font-size: 0.7rem;
    font-weight: 600;
  }
  .diff-easy { background: rgba(67,233,123,0.15); color: var(--accent3); }
  .diff-medium { background: rgba(247,151,30,0.15); color: var(--accent4); }
  .diff-hard { background: rgba(255,101,132,0.15); color: var(--accent2); }

  .ex-question {
    font-size: 1.6rem;
    font-weight: 700;
    font-family: 'JetBrains Mono', monospace;
    text-align: center;
    padding: 30px;
    background: var(--bg);
    border-radius: 12px;
    margin-bottom: 24px;
    letter-spacing: 1px;
    color: var(--text);
    min-height: 100px;
    display: flex;
    align-items: center;
    justify-content: center;
  }

  .options-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 12px;
    margin-bottom: 20px;
  }

  .option-btn {
    background: var(--surface2);
    border: 2px solid var(--border);
    border-radius: 10px;
    padding: 16px;
    cursor: pointer;
    font-family: 'JetBrains Mono', monospace;
    font-size: 1rem;
    color: var(--text);
    transition: all 0.2s;
    text-align: center;
  }

  .option-btn:hover:not(:disabled) {
    border-color: var(--accent);
    color: var(--accent);
    background: rgba(108,99,255,0.1);
  }

  .option-btn.correct {
    border-color: var(--accent3);
    background: rgba(67,233,123,0.15);
    color: var(--accent3);
  }

  .option-btn.wrong {
    border-color: var(--accent2);
    background: rgba(255,101,132,0.15);
    color: var(--accent2);
  }

  .feedback-box {
    padding: 16px 20px;
    border-radius: 10px;
    font-family: 'JetBrains Mono', monospace;
    font-size: 0.85rem;
    line-height: 1.6;
    margin-bottom: 20px;
    display: none;
  }

  .feedback-box.show { display: block; }
  .feedback-box.correct { background: rgba(67,233,123,0.1); border: 1px solid var(--accent3); color: var(--accent3); }
  .feedback-box.wrong { background: rgba(255,101,132,0.1); border: 1px solid var(--accent2); color: var(--accent2); }

  /* INPUT EXERCISE */
  .input-group {
    display: flex;
    gap: 10px;
    margin-bottom: 20px;
  }

  .math-input {
    flex: 1;
    background: var(--bg);
    border: 2px solid var(--border);
    border-radius: 10px;
    padding: 14px 18px;
    font-family: 'JetBrains Mono', monospace;
    font-size: 1.2rem;
    color: var(--text);
    outline: none;
    transition: border-color 0.2s;
    text-align: center;
  }

  .math-input:focus { border-color: var(--accent); }
  .math-input.correct { border-color: var(--accent3); }
  .math-input.wrong { border-color: var(--accent2); }

  /* PROGRESS BAR */
  .progress-wrap {
    background: var(--border);
    border-radius: 4px;
    height: 4px;
    margin-bottom: 30px;
    overflow: hidden;
  }

  .progress-fill {
    height: 100%;
    background: linear-gradient(90deg, var(--accent), var(--accent2));
    border-radius: 4px;
    transition: width 0.4s ease;
  }

  /* QUIZ SCREEN */
  .quiz-header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 20px;
    font-family: 'JetBrains Mono', monospace;
    font-size: 0.82rem;
    color: var(--text-muted);
  }

  /* RESULTS */
  .results-card {
    background: var(--surface);
    border: 1px solid var(--border);
    border-radius: 20px;
    padding: 50px 40px;
    text-align: center;
    max-width: 500px;
    margin: 40px auto;
  }

  .score-display {
    font-size: 5rem;
    font-weight: 800;
    font-family: 'JetBrains Mono', monospace;
    background: linear-gradient(135deg, var(--accent), var(--accent3));
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    margin-bottom: 10px;
  }

  .score-label {
    font-family: 'JetBrains Mono', monospace;
    color: var(--text-muted);
    font-size: 0.85rem;
    margin-bottom: 30px;
  }

  .results-breakdown {
    display: flex;
    justify-content: center;
    gap: 30px;
    margin-bottom: 30px;
  }

  .res-item { text-align: center; }
  .res-num {
    font-size: 1.8rem;
    font-weight: 800;
    font-family: 'JetBrains Mono', monospace;
  }
  .res-num.good { color: var(--accent3); }
  .res-num.bad { color: var(--accent2); }
  .res-label { font-family: 'JetBrains Mono', monospace; font-size: 0.75rem; color: var(--text-muted); }

  /* HINT */
  .hint-btn {
    background: none;
    border: 1px dashed var(--border);
    color: var(--text-muted);
    padding: 8px 16px;
    border-radius: 6px;
    cursor: pointer;
    font-family: 'JetBrains Mono', monospace;
    font-size: 0.75rem;
    transition: all 0.2s;
  }
  .hint-btn:hover { border-color: var(--accent4); color: var(--accent4); }

  .hint-box {
    background: rgba(247,151,30,0.08);
    border: 1px solid rgba(247,151,30,0.3);
    border-radius: 8px;
    padding: 12px 16px;
    font-family: 'JetBrains Mono', monospace;
    font-size: 0.8rem;
    color: var(--accent4);
    margin-top: 10px;
    display: none;
  }
  .hint-box.show { display: block; }

  /* NAV DOTS */
  .nav-dots {
    display: flex;
    gap: 6px;
    justify-content: center;
    margin-top: 20px;
  }
  .dot {
    width: 8px; height: 8px;
    border-radius: 50%;
    background: var(--border);
    transition: all 0.2s;
  }
  .dot.done { background: var(--accent3); }
  .dot.active { background: var(--accent); width: 20px; border-radius: 4px; }
  .dot.wrong-dot { background: var(--accent2); }

  /* Responsive */
  @media (max-width: 600px) {
    header { padding: 14px 20px; }
    .options-grid { grid-template-columns: 1fr; }
    .example-row { grid-template-columns: 1fr; }
    .exercise-card { padding: 24px; }
  }

  /* ANIMATIONS */
  @keyframes fadeIn {
    from { opacity: 0; transform: translateY(20px); }
    to { opacity: 1; transform: translateY(0); }
  }

  .screen.active { animation: fadeIn 0.3s ease; }

  @keyframes pulse {
    0%, 100% { transform: scale(1); }
    50% { transform: scale(1.05); }
  }
  .pulse { animation: pulse 0.4s ease; }

  /* Celebration */
  @keyframes confetti-fall {
    0% { transform: translateY(-10px) rotate(0deg); opacity: 1; }
    100% { transform: translateY(100vh) rotate(720deg); opacity: 0; }
  }

  .confetti-piece {
    position: fixed;
    width: 8px;
    height: 8px;
    border-radius: 2px;
    animation: confetti-fall 2s ease-in forwards;
    z-index: 1000;
    pointer-events: none;
  }
</style>
</head>
<body>

<header>
  <div class="logo">Aula<span> Matemática</span></div>
  <div class="score-bar">
    <div class="score-item">Puntos: <strong id="total-score">0</strong></div>
    <div class="score-item">Racha: <strong id="streak" style="color: var(--accent4)">🔥 0</strong></div>
  </div>
</header>

<main>

  <!-- HOME SCREEN -->
  <div class="screen active" id="screen-home">
    <div class="home-hero">
      <h1>Desafíos<br><em>Matemáticos</em><br>6to Básico 2026</h1>
      <p>Aprende, practica y desafíate. Ejercicios interactivos + quiz</p>
    </div>

    <div class="modules-grid">

      <div class="module-card" onclick="openModule('combinadas')">
        <span class="module-icon">⚙️</span>
        <h3>Operaciones Combinadas en los Números Naturales</h3>
        <p>Jerarquía de operaciones en los números naturales. Paréntesis, potencias, multiplicación, división, suma y resta.</p>
        <div class="tag-row">
          <span class="tag">PEMDAS/BODMAS</span>
          <span class="tag">Naturales</span>
          <span class="tag">Jerarquía</span>
        </div>
        <button class="btn btn-primary">Comenzar →</button>
      </div>

      <div class="module-card" onclick="openModule('fracciones')">
        <span class="module-icon">🔢</span>
        <h3>Fracciones y Decimales</h3>
        <p>Suma, resta, multiplicación y división de fracciones. Conversión a decimales y viceversa. MCM y MCD.</p>
        <div class="tag-row">
          <span class="tag">Fracciones</span>
          <span class="tag">Decimales</span>
          <span class="tag">MCM/MCD</span>
        </div>
        <button class="btn btn-primary" style="background: var(--accent2)">Comenzar →</button>
      </div>

      <div class="module-card" onclick="openModule('algebra')">
        <span class="module-icon">📐</span>
        <h3>Álgebra y Ecuaciones</h3>
        <p>Variables, expresiones algebraicas, ecuaciones de primer y segundo grado. Sistemas de ecuaciones.</p>
        <div class="tag-row">
          <span class="tag">Ecuaciones</span>
          <span class="tag">Variables</span>
          <span class="tag">Sistemas</span>
        </div>
        <button class="btn btn-success">Comenzar →</button>
      </div>

      <div class="module-card" onclick="openModule('basicfracciones')">
        <span class="module-icon">½</span>
        <h3>Operaciones Básicas con Fracciones</h3>
        <p>Suma, resta, multiplicación y división de fracciones paso a paso. Nivel básico para afianzar fundamentos.</p>
        <div class="tag-row">
          <span class="tag">Suma</span>
          <span class="tag">Resta</span>
          <span class="tag">× y ÷</span>
          <span class="tag">Básico</span>
        </div>
        <button class="btn btn-primary" style="background: var(--accent4)">Comenzar →</button>
      </div>

      <div class="module-card" onclick="openModule('decimales')">
        <span class="module-icon">0.5</span>
        <h3>Operaciones Básicas con Decimales</h3>
        <p>Suma, resta, multiplicación y división de números decimales. Entiende el valor posicional y el manejo del punto decimal.</p>
        <div class="tag-row">
          <span class="tag">Suma</span>
          <span class="tag">Resta</span>
          <span class="tag">× y ÷</span>
          <span class="tag">Decimales</span>
        </div>
        <button class="btn btn-primary" style="background: #00c9b1">Comenzar →</button>
      </div>

      <div class="module-card" onclick="openModule('graficos')">
        <span class="module-icon">📊</span>
        <h3>Representación y Análisis de Gráficos</h3>
        <p>Interpreta y analiza gráficos de barras, líneas y circulares. Lee datos, compara valores y extrae conclusiones.</p>
        <div class="tag-row">
          <span class="tag">Barras</span>
          <span class="tag">Líneas</span>
          <span class="tag">Circular</span>
          <span class="tag">Análisis</span>
        </div>
        <button class="btn btn-primary" style="background: #a855f7">Comenzar →</button>
      </div>

      <div class="module-card" onclick="openModule('probabilidades')">
        <span class="module-icon">🎲</span>
        <h3>Probabilidades y Azar</h3>
        <p>Conjetura sobre resultados de experimentos con dados y monedas. Calcula probabilidades usando fracciones y diagramas de árbol.</p>
        <div class="tag-row">
          <span class="tag">Dados</span>
          <span class="tag">Monedas</span>
          <span class="tag">Fracciones</span>
          <span class="tag">Árbol</span>
        </div>
        <button class="btn btn-primary" style="background: #e11d48">Comenzar →</button>
      </div>

      <div class="module-card" onclick="openModule('geometria')">
        <span class="module-icon">📐</span>
        <h3>Geometría: Ángulos y Figuras 3D</h3>
        <p>Calcula ángulos en triángulos y cuadriláteros, identifica tipos de triángulos y calcula superficies y volúmenes de cubos y paralelepípedos.</p>
        <div class="tag-row">
          <span class="tag">Ángulos</span>
          <span class="tag">Triángulos</span>
          <span class="tag">Volumen</span>
          <span class="tag">Superficie</span>
        </div>
        <button class="btn btn-primary" style="background: #0ea5e9">Comenzar →</button>
      </div>

    </div>
  </div>

  <!-- LESSON SCREEN -->
  <div class="screen" id="screen-lesson">
    <div class="lesson-header">
      <button class="back-btn" onclick="goHome()">← Volver</button>
      <h2 class="lesson-title" id="lesson-title">Módulo</h2>
    </div>

    <div class="tabs">
      <button class="tab active" onclick="switchTab('practice')">✏️ Práctica</button>
      <button class="tab" onclick="switchTab('quiz')">🎯 Quiz</button>
    </div>

    <!-- PRACTICE -->
    <div class="tab-content active" id="tab-practice">
      <div class="progress-wrap">
        <div class="progress-fill" id="practice-progress" style="width:0%"></div>
      </div>
      <div id="practice-content"></div>
      <div class="nav-dots" id="practice-dots"></div>
    </div>

    <!-- QUIZ -->
    <div class="tab-content" id="tab-quiz">
      <div id="quiz-content"></div>
    </div>

  </div>

</main>

<footer style="
  background: #0a0a0f;
  border-top: 1px solid #2a2a3e;
  padding: 20px;
  text-align: center;
  font-family: 'JetBrains Mono', monospace;
  font-size: 0.75rem;
  color: #7878a0;
  line-height: 1.8;
">
  <p>🧮 <strong style="color:#6c63ff">Aula Matemática</strong> · Ejercicios para 6° Básico Chile</p>
  <p>Alineado al Programa de Estudio Matemática 6° Básico · Mineduc 2012</p>
  <p style="margin-top:6px; font-size:0.68rem;">
    © <span id="footer-year"></span> Aula Matemática Chile · Uso educativo libre · Prohibida su venta o modificación sin autorización
  </p>
  <script>document.getElementById('footer-year').textContent = new Date().getFullYear();</script>
</footer>
// =====================
//  STATE
// =====================
let totalScore = 0;
let streak = 0;
let currentModule = null;
let practiceIdx = 0;
let practiceAnswered = [];
let quizActive = false;
let quizIdx = 0;
let quizScore = 0;
let quizWrong = 0;
let quizAnswered = [];

// =====================
// MODULES DATA
// =====================
const modules = {

  combinadas: {
    title: "⚙️ Operaciones Combinadas en los Números Naturales",
    practice: [
      { q: "Resuelve: 5 + 3 × 4", type: "mc", opts: ["32","17","23","20"], ans: 1, hint: "Según la jerarquía, la multiplicación va antes que la suma.", exp: "Primero 3×4=12, luego 5+12=17. (OA 2)" },
      { q: "Resuelve: (8 + 2) × 3", type: "mc", opts: ["14","30","26","22"], ans: 1, hint: "Primero resuelve lo que está dentro del paréntesis.", exp: "Paréntesis: 8+2=10. Luego 10×3=30. (OA 2)" },
      { q: "En la frutería, hay 4 cajas con 12 manzanas cada una y se vendieron 15. ¿Cuántas quedan?", type: "mc", opts: ["33","48","13","43"], ans: 0, hint: "Primero calcula el total: 4×12. Luego resta las vendidas.", exp: "4×12=48. 48−15=33 manzanas. (OA 2)" },
      { q: "Resuelve: 60 ÷ (2 + 4) × 3", type: "input", ans: "30", hint: "Resuelve el paréntesis primero: 2+4=6. Luego opera de izquierda a derecha.", exp: "2+4=6. 60÷6=10. 10×3=30. (OA 2)" },
      { q: "Un bus tiene 5 filas con 8 asientos. Si viajan 3 buses, ¿cuántos pasajeros caben en total?", type: "mc", opts: ["40","120","16","24"], ans: 1, hint: "Primero calcula asientos por bus, luego multiplica por 3.", exp: "5×8=40 por bus. 40×3=120 en total. (OA 2)" },
      { q: "Resuelve: 100 − 4 × (5 + 3)", type: "input", ans: "68", hint: "Paréntesis primero: 5+3=8. Luego multiplica: 4×8=32. Finalmente resta.", exp: "5+3=8 → 4×8=32 → 100−32=68. (OA 2)" },
      { q: "Sofía tiene $12 000. Compra 3 cuadernos a $2 500 y 2 lápices a $500. ¿Cuánto le sobra?", type: "mc", opts: ["$3 000","$4 500","$2 500","$5 000"], ans: 0, hint: "Calcula el gasto total y réstalo al dinero inicial.", exp: "3×2500=7500. 2×500=1000. Gasto=8500. 12000−8500=$3000. (OA 2)" },
      { q: "Resuelve: 24 ÷ 4 + 3 × 5 − 2", type: "input", ans: "19", hint: "Primero las divisiones y multiplicaciones, luego sumas y restas.", exp: "24÷4=6. 3×5=15. 6+15−2=19. (OA 2)" },
    ],
    quiz: [
      { q: "¿Cuánto es 8 + 6 ÷ 2?", opts: ["7","11","14","10"], ans: 1 },
      { q: "¿Cuánto es (10 − 4) × 3?", opts: ["18","24","22","30"], ans: 0 },
      { q: "Pedro tiene 5 bolsas con 9 canicas. Regala 12. ¿Cuántas le quedan?", opts: ["45","33","42","27"], ans: 1 },
      { q: "¿Cuánto es 50 − 3 × (2 + 5)?", opts: ["21","29","35","23"], ans: 1 },
      { q: "¿Cuánto es 36 ÷ 6 + 4 × 2?", opts: ["14","16","22","12"], ans: 0 },
      { q: "Una tienda vende 7 paquetes de 8 galletas. Si se devuelven 2 paquetes, ¿cuántas galletas quedaron vendidas?", opts: ["40","56","24","16"], ans: 0 },
    ]
  },

  fracciones: {
    title: "🔢 Fracciones y Decimales",
    practice: [
      { q: "Camila comió 3/8 de una pizza y su hermano 2/8. ¿Qué fracción comieron entre los dos?", type: "mc", opts: ["5/16","5/8","6/8","1/2"], ans: 1, hint: "Mismo denominador: suma los numeradores directamente.", exp: "3/8 + 2/8 = 5/8. (OA 6)" },
      { q: "Expresa la fracción impropia 7/3 como número mixto.", type: "mc", opts: ["2 y 1/3","3 y 1/7","1 y 4/3","2 y 2/3"], ans: 0, hint: "Divide 7÷3. El cociente es la parte entera y el resto es el numerador.", exp: "7÷3=2 con resto 1. Entonces 7/3 = 2 y 1/3. (OA 5)" },
      { q: "Suma: 1/2 + 1/4 = ?", type: "mc", opts: ["2/6","3/4","2/4","1/3"], ans: 1, hint: "MCM(2,4)=4. Convierte 1/2 a fracción equivalente con denominador 4.", exp: "1/2=2/4. Luego 2/4+1/4=3/4. (OA 6)" },
      { q: "En una receta se usan 1 y 1/2 tazas de harina y 3/4 de taza de azúcar. ¿Cuántas tazas de ingredientes secos hay en total?", type: "mc", opts: ["2 y 1/4","1 y 3/4","2 y 3/4","3 y 1/4"], ans: 0, hint: "Suma el número mixto con la fracción: 1+1/2+3/4.", exp: "1/2=2/4. 2/4+3/4=5/4=1y1/4. Total: 1+1y1/4=2y1/4. (OA 8)" },
      { q: "Expresa 25% como fracción en su mínima expresión.", type: "mc", opts: ["25/100","5/20","1/4","2/8"], ans: 2, hint: "25% = 25/100. Simplifica dividiendo numerador y denominador entre 25.", exp: "25/100 ÷ 25 = 1/4. (OA 4)" },
      { q: "En un curso de 40 alumnos, el 50% son niñas. ¿Cuántas niñas hay?", type: "input", ans: "20", hint: "50% significa la mitad. Divide 40 entre 2.", exp: "50% de 40 = 40÷2 = 20 niñas. (OA 4)" },
      { q: "Resta: 3/4 − 1/3 = ?", type: "mc", opts: ["2/1","5/12","1/12","7/12"], ans: 1, hint: "MCM(4,3)=12. Convierte ambas fracciones a denominador 12.", exp: "3/4=9/12. 1/3=4/12. 9/12−4/12=5/12. (OA 6)" },
      { q: "Expresa el número mixto 2 y 3/5 como fracción impropia.", type: "input", ans: "13/5", hint: "Multiplica la parte entera por el denominador y suma el numerador.", exp: "2×5=10. 10+3=13. Resultado: 13/5. (OA 5)" },
    ],
    quiz: [
      { q: "¿Cuánto es 1/3 + 1/3?", opts: ["2/9","2/6","2/3","1/3"], ans: 2 },
      { q: "Expresa 9/4 como número mixto.", opts: ["2 y 1/4","4 y 1/2","2 y 3/4","3 y 1/4"], ans: 0 },
      { q: "¿Cuánto es 3/4 − 1/2?", opts: ["2/2","1/4","1/2","3/8"], ans: 1 },
      { q: "¿Cuánto es el 75% de 80?", opts: ["60","75","40","56"], ans: 0 },
      { q: "En la tienda hay razón de 3 naranjas por cada 2 manzanas. Si hay 12 naranjas, ¿cuántas manzanas hay?", opts: ["6","8","18","4"], ans: 1 },
      { q: "Expresa 2 y 2/3 como fracción impropia.", opts: ["4/3","6/3","8/3","7/3"], ans: 2 },
    ]
  },

  algebra: {
    title: "📐 Álgebra y Ecuaciones",
    practice: [
      { q: "En una tabla de valores: x=1→y=3, x=2→y=6, x=3→y=9. ¿Cuál es el patrón?", type: "mc", opts: ["y = x + 2","y = x × 3","y = x + 3","y = 2x"], ans: 1, hint: "Observa cuánto vale y para cada x. ¿Qué operación conecta los valores?", exp: "y = x × 3. Para x=1: 1×3=3 ✓ Para x=2: 2×3=6 ✓ (OA 9)" },
      { q: "Usando la regla y = x × 4, ¿cuánto vale y cuando x = 7?", type: "input", ans: "28", hint: "Reemplaza x=7 en la fórmula.", exp: "y = 7 × 4 = 28. (OA 9)" },
      { q: "Resuelve la ecuación: x + 5 = 12", type: "mc", opts: ["x=17","x=7","x=5","x=6"], ans: 1, hint: "Resta 5 de ambos lados de la ecuación.", exp: "x = 12 − 5 = 7. (OA 11)" },
      { q: "Resuelve: 3 × x = 24", type: "input", ans: "8", hint: "Divide ambos lados entre 3.", exp: "x = 24 ÷ 3 = 8. (OA 11)" },
      { q: "En una tabla: x=2→y=5, x=4→y=9, x=6→y=13. ¿Qué regla describe el patrón?", type: "mc", opts: ["y = 2x","y = 2x + 1","y = x + 3","y = 3x − 1"], ans: 1, hint: "Prueba la regla con los valores de la tabla.", exp: "y = 2x + 1. Para x=2: 2×2+1=5 ✓ Para x=4: 2×4+1=9 ✓ (OA 9)" },
      { q: "Resuelve: x − 8 = 15", type: "mc", opts: ["x=7","x=23","x=13","x=20"], ans: 1, hint: "Suma 8 a ambos lados de la ecuación.", exp: "x = 15 + 8 = 23. (OA 11)" },
      { q: "¿Qué valor de x hace verdadera la ecuación 2x + 3 = 11?", type: "input", ans: "4", hint: "Primero resta 3 a ambos lados, luego divide entre 2.", exp: "2x=8 → x=4. Comprueba: 2×4+3=11 ✓ (OA 11)" },
      { q: "Escribe en lenguaje matemático: 'El doble de un número más 7 es igual a 19'.", type: "mc", opts: ["n + 7 = 19","2n + 7 = 19","2n = 19 + 7","n × 7 = 19"], ans: 1, hint: "El doble de un número es 2×n.", exp: "El doble = 2n. Más 7 = 2n+7. Es igual a 19 = 2n+7=19. (OA 10)" },
    ],
    quiz: [
      { q: "Tabla: x=1→y=4, x=2→y=8, x=3→y=12. ¿Cuál es la regla?", opts: ["y=x+3","y=4x","y=3x+1","y=2x+2"], ans: 1 },
      { q: "Resuelve: x + 9 = 20", opts: ["x=29","x=11","x=9","x=13"], ans: 1 },
      { q: "Resuelve: 5x = 45", opts: ["x=40","x=50","x=9","x=5"], ans: 2 },
      { q: "¿Qué expresión representa 'tres veces un número menos 4'?", opts: ["3 + n − 4","3n − 4","3n + 4","n − 4 × 3"], ans: 1 },
      { q: "Resuelve: x ÷ 3 = 7", opts: ["x=21","x=10","x=4","x=3"], ans: 0 },
      { q: "Usando y = 5x − 2, ¿cuánto vale y cuando x=3?", opts: ["13","17","12","15"], ans: 0 },
    ]
  },

  basicfracciones: {
    title: "½ Operaciones Básicas con Fracciones",
    practice: [
      { q: "Luis comió 2/6 de una torta y Pedro comió 1/6. ¿Qué fracción comieron en total?", type: "mc", opts: ["3/12","3/6","2/6","1/2"], ans: 1, hint: "Tienen el mismo denominador. Solo suma los numeradores.", exp: "2/6 + 1/6 = 3/6 = 1/2. (OA 6)" },
      { q: "Ana tiene 4/5 de litro de jugo y bebe 2/5. ¿Cuánto le queda?", type: "mc", opts: ["2/10","6/5","2/5","2/0"], ans: 2, hint: "Mismo denominador: resta los numeradores.", exp: "4/5 − 2/5 = 2/5. (OA 6)" },
      { q: "Suma: 1/3 + 1/4 = ?", type: "mc", opts: ["2/7","7/12","2/12","4/12"], ans: 1, hint: "MCM(3,4)=12. Convierte ambas fracciones.", exp: "1/3=4/12. 1/4=3/12. 4/12+3/12=7/12. (OA 6)" },
      { q: "Resta: 3/4 − 1/6 = ?", type: "mc", opts: ["2/2","7/12","1/3","2/10"], ans: 1, hint: "MCM(4,6)=12. Convierte: 3/4=9/12 y 1/6=2/12.", exp: "9/12 − 2/12 = 7/12. (OA 6)" },
      { q: "En una pizzería, 3/8 de las pizzas son de queso y 2/8 son de pepperoni. ¿Qué fracción corresponde a esas dos variedades?", type: "input", ans: "5/8", hint: "Suma las fracciones con el mismo denominador.", exp: "3/8 + 2/8 = 5/8. (OA 6)" },
      { q: "Javiera recorrió 5/6 de km y luego 1/3 de km más. ¿Cuánto recorrió en total?", type: "mc", opts: ["6/9","7/6","1 y 1/6","6/6"], ans: 2, hint: "MCM(6,3)=6. Convierte 1/3=2/6. Luego suma.", exp: "5/6+2/6=7/6=1y1/6 km. (OA 8)" },
      { q: "¿Cuánto es 1/2 + 1/3 + 1/6?", type: "mc", opts: ["3/11","1","5/6","4/6"], ans: 1, hint: "MCM(2,3,6)=6. Convierte todas las fracciones.", exp: "3/6+2/6+1/6=6/6=1. (OA 6)" },
      { q: "Resta: 2 y 3/4 − 1 y 1/2 = ?", type: "mc", opts: ["1 y 1/4","1 y 1/2","1 y 3/4","1/4"], ans: 0, hint: "Convierte 1/2 a cuartos: 2/4. Resta parte entera y parte fraccionaria por separado.", exp: "3/4−2/4=1/4. 2−1=1. Resultado: 1y1/4. (OA 6)" },
    ],
    quiz: [
      { q: "¿Cuánto es 2/7 + 3/7?", opts: ["5/14","6/7","5/7","1/7"], ans: 2 },
      { q: "¿Cuánto es 5/8 − 3/8?", opts: ["2/0","1/4","2/8","1/2"], ans: 1 },
      { q: "¿Cuánto es 1/2 + 1/4?", opts: ["2/8","2/6","3/4","1/3"], ans: 2 },
      { q: "¿Cuánto es 5/6 − 1/3?", opts: ["4/3","1/2","1/6","3/6"], ans: 1 },
      { q: "María tiene 1 y 1/2 metros de tela. Usa 3/4. ¿Cuánto le queda?", opts: ["3/4","1/2","1 y 1/4","1/4"], ans: 0 },
      { q: "¿Cuánto es 2/3 + 1/6?", opts: ["3/9","1/2","5/6","3/6"], ans: 2 },
    ]
  },

  decimales: {
    title: "0.5 Operaciones Básicas con Decimales",
    practice: [
      { q: "Una hormiga mide 0,4 cm. Al verla en el microscopio se amplía al triple. ¿Cuánto mide ampliada?", type: "mc", opts: ["1,4 cm","0,12 cm","1,2 cm","0,43 cm"], ans: 2, hint: "Multiplica 0,4 × 3. Primero calcula 4×3 y luego ubica el punto decimal.", exp: "4×3=12, un decimal → 1,2 cm. (OA 7)" },
      { q: "Sofía caminó 2,5 km el lunes y 1,35 km el martes. ¿Cuánto caminó en total?", type: "input", ans: "3,85", hint: "Alinea los puntos decimales: 2,50 + 1,35.", exp: "2,50 + 1,35 = 3,85 km. (OA 8)" },
      { q: "Un libro cuesta $8 750. Carlos tiene $12 000. ¿Cuánto le sobra?", type: "mc", opts: ["$3 250","$2 750","$4 250","$3 750"], ans: 0, hint: "Resta el precio del libro al dinero de Carlos.", exp: "$12 000 − $8 750 = $3 250. (OA 2)" },
      { q: "¿Cuánto es 3,5 × 4?", type: "mc", opts: ["12","14","1,4","140"], ans: 1, hint: "35 × 4 = 140. Luego ubica un decimal.", exp: "35×4=140, un decimal → 14,0 = 14. (OA 7)" },
      { q: "Divide: 6,4 ÷ 8 = ?", type: "mc", opts: ["0,8","8","0,08","80"], ans: 0, hint: "64 ÷ 8 = 8. Luego ubica un decimal.", exp: "64÷8=8, un decimal → 0,8. (OA 7)" },
      { q: "Una cuerda de 4,5 m se divide en 9 partes iguales. ¿Cuánto mide cada parte?", type: "input", ans: "0,5", hint: "Divide 4,5 ÷ 9. Primero 45÷9=5, luego ubica el decimal.", exp: "45÷9=5, un decimal → 0,5 m. (OA 7)" },
      { q: "¿Cuánto es 1,8 ÷ 10?", type: "mc", opts: ["18","0,18","0,018","180"], ans: 1, hint: "Al dividir por 10, el punto decimal se corre un lugar a la izquierda.", exp: "1,8 ÷ 10 = 0,18. (OA 7)" },
      { q: "Juana gastó $3 250,50 en el supermercado y $1 499,50 en la farmacia. ¿Cuánto gastó en total?", type: "input", ans: "4750", hint: "Suma los dos valores alineando los decimales.", exp: "$3 250,50 + $1 499,50 = $4 750,00. (OA 8)" },
    ],
    quiz: [
      { q: "¿Cuánto es 0,3 × 7?", opts: ["21","0,21","2,1","210"], ans: 2 },
      { q: "¿Cuánto es 5,6 ÷ 8?", opts: ["7","0,07","0,7","70"], ans: 2 },
      { q: "Una botella tiene 1,5 litros. Se usan 0,75 litros. ¿Cuánto queda?", opts: ["0,25 L","0,75 L","1,25 L","0,5 L"], ans: 1 },
      { q: "¿Cuánto es 2,4 × 10?", opts: ["0,24","240","24","2,40"], ans: 2 },
      { q: "¿Cuánto es 0,9 ÷ 100?", opts: ["90","0,009","0,09","9"], ans: 1 },
      { q: "Un atleta corre 400m en 48,5 segundos. Otro lo hace en 51,3 segundos. ¿Cuántos segundos de diferencia hay?", opts: ["2,8 s","3,2 s","2,2 s","3,8 s"], ans: 0 },
    ]
  },

  graficos: {
    title: "📊 Representación y Análisis de Gráficos",
    practice: [
      { q: "Un gráfico de barras muestra los libros leídos: Ana=8, Luis=5, Sara=10, Pedro=7. ¿Quién leyó más libros?", type: "mc", opts: ["Ana","Luis","Sara","Pedro"], ans: 2, hint: "Busca el valor más alto en el gráfico.", exp: "Sara tiene el valor más alto: 10 libros. (OA 24)" },
      { q: "En el mismo gráfico, ¿cuántos libros leyeron Ana y Pedro juntos?", type: "input", ans: "15", hint: "Suma los valores de Ana y Pedro.", exp: "8 + 7 = 15 libros. (OA 24)" },
      { q: "Un gráfico circular muestra deportes favoritos: Fútbol 50%, Básquetbol 30%, Tenis 20%. Si hay 200 alumnos, ¿cuántos prefieren básquetbol?", type: "mc", opts: ["50","60","100","30"], ans: 1, hint: "Calcula el 30% de 200.", exp: "30% de 200 = 200×30÷100 = 60 alumnos. (OA 24)" },
      { q: "Un gráfico de doble barra muestra: En 5°A hay 15 niñas y 12 niños; en 5°B hay 13 niñas y 14 niños. ¿En qué curso hay más alumnos?", type: "mc", opts: ["5°A","5°B","Son iguales","No se puede saber"], ans: 0, hint: "Suma el total de cada curso y compara.", exp: "5°A: 15+12=27. 5°B: 13+14=27. ¡Son iguales! (OA 24)" },
      { q: "El gráfico de tallo y hojas muestra edades: Tallo 1 | hojas 2,5,8 y Tallo 2 | hojas 0,3. ¿Cuál es la edad mayor?", type: "mc", opts: ["18","23","25","12"], ans: 1, hint: "El tallo es la decena y la hoja es la unidad.", exp: "Tallo 2, hoja 3 → 23 años. (OA 22)" },
      { q: "En un gráfico circular de presupuesto familiar: Alimentación 40%, Arriendo 35%, Transporte 15%, Otros 10%. ¿Qué fracción representa el Arriendo?", type: "mc", opts: ["7/20","1/3","35/10","1/4"], ans: 0, hint: "Expresa 35% como fracción: 35/100. Simplifica.", exp: "35/100 = 7/20. (OA 24)" },
      { q: "Diagrama de puntos de temperaturas (°C): 18,18,19,20,20,20,21,22. ¿Cuántos días tuvieron exactamente 20°C?", type: "input", ans: "3", hint: "Cuenta los puntos que están sobre el valor 20.", exp: "Hay 3 puntos sobre el valor 20. (OA 22)" },
      { q: "Gráfico de barras doble: Manzanas vendidas — Semana 1: Local A=45, Local B=30. Semana 2: Local A=35, Local B=50. ¿En cuál semana se vendió más en total?", type: "mc", opts: ["Semana 1","Semana 2","Igual en ambas","No se puede comparar"], ans: 2, hint: "Suma los totales de cada semana y compara.", exp: "Semana 1: 45+30=75. Semana 2: 35+50=85. ¡Semana 2 vendió más! Opción correcta: Semana 2. (OA 24)" },
    ],
    quiz: [
      { q: "¿Qué tipo de gráfico permite comparar dos grupos en las mismas categorías?", opts: ["Circular","Barras doble","De puntos","Tallo y hojas"], ans: 1 },
      { q: "Un gráfico circular tiene sectores: 50%, 30% y 20%. Si hay 60 personas, ¿cuántas están en el sector del 20%?", opts: ["20","12","10","6"], ans: 1 },
      { q: "Diagrama de tallo y hojas — Tallo 3 | hojas 2,5,9. ¿Qué valor es el mayor?", opts: ["32","35","39","93"], ans: 2 },
      { q: "Gráfico de barras: Lunes=25, Martes=30, Miércoles=20. ¿Cuál es el promedio diario?", opts: ["25","28","30","75"], ans: 0 },
      { q: "En un gráfico circular, un sector representa 1/4 del total. ¿A qué porcentaje equivale?", opts: ["20%","40%","25%","50%"], ans: 2 },
      { q: "¿Para qué sirve principalmente un diagrama de puntos?", opts: ["Comparar dos grupos","Mostrar partes de un todo","Ver la distribución de datos","Mostrar cambios en el tiempo"], ans: 2 },
    ]
  },

  probabilidades: {
    title: "🎲 Probabilidades y Azar",
    practice: [
      { q: "Al lanzar una moneda al aire, ¿cuáles son los resultados posibles?", type: "mc", opts: ["Solo cara","Solo sello","Cara o sello","Cara, sello y canto"], ans: 2, hint: "Una moneda tiene dos caras: cara y sello.", exp: "Los resultados posibles son cara o sello. (OA 23)" },
      { q: "Al lanzar un dado de 6 caras, ¿cuántos resultados posibles hay?", type: "mc", opts: ["3","4","6","12"], ans: 2, hint: "Un dado tiene números del 1 al 6.", exp: "Hay 6 resultados posibles: 1, 2, 3, 4, 5 y 6. (OA 23)" },
      { q: "Al lanzar un dado, ¿cuántos resultados favorables hay para obtener un número par?", type: "mc", opts: ["1","2","3","4"], ans: 2, hint: "Los números pares entre 1 y 6 son: 2, 4 y 6.", exp: "Los resultados favorables son 2, 4 y 6. Son 3 casos. (OA 23)" },
      { q: "Se lanza una moneda 100 veces. Si la tendencia es equiprobable, ¿aproximadamente cuántas veces saldrá cara?", type: "mc", opts: ["25 veces","100 veces","50 veces","10 veces"], ans: 2, hint: "Cara y sello tienen la misma posibilidad. ¿Qué fracción es 1 de 2?", exp: "La probabilidad de cara es 1/2. En 100 lanzamientos: 100×1/2 = 50 veces aproximadamente. (OA 23)" },
      { q: "Al lanzar un dado, ¿qué fracción representa la probabilidad de obtener el número 3?", type: "mc", opts: ["1/3","1/6","3/6","3/1"], ans: 1, hint: "Hay 1 resultado favorable (el 3) de 6 posibles.", exp: "Probabilidad = casos favorables / casos totales = 1/6. (OA 23)" },
      { q: "Se lanza un dado 60 veces. ¿Cuántas veces se espera obtener un número impar?", type: "input", ans: "30", hint: "Los impares son 1, 3 y 5 → 3 de 6 casos. Eso es 1/2 del total.", exp: "P(impar) = 3/6 = 1/2. En 60 lanzamientos: 60×1/2 = 30 veces. (OA 23)" },
      { q: "Al lanzar dos monedas al mismo tiempo, ¿cuáles son los resultados posibles?", type: "mc", opts: ["2 resultados","3 resultados","4 resultados","6 resultados"], ans: 2, hint: "Usa un diagrama de árbol: primera moneda (C/S) × segunda moneda (C/S).", exp: "Los resultados son: CC, CS, SC, SS → 4 resultados posibles. (OA 23)" },
      { q: "En una bolsa hay 3 canicas rojas y 2 azules. Si sacas una sin mirar, ¿qué fracción representa la probabilidad de sacar una roja?", type: "mc", opts: ["2/5","3/2","3/5","1/3"], ans: 2, hint: "Probabilidad = rojas / total de canicas.", exp: "Total = 5 canicas. P(roja) = 3/5. (OA 23)" },
    ],
    quiz: [
      { q: "Al lanzar una moneda, ¿qué fracción representa la probabilidad de que salga sello?", opts: ["1/4","2/3","1/2","1/3"], ans: 2 },
      { q: "Al lanzar un dado, ¿cuál es la probabilidad de sacar un número mayor que 4?", opts: ["1/6","2/6","3/6","4/6"], ans: 1 },
      { q: "Se lanza una moneda 200 veces. ¿Cuántas veces se espera que salga cara?", opts: ["50","200","100","150"], ans: 2 },
      { q: "En una bolsa hay 2 bolas verdes y 8 amarillas. ¿Cuál es la probabilidad de sacar una verde?", opts: ["2/8","1/5","8/10","1/8"], ans: 1 },
      { q: "Al lanzar dos monedas, ¿cuál es la probabilidad de que ambas salgan cara?", opts: ["1/2","2/4","1/4","2/2"], ans: 2 },
      { q: "Al lanzar un dado 30 veces, ¿cuántas veces se espera obtener el número 6?", opts: ["6","5","10","3"], ans: 1 },
    ]
  },

  geometria: {
    title: "📐 Geometría: Ángulos y Figuras 3D",
    practice: [
      { q: "Un triángulo tiene ángulos de 60° y 80°. ¿Cuánto mide el tercer ángulo?", type: "mc", opts: ["20°","50°","40°","60°"], ans: 2, hint: "La suma de los ángulos interiores de un triángulo es siempre 180°.", exp: "180° − 60° − 80° = 40°. (OA 17)" },
      { q: "¿Cómo se llama el triángulo que tiene sus tres lados iguales?", type: "mc", opts: ["Escaleno","Isósceles","Equilátero","Rectángulo"], ans: 2, hint: "Piensa en el prefijo 'equi-' que significa igual.", exp: "El triángulo equilátero tiene sus tres lados y sus tres ángulos iguales (60° cada uno). (OA 12)" },
      { q: "Un cuadrilátero tiene tres ángulos: 90°, 90° y 70°. ¿Cuánto mide el cuarto ángulo?", type: "input", ans: "110", hint: "La suma de los ángulos interiores de un cuadrilátero es 360°.", exp: "360° − 90° − 90° − 70° = 110°. (OA 17)" },
      { q: "¿Qué tipo de ángulo mide entre 0° y 90°?", type: "mc", opts: ["Obtuso","Recto","Agudo","Extendido"], ans: 2, hint: "Los ángulos se clasifican según si son menores, iguales o mayores que 90°.", exp: "Un ángulo agudo mide entre 0° y 90°. (OA 15)" },
      { q: "Una caja de regalo tiene forma de paralelepípedo. Mide 10 cm de largo, 6 cm de ancho y 4 cm de alto. ¿Cuánto es su volumen?", type: "mc", opts: ["240 cm³","160 cm³","200 cm³","120 cm³"], ans: 0, hint: "Volumen del paralelepípedo = largo × ancho × alto.", exp: "V = 10 × 6 × 4 = 240 cm³. (OA 19)" },
      { q: "Un cubo tiene aristas de 5 cm. ¿Cuánto mide su volumen?", type: "mc", opts: ["15 cm³","25 cm³","125 cm³","150 cm³"], ans: 2, hint: "Volumen del cubo = arista × arista × arista = arista³.", exp: "V = 5 × 5 × 5 = 125 cm³. (OA 19)" },
      { q: "Dos rectas se cortan. Si uno de los ángulos que se forman mide 65°, ¿cuánto mide el ángulo opuesto por el vértice?", type: "mc", opts: ["115°","25°","65°","180°"], ans: 2, hint: "Los ángulos opuestos por el vértice siempre tienen la misma medida.", exp: "Los ángulos opuestos por el vértice son iguales → 65°. (OA 16)" },
      { q: "Se necesita envolver una caja con forma de paralelepípedo de 8 cm × 5 cm × 3 cm. ¿Cuántos cm² de papel se necesitan como mínimo?", type: "mc", opts: ["158 cm²","120 cm²","79 cm²","200 cm²"], ans: 0, hint: "Superficie total = 2×(largo×ancho) + 2×(largo×alto) + 2×(ancho×alto).", exp: "2×(8×5) + 2×(8×3) + 2×(5×3) = 80+48+30 = 158 cm². (OA 18)" },
    ],
    quiz: [
      { q: "¿Cuánto es la suma de los ángulos interiores de un triángulo?", opts: ["90°","270°","360°","180°"], ans: 3 },
      { q: "Un triángulo tiene ángulos de 45° y 45°. ¿Cuánto mide el tercer ángulo?", opts: ["45°","90°","100°","180°"], ans: 1 },
      { q: "Un cubo tiene arista de 3 cm. ¿Cuánto mide su volumen?", opts: ["9 cm³","18 cm³","27 cm³","6 cm³"], ans: 2 },
      { q: "¿Cómo se llama el triángulo que tiene exactamente dos lados iguales?", opts: ["Equilátero","Escaleno","Rectángulo","Isósceles"], ans: 3 },
      { q: "Dos rectas paralelas son cortadas por una transversal. Los ángulos alternos internos son...", opts: ["Suplementarios","Iguales","Complementarios","Opuestos"], ans: 1 },
      { q: "Un paralelepípedo mide 4 m × 3 m × 2 m. ¿Cuál es su volumen?", opts: ["18 m³","24 m³","9 m³","12 m³"], ans: 1 },
    ]
  }
};

// =====================
// NAVIGATION
// =====================
function showScreen(id) {
  document.querySelectorAll('.screen').forEach(s => s.classList.remove('active'));
  document.getElementById('screen-' + id).classList.add('active');
}

function goHome() {
  showScreen('home');
  currentModule = null;
}

function openModule(mod) {
  currentModule = mod;
  const data = modules[mod];
  document.getElementById('lesson-title').textContent = data.title;
  // reset practice
  practiceIdx = 0;
  practiceAnswered = new Array(data.practice.length).fill(null);
  renderPractice();
  // reset quiz
  quizIdx = 0;
  quizScore = 0;
  quizWrong = 0;
  quizAnswered = new Array(data.quiz.length).fill(null);
  renderQuizQuestion();
  // show practice tab
  switchTab('practice');
  showScreen('lesson');
}

function switchTab(tab) {
  document.querySelectorAll('.tab').forEach((t,i) => {
    const tabs = ['practice','quiz'];
    t.classList.toggle('active', tabs[i] === tab);
  });
  document.querySelectorAll('.tab-content').forEach(tc => tc.classList.remove('active'));
  document.getElementById('tab-' + tab).classList.add('active');
}

// =====================
// PRACTICE
// =====================
function renderPractice() {
  const data = modules[currentModule].practice;
  const ex = data[practiceIdx];
  const total = data.length;

  // Progress
  const pct = (practiceAnswered.filter(a=>a!==null).length / total) * 100;
  document.getElementById('practice-progress').style.width = pct + '%';

  // Dots
  let dots = '';
  for (let i = 0; i < total; i++) {
    let cls = 'dot';
    if (i === practiceIdx) cls += ' active';
    else if (practiceAnswered[i] === true) cls += ' done';
    else if (practiceAnswered[i] === false) cls += ' wrong-dot';
    dots += `<div class="${cls}"></div>`;
  }
  document.getElementById('practice-dots').innerHTML = dots;

  let diffClass = practiceIdx < 2 ? 'diff-easy' : practiceIdx < 4 ? 'diff-medium' : 'diff-hard';
  let diffLabel = practiceIdx < 2 ? 'Básico' : practiceIdx < 4 ? 'Intermedio' : 'Avanzado';

  let answerArea = '';
  if (ex.type === 'mc') {
    answerArea = `<div class="options-grid">` +
      ex.opts.map((o, i) => `<button class="option-btn" id="opt-${i}" onclick="checkMC(${i})">${o}</button>`).join('') +
    `</div>`;
  } else {
    answerArea = `
      <div class="input-group">
        <input class="math-input" id="math-input" type="text" placeholder="Escribe tu respuesta..." onkeydown="if(event.key==='Enter') checkInput()">
        <button class="btn btn-primary" onclick="checkInput()">Verificar</button>
      </div>`;
  }

  document.getElementById('practice-content').innerHTML = `
    <div class="exercise-card">
      <div class="ex-meta">
        <span>Ejercicio ${practiceIdx+1} de ${total}</span>
        <span class="difficulty ${diffClass}">${diffLabel}</span>
      </div>
      <div class="ex-question">${ex.q}</div>
      ${answerArea}
      <div class="feedback-box" id="feedback"></div>
      <div style="display:flex; gap:10px; align-items:center; flex-wrap:wrap;">
        <button class="hint-btn" onclick="showHint()">💡 Pista</button>
        <div class="hint-box" id="hint-box">${ex.hint}</div>
      </div>
    </div>
    <div style="display:flex; gap:10px; justify-content:flex-end; margin-top:10px;">
      <button class="btn btn-secondary" onclick="prevExercise()" ${practiceIdx===0?'disabled':''}>← Anterior</button>
      <button class="btn btn-primary" id="next-btn" style="display:none" onclick="nextExercise()">Siguiente →</button>
    </div>
  `;

  // if already answered
  if (practiceAnswered[practiceIdx] !== null) {
    showPracticeFeedback(ex, practiceAnswered[practiceIdx]);
  }
}

function showHint() {
  const box = document.getElementById('hint-box');
  box.classList.toggle('show');
}

function checkMC(chosen) {
  const ex = modules[currentModule].practice[practiceIdx];
  const correct = chosen === ex.ans;
  document.querySelectorAll('.option-btn').forEach((b, i) => {
    b.disabled = true;
    if (i === ex.ans) b.classList.add('correct');
    else if (i === chosen && !correct) b.classList.add('wrong');
  });
  practiceAnswered[practiceIdx] = correct;
  updateScore(correct);
  showPracticeFeedback(ex, correct);
  updateDots();
}

function checkInput() {
  const ex = modules[currentModule].practice[practiceIdx];
  const inp = document.getElementById('math-input');
  const val = inp.value.trim().replace(/\s/g,'');
  const correct = val.toLowerCase() === String(ex.ans).toLowerCase();
  inp.classList.add(correct ? 'correct' : 'wrong');
  inp.disabled = true;
  practiceAnswered[practiceIdx] = correct;
  updateScore(correct);
  showPracticeFeedback(ex, correct);
  updateDots();
}

function showPracticeFeedback(ex, correct) {
  const fb = document.getElementById('feedback');
  fb.className = 'feedback-box show ' + (correct ? 'correct' : 'wrong');
  fb.innerHTML = correct
    ? `✓ ¡Correcto! — ${ex.exp}`
    : `✗ Incorrecto. ${ex.exp}`;
  const nb = document.getElementById('next-btn');
  if (nb) nb.style.display = 'inline-flex';
  const pr = modules[currentModule].practice.length;
  document.getElementById('practice-progress').style.width =
    (practiceAnswered.filter(a=>a!==null).length / pr * 100) + '%';
}

function updateDots() {
  const data = modules[currentModule].practice;
  const total = data.length;
  const dotsEl = document.getElementById('practice-dots');
  let dots = '';
  for (let i = 0; i < total; i++) {
    let cls = 'dot';
    if (i === practiceIdx) cls += ' active';
    else if (practiceAnswered[i] === true) cls += ' done';
    else if (practiceAnswered[i] === false) cls += ' wrong-dot';
    dots += `<div class="${cls}"></div>`;
  }
  dotsEl.innerHTML = dots;
}

function nextExercise() {
  const total = modules[currentModule].practice.length;
  if (practiceIdx < total - 1) {
    practiceIdx++;
    renderPractice();
  } else {
    // all done
    const correct = practiceAnswered.filter(a=>a===true).length;
    document.getElementById('practice-content').innerHTML = `
      <div class="results-card" style="margin:0 auto;">
        <div class="score-display">${correct}/${total}</div>
        <div class="score-label">ejercicios correctos</div>
        <div class="results-breakdown">
          <div class="res-item"><div class="res-num good">${correct}</div><div class="res-label">correctas</div></div>
          <div class="res-item"><div class="res-num bad">${total-correct}</div><div class="res-label">incorrectas</div></div>
        </div>
        <p style="font-family:'JetBrains Mono',monospace;font-size:0.82rem;color:var(--text-muted);margin-bottom:20px;">
          ${correct===total ? '¡Perfecto! Prueba el Quiz ahora.' : correct >= total/2 ? '¡Buen trabajo! Revisa la teoría y vuelve a practicar.' : 'Repasa la teoría e inténtalo de nuevo.'}
        </p>
        <div style="display:flex;gap:10px;justify-content:center;flex-wrap:wrap;">
          <button class="btn btn-secondary" onclick="practiceIdx=0;practiceAnswered=new Array(modules[currentModule].practice.length).fill(null);renderPractice()">Reintentar</button>
          <button class="btn btn-primary" onclick="switchTab('quiz')">Ir al Quiz →</button>
        </div>
      </div>
    `;
    document.getElementById('practice-dots').innerHTML = '';
  }
}

function prevExercise() {
  if (practiceIdx > 0) { practiceIdx--; renderPractice(); }
}

// =====================
// SCORE & STREAK
// =====================
function updateScore(correct) {
  if (correct) {
    streak++;
    const bonus = streak >= 3 ? 20 : 10;
    totalScore += bonus;
  } else {
    streak = 0;
  }
  document.getElementById('total-score').textContent = totalScore;
  document.getElementById('streak').textContent = '🔥 ' + streak;
}

// =====================
// QUIZ
// =====================
function renderQuizQuestion() {
  const data = modules[currentModule]?.quiz;
  if (!data) return;

  if (quizIdx >= data.length) {
    renderQuizResults();
    return;
  }

  const q = data[quizIdx];
  const total = data.length;
  const pct = (quizIdx / total) * 100;

  document.getElementById('quiz-content').innerHTML = `
    <div class="quiz-header">
      <span>Pregunta ${quizIdx+1} de ${total}</span>
      <span>✓ ${quizScore} | ✗ ${quizWrong}</span>
    </div>
    <div class="progress-wrap"><div class="progress-fill" style="width:${pct}%"></div></div>
    <div class="exercise-card">
      <div class="ex-question" style="font-size:1.4rem;">${q.q}</div>
      <div class="options-grid">
        ${q.opts.map((o,i) => `<button class="option-btn" id="qopt-${i}" onclick="answerQuiz(${i})">${o}</button>`).join('')}
      </div>
      <div class="feedback-box" id="quiz-feedback"></div>
    </div>
  `;
}

function answerQuiz(chosen) {
  const data = modules[currentModule].quiz;
  const q = data[quizIdx];
  const correct = chosen === q.ans;

  document.querySelectorAll('.option-btn').forEach((b,i) => {
    b.disabled = true;
    if (i === q.ans) b.classList.add('correct');
    else if (i === chosen && !correct) b.classList.add('wrong');
  });

  quizAnswered[quizIdx] = correct;
  if (correct) { quizScore++; updateScore(true); if(quizScore%3===0) celebrate(); }
  else { quizWrong++; updateScore(false); }

  const fb = document.getElementById('quiz-feedback');
  fb.className = 'feedback-box show ' + (correct ? 'correct' : 'wrong');
  fb.innerHTML = (correct ? '✓ ¡Correcto!' : '✗ Incorrecto.') + ' La respuesta es: ' + q.opts[q.ans];

  setTimeout(() => {
    quizIdx++;
    renderQuizQuestion();
  }, 1600);
}

function renderQuizResults() {
  const total = modules[currentModule].quiz.length;
  const pct = Math.round((quizScore / total) * 100);
  let msg = pct === 100 ? '¡Perfecto! Eres un maestro.' : pct >= 70 ? '¡Muy bien! Sigue practicando.' : 'Revisa la teoría y vuélvelo a intentar.';
  if (pct === 100) celebrate();

  document.getElementById('quiz-content').innerHTML = `
    <div class="results-card">
      <div class="score-display">${pct}%</div>
      <div class="score-label">de respuestas correctas</div>
      <div class="results-breakdown">
        <div class="res-item"><div class="res-num good">${quizScore}</div><div class="res-label">correctas</div></div>
        <div class="res-item"><div class="res-num bad">${quizWrong}</div><div class="res-label">incorrectas</div></div>
      </div>
      <p style="font-family:'JetBrains Mono',monospace;font-size:0.82rem;color:var(--text-muted);margin-bottom:24px;">${msg}</p>
      <div style="display:flex;gap:10px;justify-content:center;flex-wrap:wrap;">
        <button class="btn btn-secondary" onclick="quizIdx=0;quizScore=0;quizWrong=0;quizAnswered=new Array(modules[currentModule].quiz.length).fill(null);renderQuizQuestion()">Reintentar</button>
        <button class="btn btn-primary" onclick="goHome()">Otros módulos →</button>
      </div>
    </div>
  `;
}

// =====================
// CELEBRATE
// =====================
function celebrate() {
  const colors = ['#6c63ff','#ff6584','#43e97b','#f7971e','#fff'];
  for (let i = 0; i < 30; i++) {
    const el = document.createElement('div');
    el.className = 'confetti-piece';
    el.style.left = Math.random() * 100 + 'vw';
    el.style.top = '-10px';
    el.style.background = colors[Math.floor(Math.random()*colors.length)];
    el.style.animationDelay = Math.random() * 0.5 + 's';
    el.style.animationDuration = (1.5 + Math.random()) + 's';
    document.body.appendChild(el);
    setTimeout(() => el.remove(), 2500);
  }
}
</script>
</body>
</html>
