<template>
  <div class="home">
    <div id="body-banner" class="d-flex justify-content-end bg-danger">
      <Banner id="banner" />
      <div id="conteudo">
        <Header />
        <p class="w-60">
          Venha comemorar o primeiro aniversário da Laurinha, contamos com sua
          presença!
        </p>
        <br />
        <p>
          <span class="fw-bold">ESPAÇO YELLOW</span>
          <br />
          Endereço: Rua Rio Jaguaribe, 426 - Bairro Alto - Curitiba/PR
          <br />
          Obs: Estacionamento atrás do salão na rua ao lado
        </p>
      </div>
    </div>
  </div>
</template>

<script>
import Header from "@/components/Navbar/Header.vue";
import Banner from "@/components/Banner/Banner.vue";

export default {
  name: "HomeView",
  components: {
    Header,
    Banner,
  },
};
</script>

<style  scooped>
#conteudo {
  width: 60%;
  flex-direction: column;
  justify-content: center;
  text-align: center !important;
  position: absolute;
  left: 0;
  color: #fff;
  font-size: 26px;
  display: flex;
}
.w-60 {
  width: 60% !important;
}
#conteudo p {
  text-align: center;
  margin: 0 auto;
  text-shadow: 1px 1px 1px #595959;
}
#body-banner {
  position: relative;
  top: 0;
  z-index: 1500 !important;
}
</style>
