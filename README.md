<!DOCTYPE html> 
<html lang="pt-br">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="shortcut icon" href="favicon.ico" type="image/x-icon">
    <link rel="stylesheet" href="style.css">
    <title>New & Used Eletric Cars | Tesla</title>
</head>

<body>
    <img src="imagens/logo.png" alt="Logo da tesla" class="logo">

    <!--Item 1-->
    <li class="item">
        <video src="imagens/model-y.mp4" autoplay loop muted></video>

        <div class="info-carro">
            <h1>Model Y</h1>
            <p class="subtt">Parcelas a partir de 399 doláres</p>
        </div>

        <div class="rodape">
            <button>Comprar agora</button>
            <button class="test-drive">Faça um teste drive</button>
            <p class="texto-rdp">Não garantimos seu veículo imediatamente. Consultar estoque</p>
        </div>

        <!--Item 2-->
    </li>
    <li class="item">
        <img src="imagens/model-x.png" alt="Tesla Model-X" class="img-tesla">

        <div class="info-carro">
            <h1>Model X</h1>
            <p class="subtt">Parcelas a partir de 329 doláres</p>
        </div>
    </li>
    <!--Item 3-->
    <li class="item">
        <img src="imagens/model-3.png" alt="Tesla Model-3" class="img-tesla">

        <div class="info-carro">
            <h1 class="info-carro2">Model X</h1>
            <p class="subtt2">Parcelas a partir de 499 doláres</p>
        </div>
    </li>

    <div class="formulario">
        <script type="text/javascript" src="https://form.jotform.com/jsform/241935949111056"></script>
    </div>    
</body>
@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');

* {
    font-family: "Poppins", sans-serif;
    margin: 0; /* espaçamento externo */
    padding: 0; /* espaçamento interno */
    box-sizing: border-box; 
}
/* * asterísco significa TUDO, ele vai aplicar esse estilo para tudo */

html {
    scroll-snap-type: y mandatory;
}

video, .img-tesla {
     width: 100%; /* LARGURA */
     height: 100%; /* ALTURA */
     position: absolute; /* POSICIONAR O ITEM NUMA POSIÇÃO EXATA QUE EU DESEJAR */
     top: 0;
     left: 0;
     z-index: -1; /* DEFINE QUEM FICA NA FRENTE DE QUEM */
     object-fit: cover;/* FAZ COM QUE O VIDEO CUBRA TODA A TELA  */
     filter: brightness(60%);
}
 
.logo {
    filter: brightness(100);
    position: fixed;
    width: 120px;
}

.item {
    display: flex; /* HABILITA ALGUMAS PROPRIEDADES CSS */

    justify-content: space-between; /* CRIA UM ESPAÇAMENTO ENTRE OS ITENS */
    flex-direction: column; /* DEIXAR UM ITEM DEBAIXO DO OUTRO */

    position: relative;
    height: 100vh; /* TELA TODA - ALTURA */
    width: 100vw; /* TELA TODA - LARGURA */
    scroll-snap-align: start;
}

h1 {
    color: white;
    font-size: 50px;
}

.subtt {
    color: white;
}

.subtt2 {
    color: black;
}

.info-carro {
    margin-top: 80px;
    text-align: center;
}

.info-carro2{
    color: black;
}

.rodape {
    text-align: center; /* ALINHA MEU ITEM AO CENTRO */
}

button {
    background-color: rgba(34, 34, 34, 0.8);
    color: white;
    padding: 7px 80px;
    border-radius: 5px; /* ARREDONDA A BORDA DO BOTÃO */
    border: none; /* TIRA A BORDA DO BOTÃO */
    cursor: pointer; /* COLOCA A MÃOSINHA NO LUGAR DO MOUSE */
}

.test-drive {
    color: black;
    background-color: white;
}

.texto-rodape {
    color: white;
    font-size: 12px; /* TAMANHO DO TEXTO */
    margin-top: 10px;
}

.formulario {
    position: fixed;
    top: 40px;
    width: 600px;
    height: 100%;
    z-index: 3;
    left: -50%;
    transition: 1.5s;
}
    <script src="scripts.js"></script>
</html>
