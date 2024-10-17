# mirella-alura-parte-2
@@ -240,6 +240,81 @@ <h2 class="contato__titulo">Fique por dentro das novidades!</h2>

  <footer class="rodapé">
    <h2 class="rodapé__titulo">Grupo Alura</h2>
    <ul class="lista-rodapé">
      <li class="lista-rodapé__titulo">Educação</li>
      <li class="lista-rodapé__item">
        <img src="img/Caelum.svg" alt="Logo da Caelum" />
        <a href="#" class="lista-rodapé__link">Caelum</a>
      </li>
      <li class="lista-rodapé__item">
        <img src="img/CasaDoCodigo.svg" alt="Logo da Casa do Código" />
        <a href="#" class="lista-rodapé__link">Casa do Código</a>
      </li>
    </ul>
    <ul class="lista-rodapé">
      <li class="lista-rodapé__titulo">Educação online</li>
      <li class="lista-rodapé__item">
        <img src="img/Alura.svg" alt="Logo da Alura" />
        <a href="#" class="lista-rodapé__link">Alura</a>
      </li>
      <li class="lista-rodapé__item">
        <img src="img/AluraEmpresas.svg" alt="Logo da AluraParaEmpresas" />
        <a href="#" class="lista-rodapé__link">Alura para Empresas</a>
      </li>
      <li class="lista-rodapé__item">
        <img src="img/AluraLATAM.svg" alt="Logo da Alura Latam" />
        <a href="#" class="lista-rodapé__link">Alura LATAM</a>
      </li>
      <li class="lista-rodapé__item">
        <img src="img/AluraStart.svg" alt="Logo da Alura START" />
        <a href="#" class="lista-rodapé__link">Alura Start</a>
      </li>
      <li class="lista-rodapé__item">
        <img src="img/MusicDot.svg" alt="Logo da Music Dot" />
        <a href="#" class="lista-rodapé__link">Music Dot</a>
      </li>
      <li class="lista-rodapé__item">
        <img src="img/AluraLingua.svg" alt="Logo da Alura Lingua" />
        <a href="#" class="lista-rodapé__link">Alura Língua</a>
      </li>
      <li class="lista-rodapé__item">
        <img src="img/PM3.svg" alt="Logo da PM3" />
        <a href="#" class="lista-rodapé__link">PM3</a>
      </li>
    </ul>
    <ul class="lista-rodapé">
      <li class="lista-rodapé__titulo">Comunidade</li>
      <li class="lista-rodapé__item">
        <img src="img/HipstersTech.svg" alt="Logo do Hipsters ponto Tech" />
        <a href="#" class="lista-rodapé__link">Hipsters ponto Tech</a>
      </li>
      <li class="lista-rodapé__item">
        <img src="img/ScubaDev.svg" alt="Logo do Scuba Dev" />
        <a href="#" class="lista-rodapé__link">Scuba Dev</a>
      </li>
      <li class="lista-rodapé__item">
        <img src="img/LayersTech.svg" alt="Logo do Layers ponto Tech" />
        <a href="#" class="lista-rodapé__link">Layers ponto Tech</a>
      </li>
      <li class="lista-rodapé__item">
        <img src="img/LikeABoss.svg" alt="Logo do Like a Boss" />
        <a href="#" class="lista-rodapé__link">Like a Boss</a>
      </li>
      <li class="lista-rodapé__item">
        <img src="img/CarreiraSemFronteira.svg" alt="Logo do Carreira sem fronteiras" />
        <a href="#" class="lista-rodapé__link">Carreira sem fronteiras</a>
      </li>
      <li class="lista-rodapé__item">
        <img src="img/HipstersJobs.svg" alt="Logo do Hipsters ponto jobs" />
        <a href="#" class="lista-rodapé__link">Hipsters ponto jobs</a>
      </li>
      <li class="lista-rodapé__item">
        <img src="img/GUJ.svg" alt="Logo do GUJ" />
        <a href="#" class="lista-rodapé__link">GUJ</a>
      </li>
    </ul>
  </footer>

  <script src="https://cdn.jsdelivr.net/npm/swiper@11/swiper-bundle.min.js"></script>
‎styles.css
+2
Original file line number	Diff line number	Diff line change
@@ -15,6 +15,8 @@
    --azul: #002F52;
    --fonte-secundario: "Josefin Sans";
    --preto: #000000;
    --cinza: #474646;
    --cinza-claro: #858585;
}

body {
‎styles/rodapé.css
+37
Original file line number	Diff line number	Diff line change
@@ -5,4 +5,41 @@ hr {
.rodapé {
    background-color: var(--branco);
    padding: 1em;
}
.lista-rodapé {
    display: none;
}
@media screen and (min-width: 1024px) {
    .rodapé {
        display: flex;
        justify-content: space-around;
    }
    .lista-rodapé {
        display: block;
    }
    .lista-rodapé__item {
        display: flex;
        align-items: center;
        margin: 0.6em 0;
    }
    .lista-rodapé__link {
        color: var(--cinza);
        text-decoration: none;
        margin-left: 0.6em;
    }
    .lista-rodapé__titulo {
        font-size: 14px;
        color: var(--cinza-claro);
    }
    .rodapé__titulo {
        font-size: 24px;
    }
}
