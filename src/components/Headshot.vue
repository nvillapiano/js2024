<script setup>
defineProps({
  // sample prop set-up
  // msg: {
  //   type: String,
  //   required: true
  // }
})
</script>

<template>
  <div class="Headshot">
    <img src="@/assets/js-headshot.jpeg" alt="Professional headshot for Joanna Solotaroff">
  </div>
</template>



<style scoped>

.Headshot {
  position: absolute;
  bottom: 0;
  right: 0;
  
  img {
    display: block;
    border-radius: 50%;
    max-block-size: 70vh;
    min-block-size: 50vw;
    aspect-ratio: 1/1;
  }
}

</style>