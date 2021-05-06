<template>


  <div class="portfolio">
    <v-container>
      <v-row>
      <v-col offset="1">
    <PortFrame />
      </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<style scoped>

</style>

<script>
import PortFrame from '../components/PortFrame';

export default {
  name: 'Portfolio',

  components: {
    PortFrame
  },

  data: () => ({
    //
  }),
};
</script>