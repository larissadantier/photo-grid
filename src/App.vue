<template>
  <v-app>
    
    <v-main>
      <PhotoGrid/>
    </v-main>
  </v-app>
</template>

<script>
import PhotoGrid from './components/PhotoGrid';
export default {
  name: 'App',

  components: {
    PhotoGrid
  },

  data: () => ({
    //
  }),
};
</script>