<template>
  <div class="service-card-wrapper" v-if="cards">
    <div class="service-card" v-for="card in cards" v-bind:key="card.id"></div>
  </div>
</template>

<script>
export default {
  name: "ServiceCard",
  data: () => {
      return {
        cards: [
        { id:1 },
        { id:2 },
        { id:3 }
      ]
    }
  }
}
</script>

<style lang="scss" scoped>

.service-card-wrapper {
  display: flex;
  justify-content: center;
  margin: auto auto;
  height: 10rem;

  .service-card {
    background: purple;
    height: 100%;
    width: 20rem;
    display: inline-flex;
    margin: 0 1rem;
  }
}

</style>
