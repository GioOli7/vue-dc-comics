<template>
  <div class="card">
    <div class="card-img">
      <img :src="details.thumb" alt="">
    </div>
    <span class="title">{{details.series}}</span>
  </div>
</template>

<script>
export default {
  name: 'Comicscard',
  props: ['details']

}
</script>

<style scoped>

.card {
  width: calc(100% / 6 - 25px);
  margin-bottom: 50px;
}

.card-img {
  height: 185px;
  clip-path: border-box;
}

img {
  width: 100%;
}

.title {
  display: inline-block;
  margin-top: 15px;
  text-transform: uppercase;
  color: white;
  font-size: 13px;
}

</style>