<template>
  <NavBar :logo="logo_src" :alt="app_name" />
  <router-view/>
  <Footer />
</template>

<script>
import NavBar from '@/components/NavBar.vue';
import Footer from '@/components/Footer.vue';

export default {
  components: {
    NavBar,
    Footer,
  },
  data() {
    return {
      logo_src: '/img/logo.png',
      app_name: 'Make Your Burger',
    };
  },
};
</script>

<style lang="scss">
  * {
    font-family: Helvetica;
    padding: 0;
    margin: 0;
    box-sizing: border-box;
  }

  .main-container {
    margin: 3rem;
    min-height: 15.5rem;
  }

  h1 {
    text-align: center;
    font-size: 2.625em;
    margin-bottom: 1.8rem;
    color: #222;
  }
</style>
