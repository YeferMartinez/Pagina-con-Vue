<template>
  <v-carousel :show-arrows="false">
    <v-carousel-item
      v-for="(item,i) in items"
      :key="i"
      :src="item.src"
    ></v-carousel-item>
  </v-carousel>
</template>
<script>
export default {
  data () {
      return {
        items: [
          {
            src: require('../assets/images/carne-parrilla-1.jpg'),
          },
          {
            src: require('../assets/images/carne-parrilla-1.jpg'),
          },
          {
            src: require('../assets/images/carne-parrilla-1.jpg'),
          },
          {
            src: require('../assets/images/carne-parrilla-1.jpg'),
          },
        ],
      }
    },
}
</script>