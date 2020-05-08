<template>
  <div class="home">
    

  <v-carousel height="100%" hide-delimiters >
      <v-carousel-item
        v-for="(item,i) in items"
        :key="i"
        :src="item.src"
      ></v-carousel-item>
    </v-carousel>

   
  </div>
</template>

<script>


export default {
  name: 'Home',
  data () {
      return {
        items: [
          {
            src: require('../assets/projects/nyt.jpg'),
          },
          {
            src: require('../assets/projects/nyt.jpg'),
          },
          {
            src: require('../assets/projects/nyt.jpg'),
          },
          {
            src: require('../assets/projects/nyt.jpg'),
          },
        ],
      }
    },
  components: {

  }
}
</script>
<style >

.home {
  height: 100vh;
}
  
</style>