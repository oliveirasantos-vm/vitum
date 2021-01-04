<template>
  <div class="main">
    <div class="grid-container">
      <div class="text item-a">
        <div id="profession">
          Desenvolvedor <span id="e">&</span> Web Designer
        </div>
        Olá, eu me chamo Vitor Mateus, mas pode me chamar de
        <div class="logo">vitum</div>.
        <div id="biography-btn"><button>Me conheça!</button></div>
      </div>
      <div class="image item-b">
        <img id="me" src="../assets/me.png" alt="me.png" />
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>



<style scoped>
/*area-setting*/
.main {
  
  color: #f0f7d4;
}
.text {
  font-size: 42px;
  font-weight: 300;
  line-height: 70px;
  padding: 90px 70px 90px 70px;
}
.text .logo {
  font-size: 42px;
  color: transparent;
  padding-top: 2px;
  background-image: url("../assets/logo-light.svg");
  background-repeat: no-repeat;
  background-position: center;
  display: inline;
  font-weight: 700;
}
.text #profession {
  font-size: 26px;
  font-weight: 500;
  line-height: 70px;
  color: #fc600a;
}
.text #e {
  color: #b2d732;
}
.text #biography-btn {
  line-height: 150px;
}
.text #biography-btn button {
  background-color: #fc600a;
  font-family: "Work Sans", sans-serif;
  border: none;
  padding: 15px 50px 15px 50px;
  color: #f0f7d4;
  text-align: center;
  text-decoration: none;
  font-size: 22px;
  font-weight: 500;
  border-radius: 2px;
}
.text #biography-btn button:hover {
  box-shadow: 0 12px 16px 0 rgba(0, 0, 0, 0.24),
    0 17px 50px 0 rgba(0, 0, 0, 0.19);
}
#me {
  max-width: 512px;
  margin-bottom: 0;
}

/*grid-setting*/
.grid-container {
    height: 512px;
    background-image: linear-gradient(to bottom right, #110934, #4424d6);
  display: grid;
  grid-template-columns: 1.5fr 1fr;
  grid-template-areas: "column-1 column-2";
}
.item-a {
  grid-area: "column-1";
}
.item-b {
  grid-area: "column-2";
}

@media (max-width: 768px) {
  .main {
    position: relative;
    height: auto;
    background-image: none;
    color: #110934;
  }
  .text {
    font-size: 35px;
    font-weight: 300;
    line-height: 50px;
    text-align: center;
    padding: 30px;
  }
  .text .logo {
    height: 44px;
    color: transparent;
    padding-top: 2px;
    background-image: url("../assets/logo.svg");
    background-repeat: no-repeat;
    background-position: center;
    display: inline;
    font-weight: 700;
  }
  .text #profession {
    font-size: 14px;
    font-weight: 500;
    line-height: 50px;
    color: #fc600a;
  }
  .text #e {
    color: #b2d732;
  }
  .text #biography-btn {
    line-height: 100px;
  }
  .text #biography-btn button {
    background-color: #fc600a;
    font-family: "Work Sans", sans-serif;
    border: none;
    padding: 15px 35px 15px 35px;
    color: #f0f7d4;
    text-align: center;
    text-decoration: none;
    font-size: 20px;
    font-weight: 500;
    border-radius: 2px;
  }
  .text #biography-btn button:hover {
    box-shadow: 0 12px 16px 0 rgba(0, 0, 0, 0.24),
      0 17px 50px 0 rgba(0, 0, 0, 0.19);
  }
  .image {
    text-align: center;
  }
  #me {
    width: 280px;
    height: 280px;
  }

  /*grid-setting*/
  .grid-container {
    display: grid;
    height: min-content;
    grid-auto-rows: 280px auto;
    grid-template-columns: none;
  grid-template-areas: "column-1 column-2";
  }
  
  .item-a {
    grid-row: 2;
    background-color: #f0f7d4;
  }
  .item-b {
    grid-row: 1;
    background-image: linear-gradient(#110934, #4424d6);
  }
}
@media (min-width:769px) and (max-width: 1116px) {
    .text {
    font-size: 32px;
    font-weight: 300;
    line-height: 50px;
    padding: 40px 0px 40px 40px;
    }

  .text .logo {
    height: 42px;
    color: transparent;
    padding-top: 2px;
    background-image: url("../assets/logo-light.svg");
    background-repeat: no-repeat;
    background-position: center;
    display: inline;
    font-weight: 700;
  }
  
  .text #profession {
    font-size: 15px;
    font-weight: 500;
    line-height: 70px;
    color: #fc600a;
  }
  .text #biography-btn {
    line-height: 120px;
  }
  #me {
    height: 448px; 
  }
  .grid-container {
    display: grid;
    grid-auto-rows: 280px auto;
  }
  .grid-container {
    height: 448px;
  display: grid;
  grid-template-columns: 1.5fr 1fr;
  grid-template-areas: "column-1 column-2";
}
  .item-a {
    grid-area: 'column-1';
  }
  .item-b {
    grid-area: 'column-2';
  }
}
</style>