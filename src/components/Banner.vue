<template>
  <div id="main-banner">
    <h1>Make Your Buger</h1>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'Banner',
});
</script>

<style lang="scss" scoped>
  #main-banner {
    background-image: url('/img/burger.jpg');
    background-repeat: no-repeat;
    background-size: cover;
    height: 40rem;
    display: flex;
    align-items: center;
    justify-content: flex-start;

    h1 {
      color: #FFF;
      text-align: center;
      font-size: 4em;
      background-color: #222;
      padding: 1rem;
    }
  }
</style>
