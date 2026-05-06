<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Protocolo 12 Semanas — O Caminho para o Positivo</title>
<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,300;0,400;0,500;0,600;1,300;1,400&family=DM+Sans:wght@300;400;500&display=swap" rel="stylesheet">
<style>
  *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

  :root {
    --cream: #FAF6F1;
    --warm: #F2EAE0;
    --blush: #E8C9B8;
    --rose: #C4826A;
    --deep: #6B3D2E;
    --text: #2D1F1A;
    --muted: #8B6E65;
    --white: #FFFFFF;
  }

  html { scroll-behavior: smooth; }

  body {
    font-family: 'DM Sans', sans-serif;
    background: var(--cream);
    color: var(--text);
    overflow-x: hidden;
  }

  /* ── HERO ── */
  .hero {
    min-height: 100vh;
    background: linear-gradient(160deg, #2D1F1A 0%, #6B3D2E 50%, #C4826A 100%);
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    text-align: center;
    padding: 60px 24px;
    position: relative;
    overflow: hidden;
  }

  .hero::before {
    content: '';
    position: absolute;
    inset: 0;
    background: radial-gradient(ellipse at 60% 30%, rgba(232,201,184,0.18) 0%, transparent 65%);
  }

  .hero-badge {
    font-family: 'DM Sans', sans-serif;
    font-size: 11px;
    font-weight: 500;
    letter-spacing: 3px;
    text-transform: uppercase;
    color: var(--blush);
    border: 1px solid rgba(232,201,184,0.4);
    padding: 8px 20px;
    border-radius: 100px;
    margin-bottom: 36px;
    animation: fadeUp 0.8s ease both;
  }

  .hero h1 {
    font-family: 'Cormorant Garamond', serif;
    font-size: clamp(48px, 9vw, 88px);
    font-weight: 300;
    color: var(--white);
    line-height: 1.05;
    letter-spacing: -1px;
    margin-bottom: 12px;
    animation: fadeUp 0.9s ease 0.1s both;
  }

  .hero h1 em {
    font-style: italic;
    color: var(--blush);
  }

  .hero-sub {
    font-family: 'Cormorant Garamond', serif;
    font-size: clamp(18px, 3vw, 24px);
    font-weight: 300;
    font-style: italic;
    color: rgba(255,255,255,0.7);
    margin-bottom: 48px;
    animation: fadeUp 1s ease 0.2s both;
  }

  .hero-desc {
    max-width: 520px;
    font-size: 16px;
    line-height: 1.7;
    color: rgba(255,255,255,0.75);
    margin-bottom: 52px;
    animation: fadeUp 1s ease 0.3s both;
  }

  .btn-primary {
    display: inline-block;
    background: var(--blush);
    color: var(--deep);
    font-family: 'DM Sans', sans-serif;
    font-size: 15px;
    font-weight: 500;
    letter-spacing: 0.5px;
    padding: 18px 44px;
    border-radius: 100px;
    text-decoration: none;
    border: none;
    cursor: pointer;
    transition: all 0.3s ease;
    animation: fadeUp 1s ease 0.4s both;
  }

  .btn-primary:hover {
    background: var(--white);
    transform: translateY(-2px);
    box-shadow: 0 16px 40px rgba(0,0,0,0.25);
  }

  .hero-tags {
    display: flex;
    gap: 16px;
    margin-top: 40px;
    flex-wrap: wrap;
    justify-content: center;
    animation: fadeUp 1s ease 0.5s both;
  }

  .hero-tags span {
    font-size: 12px;
    letter-spacing: 1.5px;
    text-transform: uppercase;
    color: rgba(255,255,255,0.45);
  }

  .hero-tags span:not(:last-child)::after {
    content: '·';
    margin-left: 16px;
  }

  /* ── DOR ── */
  .section-pain {
    background: var(--white);
    padding: 100px 24px;
  }

  .container {
    max-width: 680px;
    margin: 0 auto;
  }

  .container-wide {
    max-width: 960px;
    margin: 0 auto;
  }

  .eyebrow {
    font-size: 11px;
    font-weight: 500;
    letter-spacing: 3px;
    text-transform: uppercase;
    color: var(--rose);
    margin-bottom: 20px;
    display: block;
  }

  .section-pain .quote-big {
    font-family: 'Cormorant Garamond', serif;
    font-size: clamp(28px, 5vw, 44px);
    font-weight: 300;
    line-height: 1.3;
    color: var(--text);
    margin-bottom: 56px;
  }

  .section-pain .quote-big em {
    font-style: italic;
    color: var(--rose);
  }

  .pain-cards {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: 2px;
    background: var(--warm);
    border-radius: 16px;
    overflow: hidden;
  }

  .pain-card {
    background: var(--white);
    padding: 36px 28px;
    transition: background 0.3s;
  }

  .pain-card:hover { background: var(--cream); }

  .pain-icon {
    font-size: 28px;
    margin-bottom: 16px;
    display: block;
  }

  .pain-card h3 {
    font-family: 'Cormorant Garamond', serif;
    font-size: 20px;
    font-weight: 500;
    margin-bottom: 10px;
    color: var(--text);
  }

  .pain-card p {
    font-size: 14px;
    line-height: 1.6;
    color: var(--muted);
  }

  /* ── MECANISMO ── */
  .section-mechanism {
    background: var(--cream);
    padding: 100px 24px;
  }

  .mechanism-header {
    text-align: center;
    margin-bottom: 72px;
  }

  .mechanism-header h2 {
    font-family: 'Cormorant Garamond', serif;
    font-size: clamp(32px, 5vw, 52px);
    font-weight: 300;
    line-height: 1.2;
    color: var(--text);
    margin-bottom: 20px;
  }

  .mechanism-header p {
    font-size: 16px;
    color: var(--muted);
    max-width: 480px;
    margin: 0 auto;
    line-height: 1.7;
  }

  .big-stat {
    background: linear-gradient(135deg, var(--deep), var(--rose));
    border-radius: 24px;
    padding: 60px 40px;
    text-align: center;
    margin-bottom: 64px;
    position: relative;
    overflow: hidden;
  }

  .big-stat::before {
    content: '';
    position: absolute;
    top: -40%;
    right: -10%;
    width: 300px;
    height: 300px;
    border-radius: 50%;
    background: rgba(255,255,255,0.06);
  }

  .big-stat .number {
    font-family: 'Cormorant Garamond', serif;
    font-size: clamp(72px, 14vw, 120px);
    font-weight: 300;
    color: var(--white);
    line-height: 1;
    display: block;
  }

  .big-stat .number-label {
    font-size: 14px;
    letter-spacing: 2px;
    text-transform: uppercase;
    color: rgba(255,255,255,0.65);
    margin-top: 8px;
    display: block;
  }

  .big-stat .stat-text {
    font-size: 17px;
    color: rgba(255,255,255,0.85);
    line-height: 1.6;
    max-width: 440px;
    margin: 28px auto 0;
  }

  .pillars {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
    gap: 24px;
  }

  .pillar {
    background: var(--white);
    border-radius: 20px;
    padding: 36px 28px;
    border: 1px solid rgba(196,130,106,0.12);
    transition: transform 0.3s, box-shadow 0.3s;
  }

  .pillar:hover {
    transform: translateY(-4px);
    box-shadow: 0 20px 48px rgba(107,61,46,0.1);
  }

  .pillar-num {
    font-family: 'Cormorant Garamond', serif;
    font-size: 13px;
    font-weight: 500;
    letter-spacing: 2px;
    color: var(--rose);
    margin-bottom: 16px;
    display: block;
  }

  .pillar h3 {
    font-family: 'Cormorant Garamond', serif;
    font-size: 22px;
    font-weight: 500;
    margin-bottom: 12px;
    color: var(--text);
  }

  .pillar p {
    font-size: 14px;
    line-height: 1.65;
    color: var(--muted);
  }

  /* ── O QUE ESTÁ DENTRO ── */
  .section-inside {
    background: var(--deep);
    padding: 100px 24px;
  }

  .section-inside .eyebrow { color: var(--blush); }

  .section-inside h2 {
    font-family: 'Cormorant Garamond', serif;
    font-size: clamp(32px, 5vw, 52px);
    font-weight: 300;
    color: var(--white);
    margin-bottom: 16px;
    line-height: 1.2;
  }

  .section-inside .lead {
    font-size: 16px;
    color: rgba(255,255,255,0.6);
    line-height: 1.7;
    max-width: 480px;
    margin-bottom: 60px;
  }

  .inside-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
    gap: 2px;
    border-radius: 20px;
    overflow: hidden;
    background: rgba(255,255,255,0.05);
  }

  .inside-item {
    padding: 32px 28px;
    background: rgba(255,255,255,0.03);
    border: 1px solid rgba(255,255,255,0.05);
    transition: background 0.3s;
  }

  .inside-item:hover { background: rgba(255,255,255,0.07); }

  .inside-item .check {
    width: 32px;
    height: 32px;
    border-radius: 50%;
    background: rgba(196,130,106,0.2);
    display: flex;
    align-items: center;
    justify-content: center;
    margin-bottom: 16px;
    color: var(--blush);
    font-size: 14px;
  }

  .inside-item h4 {
    font-family: 'Cormorant Garamond', serif;
    font-size: 19px;
    font-weight: 500;
    color: var(--white);
    margin-bottom: 8px;
  }

  .inside-item p {
    font-size: 13px;
    line-height: 1.6;
    color: rgba(255,255,255,0.5);
  }

  /* ── BÔNUS ── */
  .section-bonus {
    background: var(--warm);
    padding: 100px 24px;
  }

  .bonus-header {
    text-align: center;
    margin-bottom: 56px;
  }

  .bonus-header h2 {
    font-family: 'Cormorant Garamond', serif;
    font-size: clamp(30px, 5vw, 48px);
    font-weight: 300;
    color: var(--text);
    margin-bottom: 16px;
  }

  .bonus-header p {
    font-size: 15px;
    color: var(--muted);
  }

  .bonus-list {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 16px;
  }

  .bonus-card {
    background: var(--white);
    border-radius: 18px;
    padding: 28px 24px;
    display: flex;
    gap: 18px;
    align-items: flex-start;
    border: 1px solid rgba(196,130,106,0.1);
    transition: box-shadow 0.3s;
  }

  .bonus-card:hover {
    box-shadow: 0 8px 32px rgba(107,61,46,0.08);
  }

  .bonus-num {
    font-family: 'Cormorant Garamond', serif;
    font-size: 36px;
    font-weight: 300;
    color: var(--blush);
    line-height: 1;
    min-width: 40px;
  }

  .bonus-card h4 {
    font-family: 'Cormorant Garamond', serif;
    font-size: 18px;
    font-weight: 500;
    margin-bottom: 6px;
    color: var(--text);
  }

  .bonus-card p {
    font-size: 13px;
    line-height: 1.6;
    color: var(--muted);
  }

  /* ── PREÇO ── */
  .section-price {
    background: var(--cream);
    padding: 100px 24px;
    text-align: center;
  }

  .price-box {
    max-width: 500px;
    margin: 0 auto;
    background: var(--white);
    border-radius: 28px;
    padding: 56px 48px;
    box-shadow: 0 24px 80px rgba(107,61,46,0.12);
    border: 1px solid rgba(196,130,106,0.15);
  }

  .price-box .eyebrow { text-align: center; }

  .price-box h2 {
    font-family: 'Cormorant Garamond', serif;
    font-size: 28px;
    font-weight: 400;
    color: var(--text);
    margin-bottom: 32px;
    line-height: 1.3;
  }

  .price-from {
    font-size: 13px;
    color: var(--muted);
    text-decoration: line-through;
    margin-bottom: 4px;
  }

  .price-main {
    font-family: 'Cormorant Garamond', serif;
    font-size: 72px;
    font-weight: 300;
    color: var(--deep);
    line-height: 1;
    margin-bottom: 4px;
  }

  .price-main sup {
    font-size: 28px;
    vertical-align: super;
  }

  .price-desc {
    font-size: 13px;
    color: var(--muted);
    margin-bottom: 36px;
  }

  .price-includes {
    text-align: left;
    margin-bottom: 36px;
    display: flex;
    flex-direction: column;
    gap: 12px;
  }

  .price-includes li {
    list-style: none;
    display: flex;
    align-items: center;
    gap: 12px;
    font-size: 14px;
    color: var(--text);
  }

  .price-includes li::before {
    content: '✓';
    width: 20px;
    height: 20px;
    background: rgba(196,130,106,0.15);
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 11px;
    color: var(--rose);
    flex-shrink: 0;
  }

  .btn-primary-large {
    display: block;
    width: 100%;
    background: linear-gradient(135deg, var(--deep), var(--rose));
    color: var(--white);
    font-family: 'DM Sans', sans-serif;
    font-size: 16px;
    font-weight: 500;
    padding: 20px 32px;
    border-radius: 100px;
    text-decoration: none;
    border: none;
    cursor: pointer;
    transition: all 0.3s ease;
    margin-bottom: 20px;
  }

  .btn-primary-large:hover {
    transform: translateY(-2px);
    box-shadow: 0 16px 40px rgba(107,61,46,0.3);
  }

  .guarantee-text {
    font-size: 13px;
    color: var(--muted);
    line-height: 1.6;
  }

  .urgency-bar {
    background: rgba(196,130,106,0.08);
    border: 1px solid rgba(196,130,106,0.2);
    border-radius: 12px;
    padding: 14px 20px;
    margin-bottom: 32px;
    font-size: 13px;
    color: var(--rose);
    font-weight: 500;
  }

  /* ── FAQ ── */
  .section-faq {
    background: var(--white);
    padding: 100px 24px;
  }

  .faq-header {
    text-align: center;
    margin-bottom: 56px;
  }

  .faq-header h2 {
    font-family: 'Cormorant Garamond', serif;
    font-size: clamp(30px, 5vw, 48px);
    font-weight: 300;
    color: var(--text);
  }

  .faq-list {
    max-width: 640px;
    margin: 0 auto;
    display: flex;
    flex-direction: column;
    gap: 2px;
  }

  .faq-item {
    border-bottom: 1px solid var(--warm);
    padding: 24px 0;
  }

  .faq-item summary {
    font-family: 'Cormorant Garamond', serif;
    font-size: 20px;
    font-weight: 500;
    color: var(--text);
    cursor: pointer;
    list-style: none;
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 16px;
  }

  .faq-item summary::after {
    content: '+';
    font-size: 22px;
    color: var(--rose);
    flex-shrink: 0;
    transition: transform 0.3s;
  }

  .faq-item[open] summary::after {
    transform: rotate(45deg);
  }

  .faq-item p {
    font-size: 15px;
    line-height: 1.7;
    color: var(--muted);
    margin-top: 16px;
    padding-right: 24px;
  }

  /* ── FECHAMENTO ── */
  .section-close {
    background: linear-gradient(160deg, #2D1F1A 0%, #6B3D2E 100%);
    padding: 120px 24px;
    text-align: center;
  }

  .section-close h2 {
    font-family: 'Cormorant Garamond', serif;
    font-size: clamp(36px, 6vw, 64px);
    font-weight: 300;
    color: var(--white);
    line-height: 1.2;
    margin-bottom: 24px;
  }

  .section-close h2 em {
    font-style: italic;
    color: var(--blush);
  }

  .section-close p {
    font-size: 16px;
    color: rgba(255,255,255,0.65);
    margin-bottom: 48px;
    line-height: 1.7;
  }

  .section-close .btn-primary {
    font-size: 16px;
    padding: 20px 52px;
  }

  .close-guarantee {
    margin-top: 24px;
    font-size: 13px;
    color: rgba(255,255,255,0.4);
    letter-spacing: 0.5px;
  }

  /* ── FOOTER ── */
  footer {
    background: var(--text);
    padding: 32px 24px;
    text-align: center;
    font-size: 12px;
    color: rgba(255,255,255,0.3);
    letter-spacing: 1px;
  }

  /* ── ANIMATIONS ── */
  @keyframes fadeUp {
    from { opacity: 0; transform: translateY(24px); }
    to { opacity: 1; transform: translateY(0); }
  }

  .reveal {
    opacity: 0;
    transform: translateY(32px);
    transition: opacity 0.7s ease, transform 0.7s ease;
  }

  .reveal.visible {
    opacity: 1;
    transform: translateY(0);
  }

  /* ── MOBILE ── */
  @media (max-width: 600px) {
    .price-box { padding: 40px 28px; }
    .pain-cards, .pillars, .inside-grid, .bonus-list { grid-template-columns: 1fr; }
  }
</style>
</head>
<body>

<!-- ═══ HERO ═══ -->
<section class="hero">
  <span class="hero-badge">Protocolo 12 Semanas</span>
  <h1>O caminho para<br><em>o positivo</em></h1>
  <p class="hero-sub">Clareza. Preparo. Direção.</p>
  <p class="hero-desc">
    Um protocolo completo de 12 semanas que organiza seu corpo, equilibra seus hormônios e mostra exatamente o que fazer — passo a passo.
  </p>
  <a href="#preco" class="btn-primary">Quero começar minha preparação</a>
  <div class="hero-tags">
    <span>Fertilidade</span>
    <span>Nutrição</span>
    <span>Autoconhecimento</span>
    <span>Sem medicamentos</span>
  </div>
</section>

<!-- ═══ DOR ═══ -->
<section class="section-pain">
  <div class="container">
    <span class="eyebrow reveal">Você se reconhece aqui?</span>
    <p class="quote-big reveal">
      O problema não é a falta de tentativa.<br>
      <em>É a falta de preparo.</em>
    </p>
    <div class="pain-cards reveal">
      <div class="pain-card">
        <span class="pain-icon">🗓</span>
        <h3>Todo mês a mesma dor</h3>
        <p>A expectativa que sobe e cai. O ciclo emocional que cansa e desgasta profundamente.</p>
      </div>
      <div class="pain-card">
        <span class="pain-icon">❓</span>
        <h3>Sem saber se o corpo está pronto</h3>
        <p>A dúvida persiste. Falta clareza sobre o que está acontecendo dentro de você.</p>
      </div>
      <div class="pain-card">
        <span class="pain-icon">🌀</span>
        <h3>Tentando no escuro</h3>
        <p>Sem direção, sem estratégia. Só esperança — e esperança sem preparo não é suficiente.</p>
      </div>
    </div>
  </div>
</section>

<!-- ═══ MECANISMO ═══ -->
<section class="section-mechanism">
  <div class="container-wide">
    <div class="mechanism-header reveal">
      <span class="eyebrow">Por que 12 semanas?</span>
      <h2>Seu corpo tem um ritmo.<br>A ciência explica.</h2>
      <p>Entender isso muda tudo sobre como você se prepara.</p>
    </div>

    <div class="big-stat reveal">
      <span class="number">90</span>
      <span class="number-label">dias de maturação do óvulo</span>
      <p class="stat-text">
        Seu óvulo leva cerca de 90 dias para amadurecer. O que você come, como dorme, como cuida do seu corpo hoje — define a qualidade do ciclo que vem.
        <br><br>
        <strong style="color:var(--blush)">O que você faz agora importa mais do que você imagina.</strong>
      </p>
    </div>

    <div class="pillars">
      <div class="pillar reveal">
        <span class="pillar-num">01 · Nutrição</span>
        <h3>Maturação do óvulo</h3>
        <p>O óvulo precisa de nutrição e tempo para amadurecer com qualidade. Cada escolha alimentar hoje reflete no ciclo que vem.</p>
      </div>
      <div class="pillar reveal">
        <span class="pillar-num">02 · Equilíbrio</span>
        <h3>Hormônios em harmonia</h3>
        <p>Hormônios em equilíbrio criam o cenário ideal para a concepção. Hábitos simples podem mudar esse cenário completamente.</p>
      </div>
      <div class="pillar reveal">
        <span class="pillar-num">03 · Ambiente</span>
        <h3>Útero preparado</h3>
        <p>Um ambiente uterino saudável recebe e sustenta com naturalidade. Isso é preparável — e você vai aprender como.</p>
      </div>
    </div>
  </div>
</section>

<!-- ═══ O QUE ESTÁ DENTRO ═══ -->
<section class="section-inside">
  <div class="container-wide">
    <span class="eyebrow reveal">O protocolo</span>
    <h2 class="reveal">Um caminho completo<br>em suas mãos</h2>
    <p class="lead reveal">12 semanas organizadas de forma progressiva e gentil. Cada semana com orientações claras e práticas — no seu ritmo.</p>

    <div class="inside-grid reveal">
      <div class="inside-item">
        <div class="check">✓</div>
        <h4>Entender o corpo</h4>
        <p>Descubra como sua fertilidade realmente funciona — sem achismo, com clareza.</p>
      </div>
      <div class="inside-item">
        <div class="check">✓</div>
        <h4>Ajustar a alimentação</h4>
        <p>O que comer em cada fase do ciclo para nutrir a fertilidade de dentro pra fora.</p>
      </div>
      <div class="inside-item">
        <div class="check">✓</div>
        <h4>Reduzir inflamação</h4>
        <p>Hábitos simples que criam o ambiente certo para a concepção acontecer.</p>
      </div>
      <div class="inside-item">
        <div class="check">✓</div>
        <h4>Identificar o período fértil</h4>
        <p>Aprenda a ler os sinais do seu próprio corpo com confiança e clareza.</p>
      </div>
      <div class="inside-item">
        <div class="check">✓</div>
        <h4>Agir em cada fase</h4>
        <p>Saber exatamente o que fazer — e quando fazer — em cada semana do protocolo.</p>
      </div>
      <div class="inside-item">
        <div class="check">✓</div>
        <h4>Cuidar da mente também</h4>
        <p>Ferramentas para lidar com a
