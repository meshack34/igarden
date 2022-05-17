

<template>
  <v-app-bar app color="#111111" dark flat class="px-8">
    <v-btn icon>
      <v-icon color="#A7121D">fas fa-dragon</v-icon>
    </v-btn>


    <v-spacer></v-spacer>
    <v-btn text @click="scroll('home')">CORPORATES</v-btn>
    <v-btn text @click="scroll('project')">campus</v-btn>
    <v-btn text @click="scroll('about')">coworking</v-btn>
    <v-btn text @click="scroll('contact')"> Hire</v-btn>
    <v-btn text @click="scroll('about')">EVENTS</v-btn>
     <v-btn text @click="scroll('about')">BLOG</v-btn>
      <v-btn text @click="scroll('about')">ABOUT US</v-btn>
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