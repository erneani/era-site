<template>
  <nav class="navbar">
    <div class="navbar-logo-wrapper">
      <img src="#" alt="Main Logo" class="navbar-logo">
    </div>
    <div class="navbar-list-wrapper">
      <ul class="navbar-list" v-if="itens">
        <li class="navbar-list-item-wrapper" v-for="item in itens" v-bind:key="item.id">
          <a href="#" class="navbar-list-item">
           {{ item.label }} 
          </a>
        </li>
      </ul>
    </div>
  </nav>
</template>

<script>
export default {
  name: "NavBar",
  data: () => {
    return {
      itens: [
        { id:1, label: "Principal" },
        { id:2, label: "Serviços" },
        { id:3, label: "Quem somos" },
        { id:4, label: "Contato" }
      ]
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

.navbar {
  $primary: #277FF0;
  $secondary: #FFF;
  $hover-link: #096def;
  $shadow: #5B5C5B;
  height: 4.375rem;
  background: $secondary;
  display: flex;
  justify-content: space-between;
  box-shadow: 0px 5px 5px $shadow;

  .navbar-logo-wrapper {
    display: inline-flex;
    margin: auto 0 auto 50px;
    height: 3.125rem;

    .navbar-logo {
      height: 100%;
    }
  }

  .navbar-list-wrapper {
    display: inline-flex;

    .navbar-list {
      margin: auto 3.125rem auto 0;

      .navbar-list-item-wrapper {
        display: inline-flex;

        .navbar-list-item {
          font-size: 1rem;
          text-transform: uppercase;
          text-decoration: none;
          color: $primary;
          font-family: 'Roboto', sans-serif;
          font-weight: 400;
          transition: 0.3s ease-out;
          padding: .5rem 1rem;
          border-bottom: 2px solid transparent;

          &:hover {
            border-bottom: 2px solid $primary;
            color: $hover-link;
          }
        }
      }
    }
  }
}

</style>
