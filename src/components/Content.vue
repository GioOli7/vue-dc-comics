<template>

      <div class="content">
          <div class="container">
                <span class="btn title-section">CURRENT SERIES</span>
                <div class="cards">
                    <Comicscard v-for="(card, index) in comicsList" :key="index" :details="card" />
                    <span class="btn">LOAD MORE</span>
                </div>
          </div>
      </div>

</template>

<script>
import Comicscard from '@/components/Comicscard.vue';
import comicsList from '@/data/dc-comics.js'

export default {
    name: 'Content',
    components: {
        Comicscard,
    },
    data() {
        return {
            comicsList,
        }
    }
}
</script>

<style scoped>

.content {
    background-color: #1c1c1c;
}

.btn {
    display: inline-block;
    padding: 10px 55px;
    color: white;
    background-color: dodgerblue;
    margin: 0 auto;
    font-weight: bold;
    font-size: 12px;
}

.title-section {
    position: absolute;
    transform: translate(-15px, -50%);
    font-size: 24px;
    padding: 10px 30px;
}

.cards {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    padding: 50px 0;
    padding-bottom: 20px;
}

</style>