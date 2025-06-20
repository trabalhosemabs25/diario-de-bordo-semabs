
<!DOCTYPE html>
<html lang="pt-br">
 <head>
  <style>
   /* ... estilos já existentes ... */

  @media (max-width: 576px) {
    /* Ajuste do main */
    main {
      margin: 1rem;
      padding: 1rem;
    }

    /* Redução de fontes */
    header h1 {
      font-size: 1.5rem;
    }

    header p {
      font-size: 0.95rem;
    }

    h2 {
      font-size: 1.3rem;
    }

    p {
      font-size: 0.95rem;
    }

    /* Splash screen adaptado */
    #splash div {
      max-width: 90%;
      padding: 1.5rem;
    }

    #splash button {
      width: 100%;
      font-size: 1rem;
    }
  }

  @media (max-width: 768px) {
    nav {
      flex-direction: column;
      align-items: center;
      background: var(--secondary-color);
      gap: 0.5rem;
    }

    nav a {
      width: 100%;
      text-align: center;
      padding: 1rem 0;
      font-size: 1rem;
    }

    .menu-toggle {
      margin-top: 1rem;
    }
  }
  </style>
  <link crossorigin="anonymous" href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.6/dist/css/bootstrap.min.css" integrity="sha384-4Q6Gf2aSP4eDXB8Miphtr37CMZZQ5oXLH2yaXMJ2w8e2ZtHTl7GptT4jmndRuHDT" rel="stylesheet"/>
  <!-- Tela de apresentação com integrantes -->
  <div id="splash" style="
  position: fixed;
  top: 0;
  left: 0;
  width: 100vw;
  height: 100vh;
  background-color: rgba(0, 0, 0, 0.7);
  display: flex;
  align-items: center;
  justify-content: center;
  z-index: 10000;
