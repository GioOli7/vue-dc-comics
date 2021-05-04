<template>
  <div id="app">
    <Header />
    <Content />
    <Footer />
  </div>
</template>

<script>
import Header from '@/components/Header.vue';
import Content from '@/components/Content.vue';
import Footer from '@/components/Footer.vue';

export default {
  name: 'App',
  components: {
    Header,
    Content,
    Footer,
  }
}
</script>

<style>
/* GENERAL */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

.container {
  max-width: 1100px;
  margin: 0 auto;
  height: 100%;
}

ul {
  list-style: none;
}

a {
  text-decoration: none;
  color: black;
}

</style>
