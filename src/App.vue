<script setup>
import Masthead from './components/Masthead.vue'
</script>

<template>
  <header>
    <Masthead />
  </header>

  <RouterView />
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

</style>
