<template>
  <div class="home-section-wrapper">
    <div class="left-section-wrapper">
      <div class="left-section-content-wrapper">
        <h1 class="section-main-title">
          {{ mainTitle }}
        </h1>
        <p class="section-text">
          {{ text }}
        </p>
        <a href="#" class="section-call-to-action">
          {{ callToAction }}
        </a>
      </div>
    </div>
    <div class="rigth-section-wrapper">
      <div class="rigth-section-big-image">
        <!--  <img src="#" alt="A big image"> -->
        <div class="fake-image"></div>
      </div>
    </div> 
  </div>
</template>

<script>
export default {
  name: "Home",
  props: {
    mainTitle: String,
    text: String,
    callToAction: String
  }
}
</script>

<style lang="scss" scoped>

.home-section-wrapper {
  $primary: #277FF0;
  $secondary: #FFF;
  display: flex;
  height: 28.75rem;
  width: 100%;
  text-align: center;

  .left-section-wrapper {
    display: inline-flex;
    background-color: $primary;
    width: 65%;
    color: $secondary;

    .left-section-content-wrapper {
      height: 100%;
      font-family: "Roboto", sans-serif;

      .section-main-title {
        padding: 1.875rem;
      }
      
      .section-text {
        padding: 3.75rem;
        font-size: 1.25rem;
      }
      .section-call-to-action {
        
        padding: .5rem 1rem;
        text-decoration: none;
        text-transform: uppercase;
        color: $secondary;
        border: 1px solid $secondary;
        background: $primary;
        transition: 0.5s;
        font-size: 1.125rem;

        &:hover {
          color: $primary;
          background: $secondary;
        }
      }
    }
  }

  .rigth-section-wrapper {
    display: inline-flex;
    width: 35%;
    background: purple;

    .rigth-section-big-image {
      height: 100%;
    }
  }
}

</style>
