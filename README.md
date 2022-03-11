<!DOCTYPE html>
<html lang="pt-br">

<head>
  <meta charset="UTF-8">
  <title>Barbearia Alura</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link rel="stylesheet" href="reset.css">
  <link rel="stylesheet" href="style.css">
  <link rel="icon" href="logo.png">
  <link href="https://fonts.googleapis.com/css?family=Montserrat&display=swap" rel="stylesheet">
  
  <style>
  /* css pagina home */

body {
	font-family: 'Montserrat', sans-serif;
}

.banner {
  width: 100%;
}



.titulo-principal {
	text-align: center;
	font-size: 2em;
	margin: 0 0 1em;
	clear: left;
	text-shadow: 1px 1px 3px #000000;
}

.titulo-principal:first-letter {
	font-weight: bold;
}

.titulo-principal:before {
	content: "[ ";
}

.titulo-principal:after {
	content: " ]";
}

.principal, .formulario {
	padding: 3em 0;
	background: #fefefe;
}

.principal-texto, .formulario {
	width: 940px;
	margin: 0 auto;
}

.principal p {
	margin: 0 0 1em;
	font-size: 20px;
	text-align: justify;
}

.principal strong {
	font-weight: bold;
}

.principal em {
	font-style: italic;
}

.utensilios {
	width: 150px;
	float: left;	
	margin: 0 20px 20px 0;
}

.beneficios {
	padding: 3em 0;
	background: #888888;
}

.conteudo-beneficios {
	width: 640px;
	margin: 0 auto;
}

.imagem-beneficios {
	width: 60%;
	opacity: 0.5;
	transition: 400ms;
	box-shadow: 10px 10px 10px #000000;
}

.imagem-beneficios:hover {
	opacity: 1;
}

.lista-beneficios {
	width: 40%;
	display: inline-block;
	vertical-align: top;
}

.itens {
	line-height: 1.5;
}

.itens:before {
	content: "\1F488";
}

.itens:nth-child(1) {
	font-weight: bold;
}

/*vai tomar no cu*/

header {
	background: #BBBBBB;
	padding: 20px 0;
}

.caixa {
	position: relative;
	width: 940px;
	margin: 0 auto;
}

nav {
	position: absolute;
	top: 110px;
	right: 0;
}

nav li {
	display: inline;
	margin: 0 0 0 15px;
}

nav a {
	text-transform: uppercase;
	color: #000000;
	font-weight: bold;
	font-size: 22px;
	text-decoration: none;
}

nav a:hover {
	color: #C78C19;
	text-decoration: underline;
}

.produtos {
	width: 940px;
	margin: 0 auto;
	padding: 50px 0;
}

.produtos li {
	display: inline-block;
	text-align: center;
	width: 30%;
	vertical-align: top;
	margin: 0 1.5%;
	padding: 30px 20px;
	box-sizing: border-box;
	border: 2px solid #000000;
	border-radius: 10px;
}

.produtos li:hover {
	border-color: #C78C19;
}

.produtos li:active {
	border-color: #088C19;	
}

.produtos li:hover h2 {
	font-size: 30px;
}

.produtos h2 {
	font-size: 28px;
	font-weight: bold;
}

.produto-descricao {
	font-size: 18px;
}

.produto-preco {
	font-size: 22px;
	font-weight: bold;
	margin-top: 10px;
}

footer {
	text-align: center;
	background: url(bg.jpg);
	padding: 40px 0;
}

.copyright {
	color: #FFFFFF;
	font-size: 13px;
	margin: 20px 0 0;
}

/* Página de contato */
.contato {
	width: 940px;
	margin: 40px auto;
}

.contato label, .input-group legend {
	display: block;
	margin: 0 0 5px;
	font-size: 20px;
}

.campo-padrao, textarea {
	display: block;
	margin: 0 0 30px;
	padding: 10px 20px;
	width: 50%;
	border: 1px solid #aaa;
}

.input-group {
	margin: 0 0 20px;
}

.newsletter {
	margin: 0 0 20px;
}

.botao {
	margin: 20px 0 0;
	width: 30%;
	padding: 10px 20px;
	font-size: 24px;
	display: inline-block;
	background: orange;
	color: white;
	border: none;
	border-radius: 5px;
	transition: 1s;
}

.botao:hover {
	cursor: pointer;
	transform: scale(1.2);	
}

table {
	margin: 10px 0 0;
}

th  {
	background: #777777;
	color: #FFFFFF;
}


td, th {
	border: 1px solid #000000;
	padding: 5px 20px;
}

form {
	margin: 40px 0;
}

form label, form legend {
	display: block;
	font-size: 20px;
	margin: 0 0 10px;
}

.input-padrao {
	display: block;
	margin: 0 0 20px;
	padding: 10px 25px;
	width: 50%;
}

.checkbox, .select {
	margin: 20px 0;
}

.horario, .tabela {
	margin-top: 20px;
}

thead, tfoot {
	text-align: center;
	background-color: #555555;
	color: #FFFFFF;
	font-weight: bold;
}

td, th {
	border: 1px solid #000000;
	padding: 8px 15px;
}

