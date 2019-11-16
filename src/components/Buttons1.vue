<template>
  <div id="app">
    <v-app id="inspire">
      <v-row align="center">
        <v-col class="text-center" cols="12" sm="50">
          <div class="my-2">
            <v-btn color="primary" v-on:click="handleClickBySomeButton">I am ready!</v-btn>
          </div>
        </v-col>
      </v-row>
    </v-app>
  </div>
</template>

<script>
  

  export default {
    

    methods: {
      handleClickBySomeButton(){
        return '/SteppersRu.vue';
      },
    },

  }
</script>