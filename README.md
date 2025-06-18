
<html lang="pt">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="Site educativo sobre a história de Angola com informações sobre os períodos pré-colonial, colonial, independência e pós-independência.">
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
    <h2>Período Pré-Colonial</h2>
    <img class="ilustracao" src="i1.jpg">
    <p id="pre-colonial-text">Antes da chegada dos colonizadores, Angola era habitada por diversos grupos étnicos com estruturas sociais, políticas e económicas próprias. Reinos como o do Congo, Ndongo e Lunda tinham sistemas de governo organizados e culturas ricas.</p>
  </section>

  <section id="colonial">
    <h2>Período Colonial</h2>
    <img class="ilustracao" src="i2.png">
    <p id="colonial-text">A colonização portuguesa iniciou-se no século XV e intensificou-se nos séculos seguintes. Houve resistência por parte dos povos locais, mas Portugal consolidou o seu domínio, explorando recursos e impondo o seu controlo administrativo e cultural.</p>
  </section>

  <section id="independencia">
    <h2>Independência</h2>
    <img class="ilustracao" src="i3.jpeg">
    <p id="independencia-text">Angola conquistou a sua independência de Portugal a 11 de novembro de 1975, após anos de luta armada liderada por movimentos como o MPLA, FNLA e UNITA. A independência foi um marco importante, mas seguiu-se um longo período de guerra civil.</p>
  </section>

  <section id="pos-independencia">
    <h2>Pós-Independência</h2>
    <img class="ilustracao" src="i4.jpeg">
    <p id="pos-independencia-text">Após o fim da guerra civil em 2002, Angola iniciou um processo de reconstrução nacional. Investimentos em infraestrutura, educação e saúde foram intensificados, embora desafios sociais e económicos ainda persistam.</p>
  <section>
    <label for="curiosidade" id="curLabel">Escolha uma curiosidade:</label>
    <select id="curiosidade" onchange="verCuriosidade(this.value)">
      <option value="">-- Selecione --</option>
      <option value="https://pt.wikipedia.org/wiki/Economia_de_Angola" id="opt1">Economia de Angola</option>
      <option value="https://pt.wikipedia.org/wiki/Cultura_de_Angola" id="opt2">Cultura de Angola</option>
      <option value="https://pt.wikipedia.org/wiki/Diamantes_de_sangue" id="opt3">Diamantes em Angola</option>
    </select>
  </section>


  <footer>
    &copy; 2025 História de Angola. Todos os direitos reservados.<br>
    Desenvolvido por: Silvia Simão, Silvina Martins, Simone Zua, Deblá Benjamin. Instituto Médio Comercial de Luanda, 12ª Classe, Curso de Informática de Gestão.
  </footer>

  <script>
    const textos = {
      pt: {
        titulo: "História de Angola",
        nav1: "Pré-Colonial",
        nav2: "Colonial",
        nav3: "Independência",
        nav4: "Pós-Independência",
        "pre-colonial-text": "Antes da chegada dos colonizadores, Angola era habitada por diversos grupos étnicos com estruturas sociais, políticas e económicas próprias. Reinos como o do Congo, Ndongo e Lunda tinham sistemas de governo organizados e culturas ricas.",
        "colonial-text": "A colonização portuguesa iniciou-se no século XV e intensificou-se nos séculos seguintes. Houve resistência por parte dos povos locais, mas Portugal consolidou o seu domínio, explorando recursos e impondo o seu controlo administrativo e cultural.",
        "independencia-text": "Angola conquistou a sua independência de Portugal a 11 de novembro de 1975, após anos de luta armada liderada por movimentos como o MPLA, FNLA e UNITA. A independência foi um marco importante, mas seguiu-se um longo período de guerra civil.",
        "pos-independencia-text": "Após o fim da guerra civil em 2002, Angola iniciou um processo de reconstrução nacional. Investimentos em infraestrutura, educação e saúde foram intensificados, embora desafios sociais e económicos ainda persistam."
      },
      en: {
        titulo: "History of Angola",
        nav1: "Pre-Colonial",
        nav2: "Colonial",
        nav3: "Independence",
        nav4: "Post-Independence",
        "pre-colonial-text": "Before the arrival of colonizers, Angola was inhabited by various ethnic groups with their own social, political, and economic structures. Kingdoms like Congo, Ndongo, and Lunda had organized governments and rich cultures.",
        "colonial-text": "Portuguese colonization began in the 15th century and intensified over the following centuries. Local populations resisted, but Portugal consolidated its control, exploiting resources and imposing its administrative and cultural dominance.",
        "independencia-text": "Angola gained independence from Portugal on November 11, 1975, after years of armed struggle led by movements such as MPLA, FNLA, and UNITA. The independence marked a major milestone, followed by a long civil war.",
        "pos-independencia-text": "After the end of the civil war in 2002, Angola began a process of national reconstruction. Investments in infrastructure, education, and healthcare increased, though social and economic challenges remain."
      },
      fr: {
        titulo: "Histoire de l'Angola",
        nav1: "Pré-colonial",
        nav2: "Colonial",
        nav3: "Indépendance",
        nav4: "Post-Indépendance",
        "pre-colonial-text": "Avant l'arrivée des colonisateurs, l'Angola était peuplé de divers groupes ethniques ayant leurs propres structures sociales, politiques et économiques. Des royaumes comme le Congo, le Ndongo et le Lunda avaient des gouvernements organisés et des cultures riches.",
        "colonial-text": "La colonisation portugaise a commencé au XVe siècle et s'est intensifiée par la suite. Les populations locales ont résisté, mais le Portugal a consolidé son contrôle en exploitant les ressources et en imposant sa domination administrative et culturelle.",
        "independencia-text": "L'Angola a obtenu son indépendance du Portugal le 11 novembre 1975, après des années de lutte armée menée par des mouvements tels que le MPLA, le FNLA et l'UNITA. L'indépendance fut un jalon majeur, suivi d'une longue guerre civile.",
        "pos-independencia-text": "Après la fin de la guerre civile en 2002, l'Angola a entamé un processus de reconstruction nationale. Les investissements dans les infrastructures, l'éducation et la santé ont augmenté, bien que des défis sociaux et économiques subsistent."
      },
      es: {
        titulo: "Historia de Angola",
        nav1: "Precolonial",
        nav2: "Colonial",
        nav3: "Independencia",
        nav4: "Post-Independencia",
        "pre-colonial-text": "Antes de la llegada de los colonizadores, Angola estaba habitada por diversos grupos étnicos con estructuras sociales, políticas y económicas propias. Reinos como Congo, Ndongo y Lunda tenían gobiernos organizados y culturas ricas.",
        "colonial-text": "La colonización portuguesa comenzó en el siglo XV y se intensificó en los siglos siguientes. Las poblaciones locales resistieron, pero Portugal consolidó su control, explotando recursos e imponiendo su dominio administrativo y cultural.",
        "independencia-text": "Angola obtuvo su independencia de Portugal el 11 de noviembre de 1975, tras años de lucha armada liderada por movimientos como el MPLA, FNLA y UNITA. La independencia marcó un hito importante, seguido de una larga guerra civil.",
        "pos-independencia-text": "Tras el fin de la guerra civil en 2002, Angola inició un proceso de reconstrucción nacional. Aumentaron las inversiones en infraestructura, educación y salud, aunque persisten desafíos sociales y económicos."
      }
    };

    function mudarIdioma(idioma) {
      const t = textos[idioma];
      if (!t) return;

      document.getElementById("titulo").textContent = t.titulo;
      document.getElementById("nav1").textContent = t.nav1;
      document.getElementById("nav2").textContent = t.nav2;
      document.getElementById("nav3").textContent = t.nav3;
      document.getElementById("nav4").textContent = t.nav4;
      document.getElementById("pre-colonial-text").textContent = t["pre-colonial-text"];
      document.getElementById("colonial-text").textContent = t["colonial-text"];
      document.getElementById("independencia-text").textContent = t["independencia-text"];
      document.getElementById("pos-independencia-text").textContent = t["pos-independencia-text"];
    }
  </script>
</body>
</html>

   
  
     
