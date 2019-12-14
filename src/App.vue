<template>
  <v-app>
    <!--<v-app-bar
      app
      color="primary"
      dark
    >
      <div class="d-flex align-center">
        <v-img
          alt="Vuetify Logo"
          class="shrink mr-2"
          contain
          src="https://cdn.vuetifyjs.com/images/logos/vuetify-logo-dark.png"
          transition="scale-transition"
          width="40"
        />

        <v-img
          alt="Vuetify Name"
          class="shrink mt-1 hidden-sm-and-down"
          contain
          min-width="100"
          src="https://cdn.vuetifyjs.com/images/logos/vuetify-name-dark.png"
          width="100"
        />
      </div>

      <v-spacer></v-spacer>

      <v-btn
        href="https://github.com/vuetifyjs/vuetify/releases/latest"
        target="_blank"
        text
      >
        <span class="mr-2">Latest Release</span>
        <v-icon>mdi-open-in-new</v-icon>
      </v-btn>
    </v-app-bar>-->
    
    <v-content>
      
      <v-btn v-if="!showSteppers" @click="handleClick">Btn1</v-btn>
      <v-btn v-if="showSteppers" @click="handleClick">Btn2</v-btn>  

      <!-- 
      <Buttons1 v-if="!showSteppers" @click="handleClick"/>
      <SteppersRu v-if="showSteppers"/>
      -->
      
    </v-content>
  </v-app>
</template>

<script>

// import Buttons1 from './components/Buttons1';
// import SteppersRu from './components/SteppersRu';


export default {
  name: 'App',

  components: {
    
    // Buttons1,
    // SteppersRu,
    

  },

  data: () => ({
    showSteppers: false,
    
  }),
  methods: {
    handleClick() {
      this.showSteppers = !this.showSteppers;
    },
    
  },
  
};
</script>