.enviar {
	width: 40%;
	padding: 15px 0;
	background: orange;
	color: #FFFFFF;
	font-weight: bold;
	font-size: 18px;
	border: none;
	border-radius: 5px;
	transition: 1s;
}

.enviar:hover {
	background: red;
	transform: scale(1.2) rotate(-5deg);
}

.enviar:active {
	background: #088C19;
	transition: 1s all;
	transform: scale(1.2) rotate(360deg);

}

.mapa {
	padding: 3em 0;
	background: linear-gradient(#fefefe, #888888);
}

/*caso quisesse fazer redondo faria background: radial-gradient(#fefefe, #888888)
ou se quisesse fazer com mais cores colocaria background: linear-gradient(#fefefe, #888888, red, black) e posso colocar as porcentagens nas cores... */

.mapa-conteudo {
	width: 940px;
	margin: 0 auto;
	box-shadow: 10px 10px 10px #888888;
}

.mapa p {
	margin: 0 0 2em;
	text-align: center;
}

.video {
	width: 560px;
	margin: 2em auto;
	box-shadow: 10px 10px 10px #000000;
	opacity: 0.5;
	transition: 400ms;
}

.video:hover {
	opacity: 1;
}

main, .formulario {
	background: linear-gradient(#fefefe 75%, #888888);
}

@media screen and (max-width: 480px) {
	.caixa, .principal, .principal-texto, .conteudo-beneficios, .mapa-conteudo, .video {
		width: auto;
	}

	h1 {
		text-align: center;
	}

	nav {
		position: static;
	}

	.lista-beneficios, .imagem-beneficios  {
		width: 100%;
	}

	.principal-texto, .lista-beneficios, main {
		margin:0 10px 0 10px;
	}

	.input-padrao, .mensagem, .checkbox {
		width: 19rem;
	}

	.enviar {
		width: 22.3rem;
	}
}

  </style>
  
</head>

<body>
  <header>
    <div class="caixa">
      <a href="index.html">
        <h1><img src="logo.png" class="logo"></h1>
      </a>

      <nav>
        <ul>
          <li><a href="index.html">Home</a></li>
          <li><a href="produtos.html">Produtos</a></li>
          <li><a href="contato.html">Contato</a></li>
        </ul>
      </nav>
    </div>
  </header>

  <img class="banner" src="banner.jpg">

  <main>
    <section class="principal">

      <div class="principal-texto">
        <h2 class="titulo-principal">Sobre a Barbearia Alura</h2>

        <img class="utensilios" src="utensilios.jpg" alt="utensilios de barbeiro">

        <p>Localizada no coração da cidade a <strong>Barbearia Alura</strong> traz para o mercado o
          que há de melhor para o
          seu
          cabelo e barba.
          Fundada em 2019, a Barbearia Alura já é destaque na cidade e conquista novos clientes a cada dia.</p>

        <p id="missao"><em>Nossa missão é: <strong>"Proporcionar auto-estima e qualidade de
              vida aos
              clientes"</strong>.
          </em></p>

        <p>Oferecemos profissionais experientes e antenados às mudanças no mundo da moda. O
          atendimento possui padrão de
          excelência e agilidade, garantindo qualidade e satisfação dos nossos clientes.</p>
      </div>
    </section>

    <section class="mapa">
      <h3 class="titulo-principal">Nosso estabelecimento</h3>
      <p>Nosso estabelecimento está localizado no coração da cidade.</p>

      <div class="mapa-conteudo">
        <iframe
          src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3673.907924930622!2d-47.16758158499163!3d-22.953617845314465!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x94c8b7baad437317%3A0x9f6f277f00fe1e45!2sR.%20Bento%20Rodrigues%20Coelho%2C%2052%20-%20Cidade%20Sat%C3%A9lite%20%C3%8Dris%2C%20Campinas%20-%20SP%2C%2013059-585!5e0!3m2!1spt-BR!2sbr!4v1645564436632!5m2!1spt-BR!2sbr"
          width="100%" height="300" style="border:0;" allowfullscreen="" loading="lazy"></iframe>
      </div>
    </section>

    <section class="beneficios">
      <h3 class="titulo-principal">Benefícios</h3>

      <div class="conteudo-beneficios">
        <ul class="lista-beneficios">
          <li class="itens">Atendimento aos clientes</li>
          <li class="itens">Espaço diferenciado</li>
          <li class="itens">Localização</li>
          <li class="itens">Profissionais qualificados</li>
          <li class="itens">Pontualidade</li>
          <li class="itens">Limpeza</li>
        </ul><img src="beneficios.jpg" class="imagem-beneficios">
      </div>

      <div class="video">
        <iframe width="100%" height="315" src="https://www.youtube.com/embed/GeDbeTjXMiI" title="YouTube video player"
          frameborder="0"
          allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
          allowfullscreen></iframe>
      </div>
    </section>

  </main>

  <footer>
    <a href="index.html">
      <img src="logo-branco.png" class="logo">
    </a>
    <p class="copyright">&copy; Copyright Barbearia Alura - 2022</p>
  </footer>

</body>

</html>
