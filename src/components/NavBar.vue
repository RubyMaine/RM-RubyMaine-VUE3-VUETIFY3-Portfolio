<template>
    <v-app-bar app color="black" dark flat class="px-12" >
      <v-btn >
        <v-icon color="yellow" left class="mr-2">fas fa-signature</v-icon> RubyMaine
      </v-btn>

      <v-spacer></v-spacer>
      <v-btn text @click="scroll('home')" class="text-yellow"> Главная </v-btn>
      <v-btn text @click="scroll('about')" > О нас </v-btn>
      <v-btn text @click="scroll('portfolio')" > Портфолио </v-btn>
      <v-btn text @click="scroll('services')" > Услуги </v-btn>
      <v-btn text @click="scroll('page')" > Страница </v-btn>
      <v-btn text @click="scroll('biog')" > Биог </v-btn>
      <v-btn text @click="scroll('contact')" > Контакт </v-btn>
    </v-app-bar>
  </template>
  
  <script>
  export default {
    methods: {
      scroll(refName) {
        const element = document.getElementById(refName);
        element.scrollIntoView({ behavior: "smooth" });
      },
    },
  };
  </script>
  
  <style>
  </style>