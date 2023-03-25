<template>
  <!-- <nav>
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link>
  </nav> -->


      <thenav/>  
           
           
  <router-view/>
  <thefoter/>
</template>


<script>
import thenav from './components/thenav.vue'
import thefoter from './components/thefooter.vue'
export default {
  components:{
thenav,
thefoter
  },
  setup(){
 
  }
}
</script>

<style lang="scss">


@import './sass/main.scss';


#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  // text-align: center;
  color: #2c3e50;
}

// nav {
//   padding: 30px;

//   a {
//     font-weight: bold;
//     color: #2c3e50;

//     &.router-link-exact-active {
//       color: #42b983;
//     }
//   }
// }



</style>
