<!DOCTYPE html>
<html lang="pt">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>História de Angola</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: Arial, sans-serif;
      line-height: 1.6;
      background: url('https://upload.wikimedia.org/wikipedia/commons/thumb/9/9d/Flag_of_Angola.svg/1280px-Flag_of_Angola.svg.png') no-repeat center center fixed;
      background-size: cover;
      color: #333;
    }

    header {
      background-color: rgba(0, 0, 0, 0.8);
      color: #FFD700;
      padding: 20px;
      text-align: center;
    }

    nav ul {
      list-style: none;
      display: flex;
      justify-content: center;
      gap: 15px;
      margin-top: 10px;
    }

    nav ul li a {
      color: #FFD700;
      text-decoration: none;
      font-weight: bold;
    }

    nav ul li a:hover {
      text-decoration: underline;
    }

    section {
      padding: 30px;
      background-color: rgba(255, 255, 255, 0.9);
      margin: 20px auto;
      max-width: 900px;
      border-radius: 8px;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
    }

    h2 {
      color: #CC0000;
      margin-bottom: 15px;
    }

    button, .curiosidade-link {
      padding: 10px 20px;
      background-color: #CC0000;
      color: #fff;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      text-decoration: none;
      display: inline-block;
    }

    button:hover, .curiosidade-link:hover {
      background-color: #A30000;
    }

    footer {
      background-color: rgba(0, 0, 0, 0.8);
      color: #FFD700;
      text-align: center;
      padding: 15px;
      width: 100%;
    }

    img.ilustracao {
      width: 100%;
      border-radius: 5px;
      margin: 15px 0;
    }

    @media screen and (max-width: 600px) {
      nav ul {
        flex-direction: column;
        gap: 10px;
      }

      section {
        margin: 10px;
        padding: 20px;
      }
    }
  </style>
</head>
<body>
  <header>
    <h1>História de Angola</h1>
    <nav>
      <ul>
        <li><a href="#pre-colonial">Pré-Colonial</a></li>
        <li><a href="#colonial">Colonial</a></li>
        <li><a href="#independencia">Independência</a></li>
        <li><a href="#pos-independencia">Pós-Independência</a></li>
      </ul>
    </nav>
  </header>

  <section id="pre-colonial">
    <h2>Angola Pré-Colonial</h2>
    <img class="ilustracao" src="OIP.JPEG" alt="Reino do Kongo">
    <p>Antes da chegada dos colonizadores, Angola era formada por vários reinos como o Reino do Kongo, Ndongo e Lunda. Esses reinos tinham sistemas organizados de governo, comércio e cultura.</p>
  </section>

  <section id="colonial">
    <h2>Período Colonial</h2>
    <img class="ilustracao" src="Nzinga.WEBP" alt="Rainha Nzinga">
    <p>Durante o período colonial, Portugal ocupou o território angolano, explorando os recursos naturais e a mão de obra local. Heróis como a Rainha Nzinga e Mandume lutaram bravamente contra a colonização.</p>
    <a href="https://pt.wikipedia.org/wiki/Nzinga_de_Mbandi" target="_blank" class="curiosidade-link">Saiba mais sobre a Rainha Nzinga</a>
  </section>

  <section id="independencia">
    <h2>Luta pela Independência</h2>
    <img class="ilustracao" src="cartaz2.jpg" alt="Independência de Angola - Memória">
    <p>O povo angolano lutou durante muitos anos pela liberdade. Em 11 de Novembro de 1975, Angola tornou-se independente graças ao esforço de movimentos como o MPLA, FNLA e UNITA.</p>
  </section>

  <section id="pos-independencia">
    <h2>Angola Pós-Independência</h2>
    <img class="ilustracao" src="L.jpeg" alt="Luanda Moderna">
    <p>Após a independência, o país passou por uma guerra civil longa, mas hoje caminha rumo ao desenvolvimento com foco na educação, saúde e infraestrutura.</p>
  <section>
   <button onclick="mostrarCuriosidade()">Clique para ver uma curiosidade</button>
  </section>
  <footer>
    <p>Site criado por Silvia Sina, Silvina Martins, Simone Zua e Deblá Bejamim - 12ª Classe - IMCL</p>
  </footer>
</body>
</html>
