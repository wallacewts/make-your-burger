<template>
  <div id="nav">
    <router-link to="/" id="logo-url">
      <img :src="logo" :alt="alt" id="logo">
    </router-link>
    <router-link to="/">Home</router-link>
    <router-link to="/Pedidos">Pedidos</router-link>
  </div>
</template>

<script>
export default {
  name: 'NavBar',
  props: ['logo', 'alt'],
};
</script>

<style lang="scss" scoped>
  #nav {
    background-color: #222;
    border-bottom: 4px solid #111;
    padding: 1rem 3rem;
    display: flex;
    justify-content: flex-end;
    align-items: center;

    a {
      color: #FCBA03;
      text-decoration: none;
      margin: .8rem;
      transition: .5s;

      &:hover {
        color: #FFF;
      }
    }

    #logo-url {
      margin: auto;
      margin-left: 0;

      #logo {
        width: 2.5rem;
        height: 2.5rem;
      }
    }
  }
</style>
