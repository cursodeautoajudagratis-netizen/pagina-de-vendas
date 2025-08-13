<!doctype html>
<html lang="pt-BR">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Offer X — Página de Vendas</title>
  <meta name="description" content="Página de vendas enxuta e de alta conversão com checkout por link de pagamento." />
  <meta property="og:title" content="Offer X — Página de Vendas" />
  <meta property="og:description" content="Página de vendas enxuta e de alta conversão com checkout por link de pagamento." />
  <meta property="og:type" content="website" />
  <meta property="og:image" content="/og-image.jpg" />
  <style>
    :root{
      --bg:#0b1020; --card:#121735; --muted:#2a315c; --brand:#6ee7b7; --brand-2:#3b82f6; --text:#e6e8f2; --text-dim:#b7bed3;
    }
    *{box-sizing:border-box}
    html,body{margin:0; padding:0; background:var(--bg); color:var(--text); font-family:ui-sans-serif, system-ui, -apple-system, Segoe UI, Roboto, Ubuntu, Cantarell, Noto Sans, Arial, "Apple Color Emoji","Segoe UI Emoji";}
    a{color:inherit; text-decoration:none}
    img{max-width:100%; display:block}
    .container{max-width:1100px; margin-inline:auto; padding:24px}
    .hero{display:grid; gap:24px; align-items:center; grid-template-columns:1.2fr .8fr;}
    .card{background:linear-gradient(180deg, rgba(255,255,255,.04), rgba(255,255,255,.02)); border:1px solid rgba(255,255,255,.08); border-radius:24px; box-shadow:0 10px 30px rgba(0,0,0,.25)}
    .cta{display:inline-flex; align-items:center; justify-content:center; gap:12px; padding:18px 22px; border-radius:14px; background:linear-gradient(90deg, var(--brand), var(--brand-2)); color:#0a0f1f; font-weight:800; font-size:1.05rem; border:none; cursor:pointer; transition:transform .08s ease}
    .cta:active{transform:scale(.98)}
    .price{font-size:2rem; font-weight:900; letter-spacing:.3px}
    .badge{display:inline-block; padding:6px 10px; border-radius:999px; background:rgba(255,255,255,.08); color:var(--text-dim); font-size:.85rem}
    .grid-3{display:grid; grid-template-columns:repeat(3, 1fr); gap:16px}
    .feature{padding:18px; border-radius:18px; background:rgba(255,255,255,.04); border:1px solid rgba(255,255,255,.07)}
    .section{padding:48px 0}
    .section h2{margin:0 0 14px}
    .bullets{display:grid; gap:10px; margin:0; padding:0; list-style:none}
    .bullets li{display:flex; gap:10px; align-items:flex-start}
    .check{flex:0 0 22px; height:22px; border-radius:6px; background:linear-gradient(145deg, var(--brand), var(--brand-2)); display:inline-grid; place-items:center; font-weight:900; color:#0b1020}
    .faq-item{background:rgba(255,255,255,.04); border:1px solid rgba(255,255,255,.09); border-radius:16px; padding:16px}
    .guarantee{border:1px dashed rgba(255,255,255,.25); background:rgba(110,231,183,.08); color:#d6ffef}
    footer{opacity:.8; font-size:.9rem}
    .floating-whatsapp{position:fixed; right:18px; bottom:18px; padding:12px 14px; border-radius:999px; background:#25D366; color:#001a0e; font-weight:800; box-shadow:0 10px 30px rgba(0,0,0,.35)}
    .testimonial{display:flex; gap:12px; align-items:flex-start}
    .avatar{width:40px; height:40px; border-radius:50%; background:#2a315c}

    /* Responsive */
    @media (max-width: 900px){
      .hero{grid-template-columns:1fr}
    }
  </style>
</head>
<body>
  <header class="container" style="padding-top:28px;">
    <div style="display:flex; align-items:center; justify-content:space-between; gap:16px;">
      <div style="display:flex; align-items:center; gap:10px;">
        <div style="width:36px; height:36px; border-radius:12px; background:linear-gradient(180deg, var(--brand), var(--brand-2));"></div>
        <strong>Offer X</strong>
      </div>
      <div class="badge">Pagamento 100% seguro • 256‑bit</div>
    </div>
  </header>

  <main class="container">
    <!-- HERO -->
    <section class="hero section card" style="padding:28px;">
      <div>
        <div class="badge">Vagas limitadas</div>
        <h1 style="font-size:clamp(1.8rem, 3.6vw, 3rem); line-height:1.1; margin:.5rem 0 1rem;">Título forte da sua oferta</h1>
        <p style="opacity:.9; max-width:55ch;">Subtítulo que resume o principal benefício e elimina objeções. Use linguagem simples, foco no resultado e prazo.</p>
        <ul class="bullets" style="margin-top:16px;">
          <li><span class="check">✓</span><span>Benefício 1 direto ao ponto</span></li>
          <li><span class="check">✓</span><span>Benefício 2 com um detalhe específico</span></li>
          <li><span class="check">✓</span><span>Benefício 3 destacando rapidez/segurança</span></li>
        </ul>
        <div style="display:flex; align-items:center; gap:14px; margin-top:22px; flex-wrap:wrap;">
          <div class="price" id="preco">R$ <span data-price>197,00</span></div>
          <div class="badge">ou 12x no cartão</div>
        </div>
        <div style="display:flex; gap:12px; margin-top:22px; flex-wrap:wrap;">
          <!-- SUBSTITUA O HREF PELO SEU LINK DE PAGAMENTO -->
          <a id="btn-comprar" class="cta" href="#" target="_blank" rel="noopener">Quero garantir minha vaga</a>
          <a class="badge" href="#faq">Tirar dúvidas</a>
        </div>
        <div style="margin-top:12px; opacity:.85; font-size:.95rem;">Aceitamos Pix • Cartão • Boleto (via provedor de pagamentos)</div>
      </div>
      <div>
        <div class="card" style="padding:16px;">
          <img src="https://images.unsplash.com/photo-1557264305-0fcf4f5a5c33?q=80&w=1400&auto=format&fit=crop" alt="Mockup do produto" style="border-radius:16px;" />
        </div>
        <div class="badge" style="margin-top:8px; display:block; text-align:center;">Imagem ilustrativa do produto/serviço</div>
      </div>
    </section>

    <!-- PROVAS/FEATURES -->
    <section class="section">
      <h2>O que você vai receber</h2>
      <div class="grid-3">
        <div class="feature"><strong>Módulo 1</strong><br><span class="text-dim">Descrição breve do item incluso.</span></div>
        <div class="feature"><strong>Módulo 2</strong><br><span class="text-dim">Descrição breve do item incluso.</span></div>
        <div class="feature"><strong>Bônus</strong><br><span class="text-dim">Descreva um bônus irresistível.</span></div>
      </div>
    </section>

    <!-- PROVAS SOCIAIS -->
    <section class="section">
      <h2>Depoimentos</h2>
      <div class="grid-3">
        <div class="feature testimonial"><div class="avatar"></div><div><strong>Ana</strong><br>"Resultado acima do esperado!"</div></div>
        <div class="feature testimonial"><div class="avatar"></div><div><strong>Bruno</strong><br>"Processo simples e rápido."</div></div>
        <div class="feature testimonial"><div class="avatar"></div><div><strong>Carla</strong><br>"Suporte excelente!"</div></div>
      </div>
    </section>

    <!-- GARANTIA / RISCO REVERSO -->
    <section class="section">
      <div class="feature guarantee">
        <strong>Garantia incondicional de 7 dias.</strong> Se não for para você, devolvemos 100% do valor. Basta um e‑mail dentro do prazo.
      </div>
    </section>

    <!-- FAQ -->
    <section id="faq" class="section">
      <h2>Perguntas frequentes</h2>
      <div class="grid-3">
        <div class="faq-item"><strong>Como recebo o acesso?</strong><br>Você recebe por e‑mail imediatamente após o pagamento ser confirmado.</div>
        <div class="faq-item"><strong>Quais formas de pagamento?</strong><br>Pix, cartão de crédito e boleto (dependendo do provedor).</div>
        <div class="faq-item"><strong>Tenho suporte?</strong><br>Sim, suporte por e‑mail em horário comercial.</div>
      </div>
    </section>
  </main>

  <footer class="container section">
    <div style="display:flex; justify-content:space-between; gap:16px; flex-wrap:wrap;">
      <div>© <span id="ano"></span> Sua Marca</div>
      <div><a href="#">Termos</a> • <a href="#">Privacidade</a> • <a href="#">Contato</a></div>
    </div>
  </footer>

  <!-- Botão WhatsApp (opcional) -->
  <a class="floating-whatsapp" href="#" id="zap" target="_blank" rel="noopener">WhatsApp</a>

  <script>
    // Personalização rápida — edite aqui
    const CONFIG = {
      produto: 'Curso de Autoajuda (Mudando Vidas)',
      preco: '1,00', // valor exibido (BRL). Ex: '97,00' ou '1.297,00'
      pagamentoUrl: '00020126410014br.gov.bcb.pix0119lifenow18@gmail.com52040000530398654041.005802BR5925Leidynnara Keith Rodrigue6008Brasilia62080504mpda6304C7D7', // COLE AQUI O LINK DE PAGAMENTO (Stripe, Mercado Pago, PagSeguro, etc.)
      whatsapp: '55319712318155', // opcional: número com DDI+DDD, ex: '5511999999999'
      mensagemZap: 'Olá! Tenho uma dúvida sobre a oferta.'
    };

    // Preenche textos e links automaticamente
    document.title = CONFIG.produto + ' — Página de Vendas';
    const priceEl = document.querySelector('[data-price]');
    if (priceEl) priceEl.textContent = CONFIG.preco;
    const btn = document.getElementById('btn-comprar');
    if (btn) btn.href = CONFIG.pagamentoUrl;
    const ano = document.getElementById('ano');
    if (ano) ano.textContent = new Date().getFullYear();

    // WhatsApp
    const zap = document.getElementById('zap');
    if (CONFIG.whatsapp) {
      zap.style.display = 'inline-block';
      zap.href = `https://wa.me/${CONFIG.whatsapp}?text=${encodeURIComponent(CONFIG.mensagemZap)}`;
    } else {
      zap.style.display = 'none';
    }

    // Event tracking simples (para usar no Google Tag Manager)
    btn?.addEventListener('click', () => {
      window.dataLayer = window.dataLayer || [];
      window.dataLayer.push({event: 'cta_click', value: CONFIG.preco});
    });
  </script>
</body>
</html>
