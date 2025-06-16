<html lang="pt">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>História de Angola</title>
  <style>
    * { margin: 0; padding: 0; box-sizing: border-box; }

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

    .idioma-selector {
      margin-top: 10px;
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

    button, .curiosidade-link, select {
      padding: 10px 20px;
      background-color: #CC0000;
      color: #fff;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      text-decoration: none;
      display: inline-block;
      margin-top: 15px;
    }

    button:hover, .curiosidade-link:hover, select:hover {
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
    <h1 id="titulo">História de Angola</h1>
    <nav>
      <ul>
        <li><a href="#pre-colonial" id="nav1">Pré-Colonial</a></li>
        <li><a href="#colonial" id="nav2">Colonial</a></li>
        <li><a href="#independencia" id="nav3">Independência</a></li>
        <li><a href="#pos-independencia" id="nav4">Pós-Independência</a></li>
      </ul>
    </nav>

    <div class="idioma-selector">
      <label for="idioma" style="color: #FFD700;">Mudar de idioma:</label>
      <select id="idioma" onchange="mudarIdioma(this.value)">
        <option value="pt">Português</option>
        <option value="en">Inglês</option>
        <option value="fr">Francês</option>
        <option value="es">Espanhol</option>
      </select>
    </div>
  </header>

  <section id="pre-colonial">
    <h2 id="preTitulo">Angola Pré-Colonial</h2>
    <img class="ilustracao" src="I1.jpg">
    <p id="preTexto">Antes da chegada dos colonizadores, Angola era formada por reinos bem organizados, como o Reino do Kongo, Ndongo e Lunda. Esses reinos possuíam sistemas políticos próprios, comércio interno e externo, e uma cultura rica baseada em tradições orais, agricultura e mineração.</p>
  </section>

  <section id="colonial">
    <h2 id="colTitulo">Período Colonial</h2>
    <img class="ilustracao" src="I2.png">
    <p id="colTexto">Durante a colonização portuguesa, os recursos naturais e os povos de Angola foram explorados. Surgiram diversas formas de resistência, como a luta da Rainha Nzinga, que é símbolo de coragem, diplomacia e defesa da soberania do seu povo frente à opressão europeia.</p>
    <a href="https://pt.wikipedia.org/wiki/Nzinga_de_Mbandi" target="_blank" class="curiosidade-link" id="linkNzinga">Saiba mais sobre a Rainha Nzinga</a>
  </section>

  <section id="independencia">
    <h2 id="indTitulo">Luta pela Independência</h2>
    <img class="ilustracao" src="I3.jpeg">
    <p id="indTexto">Com o tempo, movimentos de libertação como o MPLA, FNLA e UNITA organizaram-se para conquistar a independência. Após anos de luta armada e resistência popular, Angola tornou-se independente em 11 de Novembro de 1975, tornando-se uma república soberana.</p>
  </section>

  <section id="pos-independencia">
    <h2 id="posTitulo">Angola Pós-Independência</h2>
    <img class="ilustracao" src="I4.webp">
    <p id="posTexto">Depois da independência, o país enfrentou uma longa guerra civil. Nos últimos anos, Angola tem investido no desenvolvimento de infraestruturas, educação e saúde. A reconstrução nacional é um esforço contínuo que reflete a força e a resiliência do povo angolano.</p>

    <label for="curiosidade" id="curLabel">Escolha uma curiosidade:</label>
    <select id="curiosidade" onchange="verCuriosidade(this.value)">
      <option value="">-- Selecione --</option>
      <option value="https://pt.wikipedia.org/wiki/Economia_de_Angola" id="opt1">Economia de Angola</option>
      <option value="https://pt.wikipedia.org/wiki/Cultura_de_Angola" id="opt2">Cultura de Angola</option>
      <option value="https://pt.wikipedia.org/wiki/Diamantes_de_sangue" id="opt3">Diamantes em Angola</option>
    </select>
  </section>

  <footer>
    <p id="rodape">Site criado por Silvia Sina, Silvina Martins, Simone Zua e Deblá Bejamim - 12ª Classe - IMCL</p>
  </footer>

  <script>
    const traducoes = {
      pt: {
        titulo: "História de Angola",
        nav1: "Pré-Colonial",
        nav2: "Colonial",
        nav3: "Independência",
        nav4: "Pós-Independência",
        preTitulo: "Angola Pré-Colonial",
        preTexto: "Antes da chegada dos colonizadores, Angola era formada por reinos bem organizados...",
        colTitulo: "Período Colonial",
        colTexto: "Durante a colonização portuguesa, os recursos naturais e os povos de Angola foram explorados...",
        linkNzinga: "Saiba mais sobre a Rainha Nzinga",
        indTitulo: "Luta pela Independência",
        indTexto: "Com o tempo, movimentos de libertação como o MPLA, FNLA e UNITA...",
        posTitulo: "Angola Pós-Independência",
        posTexto: "Depois da independência, o país enfrentou uma longa guerra civil...",
        curLabel: "Escolha uma curiosidade:",
        opt1: "Economia de Angola",
        opt2: "Cultura de Angola",
        opt3: "Diamantes em Angola",
        rodape: "Site criado por Silvia Sina, Silvina Martins, Simone Zua e Deblá Bejamim - 12ª Classe - IMCL"
      },
      en: {
        titulo: "History of Angola",
        nav1: "Pre-Colonial",
        nav2: "Colonial",
        nav3: "Independence",
        nav4: "Post-Independence",
        preTitulo: "Pre-Colonial Angola",
        preTexto: "Before the arrival of colonizers, Angola was made up of organized kingdoms...",
        colTitulo: "Colonial Period",
        colTexto: "During Portuguese colonization, Angola's natural resources and people were exploited...",
        linkNzinga: "Learn more about Queen Nzinga",
        indTitulo: "Struggle for Independence",
        indTexto: "Over time, liberation movements such as MPLA, FNLA and UNITA...",
        posTitulo: "Post-Independence Angola",
        posTexto: "After independence, the country went through a long civil war...",
        curLabel: "Choose a curiosity:",
        opt1: "Angola's Economy",
        opt2: "Angolan Culture",
        opt3: "Diamonds in Angola",
        rodape: "Website created by Silvia Sina, Silvina Martins, Simone Zua and Deblá Bejamim - 12th Grade - IMCL"
      },
      fr: {
        titulo: "Histoire de l'Angola",
        nav1: "Précolonial",
        nav2: "Colonial",
        nav3: "Indépendance",
        nav4: "Post-Indépendance",
        preTitulo: "L'Angola Précolonial",
        preTexto: "Avant l'arrivée des colonisateurs, l'Angola était composé de royaumes bien organisés...",
        colTitulo: "Période Coloniale",
        colTexto: "Pendant la colonisation portugaise, les ressources et les peuples de l'Angola ont été exploités...",
        linkNzinga: "En savoir plus sur la Reine Nzinga",
        indTitulo: "Lutte pour l'Indépendance",
        indTexto: "Au fil du temps, des mouvements de libération comme le MPLA, le FNLA et l'UNITA...",
        posTitulo: "L'Angola Post-Indépendance",
        posTexto: "Après l'indépendance, le pays a traversé une longue guerre civile...",
        curLabel: "Choisissez une curiosité :",
        opt1: "Économie de l'Angola",
        opt2: "Culture de l'Angola",
        opt3: "Diamants en Angola",
        rodape: "Site créé par Silvia Sina, Silvina Martins, Simone Zua et Deblá Bejamim - 12e classe - IMCL"
      },
      es: {
        titulo: "Historia de Angola",
        nav1: "Precolonial",
        nav2: "Colonial",
        nav3: "Independencia",
        nav4: "Post-Independencia",
        preTitulo: "Angola Precolonial",
        preTexto: "Antes de la llegada de los colonizadores, Angola estaba formada por reinos bien organizados...",
        colTitulo: "Período Colonial",
        colTexto: "Durante la colonización portuguesa, los recursos y pueblos de Angola fueron explotados...",
        linkNzinga: "Más sobre la Reina Nzinga",
        indTitulo: "Lucha por la Independencia",
        indTexto: "Con el tiempo, movimientos de liberación como el MPLA, FNLA y UNITA...",
        posTitulo: "Angola Post-Independencia",
        posTexto: "Después de la independencia, el país enfrentó una larga guerra civil...",
        curLabel: "Elige una curiosidad:",
        opt1: "Economía de Angola",
        opt2: "Cultura de Angola",
        opt3: "Diamantes en Angola",
        rodape: "Sitio creado por Silvia Sina, Silvina Martins, Simone Zua y Deblá Bejamim - 12ª Clase - IMCL"
      }
    };

    function mudarIdioma(idioma) {
      const t = traducoes[idioma];
      document.getElementById("titulo").textContent = t.titulo;
      document.getElementById("nav1").textContent = t.nav1;
      document.getElementById("nav2").textContent = t.nav2;
      document.getElementById("nav3").textContent = t.nav3;
      document.getElementById("nav4").textContent = t.nav4;
      document.getElementById("preTitulo").textContent = t.preTitulo;
      document.getElementById("preTexto").textContent = t.preTexto;
      document.getElementById("colTitulo").textContent = t.colTitulo;
      document.getElementById("colTexto").textContent = t.colTexto;
      document.getElementById("linkNzinga").textContent = t.linkNzinga;
      document.getElementById("indTitulo").textContent = t.indTitulo;
      document.getElementById("indTexto").textContent = t.indTexto;
      document.getElementById("posTitulo").textContent = t.posTitulo;
      document.getElementById("posTexto").textContent = t.posTexto;
      document.getElementById("curLabel").textContent = t.curLabel;
      document.getElementById("opt1").textContent = t.opt1;
      document.getElementById("opt2").textContent = t.opt2;
      document.getElementById("opt3").textContent = t.opt3;
      document.getElementById("rodape").textContent = t.rodape;
    }

    function verCuriosidade(link) {
      if (link) window.open(link, '_blank');
    }
  </script>
</body>
</html>

