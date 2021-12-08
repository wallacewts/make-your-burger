<template>
  <div class="main-container">
    <Banner />
    <h1>Monte o seu burger:</h1>

  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import Banner from '@/components/Banner.vue';

export default defineComponent({
  name: 'Home',
  components: {
    Banner,
  },
});
</script>
