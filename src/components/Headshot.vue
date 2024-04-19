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
  bottom: 2rem;
  right: 2rem;
  
  img {
    display: block;
    border-radius: 50%;
    max-block-size: 30rem;
    block-size: 40vw;
    aspect-ratio: 1/1;
  }
}

</style>