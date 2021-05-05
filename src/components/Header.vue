<template>
  <header class="container">
      <img src="../assets/img/dc-logo.png" alt="DC logo">
      <nav>
          <ul>
              <li v-for="(link, index) in navLinks" :key="index" :class="{active: link.current}">
                  <a :href="link.url" :class="{active: link.current}"> {{ link.text }} </a>
              </li>
          </ul>
      </nav>
  </header>
</template>

<script>
import navLinks from '@/data/navLinks.js';

export default {
    // per coerenza inserisco lo stesso nome che ha il componente
    name: 'Header',
    data() {
        return {
            // sarebbe come -> navLinks: navLinks; siccome hanno lo stesso nome, sfrutto ES per abbreviare.
            navLinks,
        }
    }

}
</script>



<style scoped lang="scss">
@import "@/styles/vars.scss";


header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 150px;
    padding: 20px 0;
}

.active {
    color: $primary;
}

ul {
    display: flex;
    text-transform: uppercase;
    li {
        padding: 10px;
        border-bottom: 5px solid transparent;
        height: 150px;
        display: flex;
        align-items: center;
        &:hover,
        &.active {
            border-bottom: 5px solid $primary;
        }
        a {
            color: black;
            font-size: 12px;
            font-weight: bold;
        }
    }
}

// **********OLD CSS for example
// ul {
//     display: flex;
//     text-transform: uppercase;
    
// }

// ul li {
//     padding: 10px;
//     border-bottom: 5px solid transparent;
//     height: 150px;
//     display: flex;
//     align-items: center;
// }

// li:hover,
// li.active{
//     border-bottom: 5px solid #0c7cec;
// }


// li a {
//     color: black;
//     font-size: 12px;
//     font-weight: bold;
// }


</style>