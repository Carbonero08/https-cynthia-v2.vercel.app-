<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>$CYNTHIA - La muñeca está suelta</title>
  <style>
    body {
      background-color: #1a1a1a;
      font-family: 'Comic Sans MS', cursive, sans-serif;
      margin: 0;
      padding: 0;
      text-align: center;
      color: #fff;
    }
    header {
      background: #e60073;
      padding: 2rem 1rem;
    }
    .hero img {
      max-width: 250px;
      border-radius: 20px;
      box-shadow: 0 0 20px #ff3399;
    }
    .countdown {
      font-size: 2rem;
      margin: 1rem 0;
      color: #ffccff;
    }
    section {
      padding: 2rem 1rem;
    }
    .tokenomics {
      background-color: #330033;
      border-top: 4px solid #ff3399;
    }
    .roadmap, .about {
      background-color: #1a1a1a;
    }
    .tokenomics ul, .roadmap ul {
      list-style-type: none;
      padding: 0;
    }
    .tokenomics li, .roadmap li {
      margin: 1rem 0;
      color: #ff99cc;
    }
    .links a {
      display: inline-block;
      margin: 0.5rem;
      padding: 0.75rem 1.5rem;
      background-color: #ff3399;
      color: white;
      text-decoration: none;
      border-radius: 8px;
      font-weight: bold;
    }
    footer {
      background-color: #330033;
      padding: 2rem;
    }
    h1, h2 {
      color: #ff66cc;
    }
  </style>
</head>
<body>
  <header>
    <div class="hero">
      <h1>$CYNTHIA</h1>
      <p>La muñeca está fuera de control 🧠🔥</p>
      <img src="https://cynthia-v2.vercel.app/img/cynthia_pirata.png" alt="Cynthia Pirata" />
      <div class="countdown" id="countdown">Lanzamiento en: ...</div>
    </div>
    <div class="links">
      <a href="#">ÚNETE A TELEGRAM</a>
      <a href="#">SEGUINOS EN X</a>
    </div>
  </header>

  <section class="tokenomics">
    <h2>Tokenomics</h2>
    <p>Supply total: 100,000,000 $CYNTHIA</p>
    <ul>
      <li>🔥 40% Quemado</li>
      <li>🔒 20% Bloqueado (Founder/Dev)</li>
      <li>🎁 20% Airdrop + Marketing</li>
      <li>💰 20% Preventa + Liquidez</li>
    </ul>
    <p><em>“Soy Cynthia, la capitana. Quemé el 40% y los tesoros serán repartidos con mi tripulación.”</em></p>
    <p><em>“No es una utilidad… es una maldición pirata en la blockchain. ⛵🔥”</em></p>
  </section>

  <section class="roadmap">
    <h2>Roadmap</h2>
    <ul>
      <li>🧪 Fase 1: Web + comunidad + memes + hype pirata</li>
      <li>🚀 Fase 2: Lanzamiento en pump.fun + contador regresivo</li>
      <li>📈 Fase 3: Airdrop + Dexscreener + holders 500+</li>
      <li>🦜 Fase 4: Merch de Cynthia + memes diarios + raids</li>
      <li>👑 Fase 5: Burn ritual + sticker pack oficial</li>
    </ul>
  </section>

  <section class="about">
    <h2>¿Qué es Cynthia?</h2>
    <p>
      Cynthia es la capitana de los degenerados. Una muñeca perdida del multiverso que encontró su camino en la blockchain de Solana.
      Inspirada por Rugrats, Internet y el caos, $CYNTHIA no es solo una moneda, es una fuerza sin utilidad... pero con destino.
    </p>
  </section>

  <footer class="links">
    <a href="#">Telegram</a>
    <a href="#">X (Twitter)</a>
    <a href="#">Ver en Dexscreener</a>
    <a href="#">Proof of Burn</a>
  </footer>

  <script>
    const launchDate = new Date("2025-08-20T19:00:00Z").getTime();
    const countdown = document.getElementById("countdown");
    const x = setInterval(function () {
      const now = new Date().getTime();
      const distance = launchDate - now;
      const days = Math.floor(distance / (1000 * 60 * 60 * 24));
      const hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
      const minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
      const seconds = Math.floor((distance % (1000 * 60)) / 1000);
      countdown.innerHTML = `Lanzamiento en: ${days}d ${hours}h ${minutes}m ${seconds}s`;
      if (distance < 0) {
        clearInterval(x);
        countdown.innerHTML = "¡YA LANZAMOS EN PUMP.FUN!";
      }
    }, 1000);
  </script>
</body>
</html>