">
   <div style="
    background: white;
    border-radius: 20px;
    padding: 2rem;
    text-align: center;
    max-width: 300px;
    box-shadow: 0 10px 20px rgba(0,0,0,0.3);
    animation: fadeIn 1s ease;
  ">
    <h2 style="color: #4a148c; margin-bottom: 1rem;">
     Integrantes
    </h2>
    <ul style="list-style: none; padding: 0; font-size: 1rem; color: #333;">
     <li>
      Alexsandro nunes
     </li>
     <li>
      Francisco gabriel
     </li>
     <li>
      Gabriel silva lopes
     </li>
     <li>
      Joao Fernado pereira
     </li>
     <li>
      kleverson soares
     </li>
     <li>
      murilo de oliveira
     </li>
    </ul>
    <button onclick="document.getElementById('splash').style.display='none'" style="
      margin-top: 1.5rem;
      padding: 0.5rem 1rem;
      background-color: #7b1fa2;
      color: rgb(255, 255, 255);
      border: none;
      border-radius: 8px;
      cursor: pointer;
      transition: background-color 0.3s ease;
    ">
     Entrar
    </button>
   </div>
  </div>
  <style>
   @keyframes fadeIn {
  from { opacity: 0; transform: scale(0.9); }
  to { opacity: 1; transform: scale(1); }
}
  </style>
  <script>
   // Fecha automaticamente após alguns segundos (opcional)
  setTimeout(() => {
    const splash = document.getElementById('splash');
    if (splash) splash.style.display = 'none';
  }, 8000);
  </script>
  <meta charset="utf-8"/>
  <meta content="width=device-width, initial-scale=1.0" name="viewport"/>
  <title>
   Diário de Bordo Virtual
  </title>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&amp;display=swap" rel="stylesheet"/>
  <link href="adal_high_quality.png" rel="icon" type="image/png"/>
  <style>
   :root {
      --primary-color: #000000;
      --secondary-color: #7b1fa2;
      --accent-color: #ba68c8;
      --background-light: #f3e5f5;
      --text-dark: #2e2e2e;
    }
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }
    html, body {
      height: 100%;
    }
    body {
      font-family: 'Poppins', sans-serif;
      color: var(--text-dark);
      background: linear-gradient(-45deg, #f3e5f5, #e1bee7, #ce93d8, #ba68c8);
      background-size: 400% 400%;
      animation: gradientWave 15s ease infinite;
      scroll-behavior: smooth;
    }
    .logo-canto {
      position: fixed;
      top: 10px;
      left: 10px;
      width: 50px;
      height: auto;
      z-index: 9999;
    }
    header {
      background: linear-gradient(135deg, #000000, #000000, #000000);
      background-size: 600% 600%;
      animation: wave 10s ease infinite;
      color: white;
      text-align: center;
      padding: 3rem 1rem 2rem;
      box-shadow: 0 4px 6px rgba(0, 0, 0, 0.3);
    }
    header h1 {
      font-size: 2.5rem;
      margin-bottom: 0.5rem;
    }
    header p {
      font-size: 1.1rem;
    }
    .menu-toggle {
      display: none;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      width: 40px;
      height: 40px;
      margin: 1rem auto;
      cursor: pointer;
      z-index: 9999;
    }
    .menu-toggle span {
      width: 30px;
      height: 4px;
      background: white;
      margin: 4px 0;
      border-radius: 2px;
    }
    nav {
      background: var(--secondary-color);
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 1rem;
      padding: 1rem;
      position: sticky;
      top: 0;
      z-index: 999;
    }
    nav a {
      color: white;
      text-decoration: none;
      font-weight: 600;
      padding: 0.5rem 1rem;
      border-radius: 6px;
      background-color: rgba(255,255,255,0.1);
      transition: all 0.3s ease;
    }
    nav a:hover {
      background-color: rgba(255,255,255,0.3);
      transform: scale(1.05);
    }
    main {
      max-width: 960px;
      margin: 2rem auto;
      padding: 2rem;
      background: white;
      border-radius: 16px;
      box-shadow: 0 10px 25px rgba(0,0,0,0.1);
    }
    section.entry {
      margin-bottom: 2rem;
      padding: 1rem 1.5rem;
      border-left: 4px solid var(--accent-color);
      background: #fafafa;
      border-radius: 10px;
      transition: transform 0.3s;
    }
    section.entry:hover {
      transform: translateY(-3px);
      box-shadow: 0 6px 12px rgba(0,0,0,0.1);
    }
    h2 {
      color: var(--primary-color);
      font-size: 1.6rem;
      margin-bottom: 0.3rem;
    }
    .date {
      font-size: 0.9rem;
      color: #666;
      margin-bottom: 0.8rem;
    }
    p {
      font-size: 1rem;
      line-height: 1.6;
    }
    .scroll-top {
      position: fixed;
      bottom: 20px;
      right: 20px;
      background: var(--primary-color);
      color: white;
      padding: 10px 15px;
      border: none;
      border-radius: 50%;
      font-size: 20px;
      cursor: pointer;
      box-shadow: 0 4px 10px rgba(0,0,0,0.2);
      display: none;
    }
    .scroll-top:hover {
      background: var(--secondary-color);
    }
    footer {
      text-align: center;
      padding: 2rem 1rem;
      background: var(--primary-color);
      color: white;
      margin-top: 3rem;
      font-size: 0.9rem;
    }
    @media (max-width: 768px) {
      .menu-toggle {
        display: flex;
      }
      nav {
        display: none;
        flex-direction: column;
        align-items: center;
        position: absolute;
        top: 70px;
        width: 100%;
        left: 0;
      }
      nav.active {
        display: flex;
      }
    }
    @keyframes gradientWave {
      0% { background-position: 0% 50%; }
      50% { background-position: 100% 50%; }
      100% { background-position: 0% 50%; }
    }
    @keyframes wave {
      0% { background-position: 0% 50%; }
      50% { background-position: 100% 50%; }
      100% { background-position: 0% 50%; }
    }
  </style>
 </head>
 <body>
  <img alt="Logo Escola" class="logo-canto" src="adal_high_quality.png"/>
  <div class="menu-toggle" onclick="document.querySelector('nav').classList.toggle('active')">
   <span>
   </span>
   <span>
   </span>
   <span>
   </span>
  </div>
  <header>
   <h1>
    Diário de Bordo Virtual
   </h1>
   <p>
    Registre aqui as etapas, decisões e aprendizados do seu projeto.
   </p>
  </header>
  <nav>
   <a href="#entrada1">
    02/06
   </a>
   <a href="#entrada2">
    04/06
   </a>
   <a href="#entrada3">
    05/06
   </a>
   <a href="#entrada4">
    06/06
   </a>
   <a href="#entrada5">
    09/06
   </a>
   <a href="#entrada6">
    Outro
   </a>
  </nav>
  <main>
   <section class="entry" id="entrada1">
    <h2>
     02/06/2025
    </h2>
    <p>
     No dia 2 de junho, foi realizada a apresentação detalhada do modelo de aplicação que orientaria o funcionamento da SEMABS. Durante essa apresentação, foram expostos os objetivos principais, as metodologias a serem adotadas, bem como o cronograma de atividades previsto para o desenvolvimento do projeto. A equipe pôde compreender claramente como o processo seria conduzido.
    </p>
   </section>
   <section class="entry" id="entrada2">
    <h2>
     04/06/2025
    </h2>
    <p>
     No dia 4 de junho, durante a aula de Química, ocorreu a escolha oficial da equipe que iria compor o grupo responsável pelo projeto. Essa seleção foi realizada sob a supervisão da professora Nádia.
    </p>
   </section>
   <section class="entry" id="entrada3">
    <h2>
     05/06/2025
    </h2>
    <p>
     No dia 5 de junho, durante a aula ministrada pela professora Colores, responsável pela disciplina NTPPS, foi definido o eixo temático que nortearia a pesquisa do trabalho. A professora Colores forneceu orientações importantes sobre a delimitação do tema e os recursos metodológicos disponíveis, o que facilitou a tomada de decisão.
    </p>
   </section>
   <section class="entry" id="entrada4">
    <h2>
     06/06/2025
    </h2>
    <p>
     No dia 6 de junho, a equipe tomou a decisão de escolher o professor José Marcelo, docente da disciplina de Física, como orientador do projeto. Além disso, nesse mesmo dia, a equipe iniciou a elaboração do caderno de bordo, utilizando um formato inovador inspirado em um site digital, que inclui um QR Code para facilitar o acesso e a divulgação do conteúdo do projeto.
    </p>
   </section>
   <section class="entry" id="entrada5">
    <h2>
     09/06/2025
    </h2>
    <p>
     No dia 9 de junho, nos reunimos com o grupo para dar início, de forma mais concreta, ao desenvolvimento do nosso trabalho sobre educação ambiental.
    </p>
   </section>
   <section class="entry" id="entrada6">
    <h2>
     10/06/2025
    </h2>
    <p>
     No dia 10 de junho, demos continuidade ao desenvolvimento do nosso projeto, com foco especial na criação do diário de bordo em formato digital. Avançamos na estruturação da página, organizando melhor o conteúdo já registrado nos dias anteriores e aprimorando o visual do site, seguimos com a elaboração do relatório, revisando os tópicos já produzidos, ajustando a linguagem e complementando com novas informações relevantes.
    </p>
   </section>
   <section class="entry" id="entrada7">
    <h2>
     11/06/2025
    </h2>
    <p>
     No dia 11 de junho, realizamos uma reunião com alguns integrantes do grupo e com o nosso orientador, professor José Marcelo. Durante o encontro, discutimos o andamento do projeto, trocamos ideias e alinhamos pontos importantes para a próxima etapa. A conversa foi produtiva e nos ajudou a esclarecer dúvidas e reforçar o foco do grupo.
    </p>
   </section>
  </main>
  <button class="scroll-top" onclick="window.scrollTo({top: 0, behavior: 'smooth'})">
   ↑
  </button>
  <footer>
   <p>
    Desenvolvido como parte do projeto educacional da SEMABS 2025
   </p>
  </footer>
  <script>
   window.onscroll = function () {
      const btn = document.querySelector('.scroll-top');
      if (window.scrollY > 200) {
        btn.style.display = 'block';
      } else {
        btn.style.display = 'none';
      }
    }
  </script>
 </body>
</html>
