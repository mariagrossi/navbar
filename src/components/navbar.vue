<template>
  <div class="masterDiv">
    <div class="navbar">
      <b-navbar id="navbox" toggleable="md">
        <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
        <b-collapse id="nav-collapse" is-nav>
            <div>
                <!-- Logo -->
                <b-navbar variant="faded" type="light">
                    <b-navbar-brand id="logo" href="#">
                        <img src="../assets/logo.png">
                    </b-navbar-brand>
                </b-navbar>
            </div>
            <b-navbar-nav id ="nav-itens" class="ml-auto">
                <b-nav-item class = "qs" href="#"><u>Quem somos?</u></b-nav-item>
                <b-nav-item class ="proj" href="#">Projetos</b-nav-item>
                <b-nav-item class = "cont" href="#">Contato</b-nav-item>

                <form>
                  <input type="text" name="search" placeholder="Pesquisar">
                </form>
                <b-button size="sm" class="my-2 my-sm-0" type="submit">Buscar</b-button>
            </b-navbar-nav>
        </b-collapse>
      </b-navbar>
    </div>
  </div>
</template>

<script>
export default {
  name: "navbar",
};
</script>

<style scoped>
.navBar {
  /*position: fixed;*/
  top: -0.82%;
  bottom: 0.82%;
  right: 0;
  left: 0;
  z-index: 100;
  /*height: 100%;
  width: 100%;*/
  flex: 100%;

}
#navbox {
  background:  #B5B6B9;
  height: 100%;
  width: 100%;
}
#ml-auto {
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 100%;
  padding-left: 15%;
  padding-right: 15%;
}

.qs {
  position: absolute;
  left: 47.53%;
  right: 42.74%;
  top: 40.16%;
  bottom: 39.34%;
}

.proj {
  position: absolute;
  left: 60.75%;
  right: 33.78%;
  top: 40.16%;
  bottom: 39.34%;
}

.cont {
  position: absolute;
  left: 71.63%;
  right: 23.58%;
  top: 40.16%;
  bottom: 39.84%;
}

input[type=text] {
  width: 242px;
  height: 32px;
  box-sizing: border-box;
  border: 1px solid black;
  border-radius: 5px;

  background-color: #B5B6B9;
  background: url(../assets/search.svg);
  font-family: Noto Sans;
  font-style: normal;
  font-weight: 400;
  font-size: 15px;
  line-height: 18px;
;
  background-position: 10px 10px; 
  background-repeat: no-repeat;
  padding: 12px 20px 12px 40px;
  align-content: center;
}
::placeholder{
    color: black;
    align-items: center;
    font-family: Noto Sans;
    font-weight: 400;
    font-size: 15px;
    line-height: 18px;
}

#logo{
    display: flex;
    height: 90px;
    width: 90px;
    left: 36px;
    top: 19px;
    border-radius: 0px;

}
.nav-itens{
  justify-content: space-between;
  align-items: end;
  white-space: nowrap;
  color:  #15213C;
}

.navbar-light .navbar-nav .nav-link {
  transition: 0.3s;
  color:  #15213C;
;
}
@media (max-width: 778px) {
  #navbox {
    display: flex;
    justify-content: flex-end;
  }
}


</style>
