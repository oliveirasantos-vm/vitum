<template>
  <nav class="navtop">
    <input type="checkbox" id="check" />
    <label for="check" class="checkbtn">
      <i class="fas fa-bars"></i>
    </label>
    <label class="logo"
      ><a href="/"
        ><img src="../assets/logo-light.svg" alt="logo-light.svg" /></a
    ></label>
    <ul class="nav-items">
      <li><a href="/biografia">Biografia</a></li>
      <li><a href="/anunciar">Formação</a></li>
      <li><a href="/buscar">Serviços</a></li>
      <li><a href="/contato">Contato</a></li>
      <li>
        <a href="https://github.com/oliveirasantos-vm"
          ><i class="fab fa-github"></i
        ></a>
      </li>
    </ul>
  </nav>
</template>

<script>
export default {};
</script>

<style scoped>
* {
  padding: 0;
  margin: 0;
  text-decoration: none;
  list-style: none;
  box-sizing: border-box;
}

.navtop {
  background: #110934;
  height: 70px;
  width: 100%;
}

.logo img {
  height: 35px;
  float: left;
  margin: 17.5px 30px 17.5px 30px;
}

.nav-items {
  float: right;
  font-weight: 300;
  margin-right: 35px;
}

.nav-items li {
  display: inline-block;
  line-height: 70px;
  font-size: 17px;
  margin-left: 15px;
  margin-right: 15px;
}

a {
  text-decoration: none;
  color: #dcdcdc;
}

a.active,
a:hover {
  color: #f0f7d4;
}

.checkbtn {
  font-size: 30px;
  color: #f0f7d4;
  float: right;
  line-height: 70px;
  margin-right: 40px;
  cursor: pointer;
  display: none;
}

#check {
  display: none;
}

@media (max-width: 858px) {
  .checkbtn {
    display: block;
  }
  ul {
    position: fixed;
    width: 100%;
    height: 100vh;
    background: #4424d6;
    top: 70px;
    left: -100%;
    text-align: center;
    transition: all 0.5s;
    z-index: 50;
    padding: none;
    margin: none;
  }
  .nav-items li {
    display: inline-block;
    line-height: 70px;
    font-size: 17px;
    margin-left: 0px;
    margin-right: 0px;
  }
  nav ul li {
    line-height: 30px;
  }
  nav ul li a {
    display: block;
    font-size: 20px;
    font-weight: 300;
  }
  li {
    width: 100%;
  }
  a:active,
  a:hover {
    color: #f0f7d4;
  }
  #check:checked ~ ul {
    left: 0;
  }
}
</style>