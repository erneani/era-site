<template>
  <div class="section-about-header">
    <h2>
      {{ title }}
    </h2>
  </div>
</template>

<script>
export default {
  name: "AboutUsHeader",
  props: {
    title: String
  }
}
</script>

<style lang="scss" scoped>
.section-about-header {
  $primary: #277FF0;
  $secondary: #FFF;
  $gray: #E5E5E8;
  $text-color: #5B5C5B;
  font-family: "Roboto", sans-serif;
  color: $text-color;
  background: $gray;
  margin: auto;
  padding: 0.75rem;
  h2 {
    text-transform: uppercase;
    text-align: center;
    font-size: 1.5rem;
    font-weight: 500;
  }
}
</style>
