<template>
  <header class="container">
      <img src="../assets/img/dc-logo.png" alt="DC logo">
      <nav>
          <ul>
              <li v-for="(link, index) in navLinks" :key="index">
                  <a :href="link.url"> {{ link.text }} </a>
              </li>
          </ul>
      </nav>
  </header>
</template>

<script>
export default {
    // per coerenza inserisco lo stesso nome che ha il componente
    name: 'Header',
    data() {
        return {
            navLinks: [
                {
                    text:'characters', url:"/characters", current: true,
                },
                {
                    text:'comics', url:"/comics", current: false,
                }, 
                {
                    text:'movies', url:"/movies", current: false,
                },
                {
                    text:'tv', url:"/tv", current: false,
                },
                {
                    text:'games', url:"/games", current: false,
                },
                {
                    text:'collectibles', url:"/collectibles", current: false,
                }, 
                {
                    text:'videos', url:"/videos", current: false,
                }, 
                {
                    text:'fans', url:"/fans", current: false,
                },
                {
                    text:'news', url:"/news", current: false,
                },
                {
                    text:'shop', url:"/shop", current: false,
                },
            ],
        }
    }

}
</script>



<style scoped>

header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 150px;
    padding: 20px 0;
}

ul {
    display: flex;
    text-transform: uppercase;
}

ul li {
    padding: 10px;
    border-bottom: 3px solid transparent;
}

li:hover,
li:active{
    border-bottom: 3px solid #0c7cec;
}


li a {
    color: black;
    font-size: 12px;
    font-weight: bold;
    height: 100%;
}


</style>