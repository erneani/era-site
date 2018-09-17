<template>
  <div class="service-card-body">
    <div class="service-card" v-if="cards" v-for="card in cards" v-bind:key="card.id">
      <h3 class="service-card-title">
        {{ card.title }}
      </h3>
      <p class="service-card-text">
        {{ card.text }}
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name: "ServicesBody",
  data: () => {
    return { 
      cards: [
        { id:1, title: "Encomendas", text: "From upsodia to trajodia, we have it!" },
        { id:2, title: "Manutenção", text: "Integer est nisl, commodo sit amet turpis nec, vulputate egestas risus. Vestibulum metus dolor, molestie condimentum metus at, pulvinar ullamcorper ligula." },
        { id:3, title: "Gráfica", text: "Lorem ispum dolor sit amet nameteun consectur dales gravida iconi dum trophius admoni adornis saphis vur" },
      ]
    }
  }
}
</script>

<style lang="scss" scoped>

.service-card-body {
  $primary: #277FF0;
  $secondary: #FFF;
  $text-color: #5B5C5B;
  display: flex;
  justify-content: center;
  margin: auto auto;
  height: auto;
  overflow: visible;
  background: $primary;

  .service-card {
    background: $secondary;
    height: 100%;
    width: 20rem;
    display: inline-flex;
    margin: 0 1rem;
    text-align: center;
    font-family: "Roboto", sans-serif;
    color: $text-color;
    flex-direction: column;
    min-height: auto;

    .service-card-title {
      font-size: 1.375rem;
    }

    .service-card-text {
      padding: 0 2rem 0.5rem 2rem;
      font-size: 1.125rem;
    }
  }
}

</style>
