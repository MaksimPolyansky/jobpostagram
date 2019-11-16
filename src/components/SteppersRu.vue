<template>
  <v-stepper v-model="e6" vertical>
    <v-stepper-step :complete="e6 > 1" step="1">Выберете тип объявления</v-stepper-step>

    <v-stepper-content step="1">
      <v-card color="grey lighten-1" class="mb-12" height="100px"></v-card>
      <v-btn color="primary" @click="e6 = 2">Continue</v-btn>
      
    </v-stepper-content>

    <v-stepper-step :complete="e6 > 2" step="2">Город и адрес офиса</v-stepper-step>

    <v-stepper-content step="2">
      <v-card color="grey lighten-1" class="mb-12" height="200px"></v-card>
      <v-btn color="primary" @click="e6 = 3">Continue</v-btn>
      <v-btn text @click="e6 = 1">Cancel</v-btn>
    </v-stepper-content>

    <v-stepper-step :complete="e6 > 3" step="3">Формат работы</v-stepper-step>

    <v-stepper-content step="3">
      <v-card color="grey lighten-1" class="mb-12" height="200px"></v-card>
      <v-btn color="primary" @click="e6 = 4">Continue</v-btn>
      <v-btn text @click="e6 = 2">Cancel</v-btn>
    </v-stepper-content>

    <v-stepper-step :complete="e6 > 4" step="4">Занятость</v-stepper-step>

    <v-stepper-content step="4">
      <v-card color="grey lighten-1" class="mb-12" height="200px"></v-card>
      <v-btn color="primary" @click="e6 = 5">Continue</v-btn>
      <v-btn text @click="e6 = 3">Cancel</v-btn>
    </v-stepper-content>

    <v-stepper-step :complete="e6 > 5" step="5">
      Зарплатная вилка
      <small>Оба значения (от ... до ...)</small>
    </v-stepper-step>

    <v-stepper-content step="5">
      <v-card color="grey lighten-1" class="mb-12" height="200px"></v-card>
      <v-btn color="primary" @click="e6 = 6">Continue</v-btn>
      <v-btn text @click="e6 = 4">Cancel</v-btn>
    </v-stepper-content>

    <v-stepper-step :complete="e6 > 6" step="6">Описание вакансии</v-stepper-step>

    <v-stepper-content step="6">
      <v-card color="grey lighten-1" class="mb-12" height="200px"></v-card>
      <v-btn color="primary" @click="e6 = 7">Continue</v-btn>
      <v-btn text @click="e6 = 5">Cancel</v-btn>
    </v-stepper-content>

    <v-stepper-step :complete="e6 > 7" step="7">Название компании</v-stepper-step>

    <v-stepper-content step="7">
      <v-card color="grey lighten-1" class="mb-12" height="200px"></v-card>
      <v-btn color="primary" @click="e6 = 8">Continue</v-btn>
      <v-btn text @click="e6 = 6">Cancel</v-btn>
    </v-stepper-content>

    <v-stepper-step step="8">Контакты</v-stepper-step>
    <v-stepper-content step="8">
      <v-card color="grey lighten-1" class="mb-12" height="200px"></v-card>
      <v-btn color="primary" @click="e6 = 1">Continue</v-btn>
      <v-btn text @click="e6 = 7">Cancel</v-btn>
    </v-stepper-content>
  </v-stepper>
</template>


<script>
  export default {
    data () {
      return {
        e6: 1,
      }
    },
  }
</script>