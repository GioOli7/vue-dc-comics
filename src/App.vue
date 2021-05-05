<template>
  <div id="app">
    <Header />
    <main>
      <Hero />
      <Content />
      <BannerShop />
    </main>
    <Footer />
  </div>
</template>

<script>
import Header from '@/components/Header.vue';
import Content from '@/components/Content.vue';
import Footer from '@/components/Footer.vue';
import Hero from '@/components/Hero.vue';
import BannerShop from '@/components/BannerShop.vue';



export default {
  name: 'App',
  components: {
    Header,
    Hero,
    Content,
    BannerShop,
    Footer,
  }
}
</script>

<style lang="scss">
/* GENERAL */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

.container {
  max-width: 1250px;
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
