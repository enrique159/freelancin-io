<template>
  <div id="app">
    <Header/>
    <Stats/>
    <Features/>
  </div>
</template>

<script>
import Header from '@/components/Header.vue';
import Stats from '@/components/Stats.vue';
import Features from '@/components/Features.vue';
export default {
  components: {
    Header,
    Stats,
    Features
  },
};
</script>

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Inter:wght@100;200;300;400;500;600;700;800;900&display=swap");
@import url("https://cdn.jsdelivr.net/npm/bootstrap-icons@1.8.1/font/bootstrap-icons.css");
@import '@/assets/styles.scss';
</style>