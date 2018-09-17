<template>
  <div class="services-description">
    <h2 class="services-title">
      {{ title }}
    </h2>
    <p class="services-text">
      {{ text }}
    </p>
  </div>
</template>

<script>
export default {
  name: "Services",
  props: {
    title: String,
    text: String
  }
}
</script>

<style lang="scss" scoped>
.services-description {
  $primary: #277FF0;
  $text-color: #5B5C5B;
  padding: 2rem 4rem;
  display: flex;
  flex-direction: column;
  text-align: center;
  font-family: "Roboto", sans-serif;

  .services-title {
    color: $primary;
    font-size: 1.875rem;
    margin: 0;
  }

  .services-text {
    color: $text-color;
    margin: 0.75rem auto;
    font-size: 1.25rem;
    width: 50%;
  }  
}
</style>
