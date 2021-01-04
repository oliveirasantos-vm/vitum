<template>
  <div id="biography">
    <div class="grid">
      <div class="column-1 row-1 item img childhood item-1"></div>
      <div class="column-2 row-1 item txt r item-2">
        <div class="content">
          Olá, meu nome é Vitor Mateus, mas pode me chamar de vitum. Nasci em
          Gravataí, em 16 de janeiro de 2001, no Rio Grande do Sul, na região
          metropolitana de Porto Alegre. Foi lá, onde passei boa parde da minha
          infância. Desde pequeno sou aficcionado por computadores, ainda lembro
          do meu primeiro computador, ele era branco, meio amarelado, o monitor
          parecia uma televisão antiga, ele era lento e tinha que ter paciência
          para usar, mas, mesmo assim, eu adorava ele.
        </div>
      </div>
      <div class="column-1 row-2 item txt item-3">
        <div class="content">
          Conforme fui crescendo, fui seguindo nessa área. Meu primeiro curso
          foi de Designer Gráfico, depois, Montagem e Manutenção de Computadores
          seguido por Manutenção de Notebook, aí então veio o meu Ensino Médio
          Integrado ao Curso Técnico em Informática. Me formei em 4 anos, sendo
          destaque nas disciplinas técnicas. Fui gratificado como orador da
          turma, onde pude homenagear os colegas, professores e servidores do
          Instituto Federal do Rio Grande do Sul - Campus Osório.
        </div>
      </div>
      <div class="column-2 row-2 item item-4">
        <div class="img">
          <iframe
            id="video"
            src="https://www.youtube.com/embed/c1QXJSvbVUU"
            frameborder="0"
            allowfullscreen
          ></iframe>
        </div>
      </div>
      <div class="column-1 row-3 item img carrer item-5"></div>
      <div class="column-2 row-3 item txt item-6">
        <div class="content">
          Durante meus estudos, iniciei minha carreira no mercado de trabalho.
          Fui estagiário na WebSul Telecom LTDA, uma provedora de internet do
          litoral norte, onde atuava como suporte técnico. Depois trabalhei como
          estagiário no Departamento de Tecnologia da Informação da Prefeitura
          Municipal de Osório. Logo depois, quando me formei, trabalhei como Web
          Designer na Raizler Magnéticos, muito conhecida por ser a maior
          empresa de ímãs de geladeira do Brasil.
        </div>
      </div>
      <div class="column-1 row-4 item txt item-7">
        <div class="content">
          Hoje estou habilitado para desenvolver aplicações web, tanto
          front-end, com HTML, CSS e JavaScript, como back-end, com MySQL e
          Nodejs. Além de conhecimento avançado em Designer Gráfico, sabendo
          utilizar as ferramentas de edição de imagem e vetor. Também tenho
          facilidade em aprender coisas novas, esse site por exemplo, está sendo
          desenvolvido em vue.js, acredita que eu nem conhecia esse framework
          antes? Enfim, hoje estou disponível no mercado de trabalho, mas quem
          sabe amanhã eu esteja trabalhando na sua empresa!
        </div>
      </div>
      <div class="column-2 row-4 item img future item-8"></div>
    </div>
  </div>
</template>

<style scoped>
#biography {
  background-image: url("../assets/biography-bg.svg");
  background-size: 1091px 1200px;
  background-color: #f0f7d4;
  color: #110934;
  background-position: center;
  background-repeat: no-repeat;
  text-align: justify;
}
.grid {
  display: grid;
  grid-template-rows: 300px 300px 300px 300px;
  grid-template-columns: 1fr 1fr;
  grid-column-gap: 30px 30px;
  align-items: center;
  padding: 50px 100px 50px 100px;
}
.item {
  position: relative;
  height: 300px;
  align-items: center;
}

.carrer {
  width: 70%;
  height: 220px;
  margin-top: 40px;
  margin-bottom: 40px;
  margin-left: 15%;
  margin-right: 15%;
  background-image: url("../assets/carrer.jpg");
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
}

.content {
  position: absolute;
  left: 0;
  right: 0;
  width: 100%;
  bottom: 0;
}
.column-1 {
  grid-column: 1;
}
.column-2 {
  grid-column: 2;
}
.row-1 {
  grid-row: 1;
}
.row-2 {
  grid-row: 2;
}
.row-3 {
  grid-row: 3;
}
.row-4 {
  grid-row: 4;
}
.img {
  left: 0;
  right: 0;
  border-radius: 10px;
}
#video {
  width: 70%;
  height: 220px;
  margin-top: 40px;
  margin-bottom: 40px;
  margin-left: 15%;
  margin-right: 15%;
}
.childhood {
  width: 70%;
  height: 220px;
  margin-top: 40px;
  margin-bottom: 40px;
  margin-left: 15%;
  margin-right: 15%;
  background-image: url("../assets/childhood.jpg");
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
}

.future {
  width: 70%;
  height: 220px;
  margin-top: 40px;
  margin-bottom: 40px;
  margin-left: 15%;
  margin-right: 15%;
  background-image: url("../assets/future.png");
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
}


@media (max-width: 768px) {
  #biography {
    position: relative;
    background-image: url("../assets/biography-bg-mobile.svg");
    background-size: 280px 3072px;
    background-color: #f0f7d4;
    color: #110934;
    height: 3072px;
    background-repeat: no-repeat;
    text-align: justify;
    font-size: 14px;
  }
  .grid {
    position: relative;
    display: grid;
    grid-template-rows: 512px 256px 512px 256px 512px 256px 512px 256px;
    grid-template-columns: 1fr;
    grid-column-gap: 0px;
    grid-row-gap: 0px;
    align-items: center;
    padding: 10px 20px 10px 10px;
  }
  .item-1 {grid-row: 2; }
  .item-2 {grid-row: 1;}
  .item-3 {grid-row: 3;}
  .item-4 {grid-row: 4; }
  .item-5 {grid-row: 6;}
  .item-6 {grid-row: 5;}
  .item-7 {grid-row: 7;}
  .item-8 {grid-row: 8;}
  .row-1 {grid-row: 0;}
  .row-2 {grid-row: 0;}
  .row-3 {grid-row: 0;}
  .row-4 {grid-row: 0;}
  
  .txt{
    position: relative;
  }
  .content {
    position: absolute;
    left: 0;
    right: 0;
    width: 100%;
    bottom: 0;;
  }
  .column-1 {
    grid-column: 1;
  }
  .column-2 {
    grid-column: 1;
  }
  .img {
    position: relative;
    width: 100%;
    height: 75%;
    margin-bottom: 25%;
    margin-left: 0; margin-right: 0;
    border-radius: 10px;
  }
  
  .childhood {
    background-image: url("../assets/childhood.jpg");
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
  }
  .carrer {
    background-image: url("../assets/carrer.jpg");
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
  }
  #video {
    width: 100%;
    height: 75%;
    margin-bottom: 25%;
    margin-left: 0; margin-right: 0;
    border-radius: 10px;
  }
  .future {
    background-image: url("../assets/future.png");
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
  }
}
@media (min-width: 769px) and (max-width: 1116px) {
}
@media (min-width: 769px) and (max-width: 1116px) {
}
@media (min-width: 769px) and (max-width: 1116px) {
}
</style>