<template>
  <div class="banner">
      <div class="container">
          <div class="card" v-for="(card, index) in cards" :key="index">
                <img :src="card.img" alt="">
                <span>{{card.title}}</span>
          </div>
      </div>
  </div>
</template>

<script>
export default {
    name: 'BannerShop',
    data() {
        return {
            cards: [
                {
                    title: 'DIGITAL COMICS',
                    img: require('../assets/img/buy-comics-digital-comics.png')
                },
                {
                    title: 'DC MERCHANDISE',
                    img: require('../assets/img/buy-comics-merchandise.png')
                },
                {
                    title: 'SUBSCRIPTION',
                    img: require('../assets/img/buy-comics-subscriptions.png')
                },
                {
                    title: 'COMIC SHOP LOCATOR',
                    img: require('../assets/img/buy-comics-shop-locator.png')
                },
                {
                    title: 'DC POWER VISA',
                    img: require('../assets/img/buy-dc-power-visa.svg')
                },
            ]
        }
    }

}
</script>

<style scoped>

.banner {
    height: 155px;
    background-color: dodgerblue;
}

.container,
.card {
    display: flex;
    align-items: center;
    justify-content: space-between;
}

.card {
    font-size: 14px;
    color: white;
}

.container {
    max-width: 1150px;
}

img {
    max-width: 60px;
    height: 60px;
    margin-right: 15px;
}

</style>