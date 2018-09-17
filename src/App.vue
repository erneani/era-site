<template>
  <div id="app">
    <NavBar />
    <Home 
      main-title="Lorem Ipsum" 
      text="Lorem ipsum dolor sit amet, consectetur adipiscing elit. Cras ultricies id nisi eu mollis. Duis sit amet magna pretium lectus pretium ultricies."
      call-to-action="Saiba mais!"  
    />
    <Services
      title="Serviços"
      text="Lorem ipsum dolor sit amet, consectetur adipiscing elit. Cras ultricies id nisi eu mollis. Duis sit amet magna pretium lectus pretium ultricies."
    />
    <ServiceCard />
    <ServicesBody />
    <AuxiliarBar />
    <AboutUsHeader title="Quem somos"/>
    <AboutUs
      left-header="Nossa missão"
      left-text="Lorem ipsum dolor sit amet, consectetur adipiscing elit. Cras ultricies id nisi eu mollis. Duis sit amet magna pretium lectus pretium ultricies."
      right-header="Sobre nós"
      right-text="Lorem ipsum dolor sit amet, consectetur adipiscing elit. Cras ultricies id nisi eu mollis. Duis sit amet magna pretium lectus pretium ultricies."
    />
  </div>
</template>

<script>
import NavBar from "./components/NavBar.vue";
import Home from "./sections/Home.vue";
import Services from "./components/Services.vue";
import ServiceCard from "./components/Service-card.vue";
import ServicesBody from "./components/Service-body.vue";
import AuxiliarBar from "./components/Auxiliar-bar.vue";
import AboutUsHeader from "./components/About-us-header.vue";
import AboutUs from "./components/About-us.vue";

export default {
  name: "app",
  components: {
    NavBar,
    Home,
    Services,
    ServiceCard,
    ServicesBody,
    AuxiliarBar,
    AboutUsHeader,
    AboutUs
  }
};
</script>

<style lang="scss">
body {
  margin: 0;
  padding: 0;
}

#app {
  
}
</style>
