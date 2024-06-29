<script setup>
import Masthead from './components/Masthead.vue'
import Footer from './components/Footer.vue'
</script>

<template>
  <header>
    <Masthead />
  </header>
  <RouterView />
  <footer>
    <Footer></Footer>
  </footer>
</template>

<style >

/* Globals */


.fraunces {
  font-family: "Fraunces", serif;
  font-optical-sizing: auto;
  font-weight: 400;
  font-style: normal;
  font-variation-settings:
    "SOFT" 0,
    "WONK" 0;
}

.syne {
  font-family: "Syne", sans-serif;
  font-optical-sizing: auto;
  font-weight: 400;
  font-style: normal;
}


</style>
