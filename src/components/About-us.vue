<template>
  <div class="section-about">
    <div class="about-left-panel">
      <div class="about-left-row">
        <h2 class="about-left-header">
          {{ leftHeader }}
        </h2>
        <!--<img src="#" alt="An about-us image" class="left-image">-->
        <div class="about-left-image"></div>
      </div>
      <p class="about-left-text">
        {{ leftText }}
      </p>
    </div>
    <div class="about-right-panel">
      <p class="about-right-text">
        {{ rightText }}
      </p>
      <h2 class="about-right-header">
        {{ rightHeader }}
      </h2>
    </div>
  </div>
</template>

<script>
export default {
  name: "AboutUs",
  props: {
    leftHeader: String,
    leftText: String,
    rightHeader: String,
    rightText: String
  }  
}
</script>

<style lang="scss" scoped>

.section-about {
  $primary: #277FF0;
  $secondary: #FFF;
  $gray: #E5E5E8;
  $text-color: #5B5C5B;
  font-family: "Roboto", sans-serif;
  display: flex;
  flex-direction: row;

  .about-left-panel {
    display: inline-flex;
    flex-direction: column;
    justify-content: space-around;
    width: 50%;
    height: 25rem;
    background: $primary;
    color: $secondary;
    
    .about-left-row {
      flex-direction: row;

      .about-left-header {
        padding: 2rem;
        font-size: 1.5rem;
        display: inline-flex;
      }

      .about-left-image {
        display: none;
      }
    }

    .about-left-text {
      padding: 2rem;
      font-size: 1.25rem;
    }
  }

  .about-right-panel {
    display: inline-flex;
    flex-direction: column;
    justify-content: space-around;
    width: 50%;
    height: 25rem;
    background: $secondary;
    color: $primary;

    .about-right-header {
      padding: 2rem;
      font-size: 1.5rem;
      text-align: end;
    }

    .about-right-text {
      padding: 2rem;
      font-size: 1.25rem;
      text-align: end;
    }
  }
}

</style>
