<template>
  <div class="banner">
      <div class="container">
          <div class="card" v-for="(card, index) in shops" :key="index">
                <img :src="card.img" alt="">
                <span>{{card.title}}</span>
          </div>
      </div>
  </div>
</template>

<script>
import shops from "@/data/shops.js";

export default {
    name: 'BannerShop',
    data() {
        return {
            shops, 
        }
    }

}
</script>

<style scoped lang="scss">
@import "@/styles/vars.scss";


.banner {
    height: 155px;
    background-color: $primary;
}

.container {
    max-width: 1150px;
    .card {
        font-size: 14px;
        color: white;
        img {
            max-width: 60px;
            height: 60px;
            margin-right: 15px;
        }
    }
    // stili consivisi da container e card
    &,
    .card {
        display: flex;
        align-items: center;
        justify-content: space-between;
    }
}

/* .container,
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
} */

// img {
//     max-width: 60px;
//     height: 60px;
//     margin-right: 15px;
// }

</style>