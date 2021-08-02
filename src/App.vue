<template>
  <v-app>
    <v-container> 
      <v-row class="d-flex justify-center align-center">
        <v-col
            cols="6"
        >
          <h1>spli<br>tter</h1>
        </v-col>
    </v-row>
    </v-container>
    <v-main>
      <Calculator/>
    </v-main>
  </v-app>
</template>

<script>
import Calculator from './components/Calculator';

export default {
  name: 'App',

  components: {
    Calculator,
  },

  data: () => ({
    //
  }),
};
</script>
<style scoped>
  h1 {
    text-align: center;
  }
  #app {
  background-color: hsl(185, 41%, 84%);
}
</style>