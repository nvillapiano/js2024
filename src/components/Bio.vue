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
  <div class="Bio">
    <h2>Hi, I'm Joanna.</h2>
    <p>
      I specialize in making big-hearted, funny content. In addition to my creative work, I received my End of Life care certificate from the University of Vermont and am committed to better end of life outcomes for all through education and storytelling.
    </p>
    <div class="Bio--shape">
      <svg viewBox="0 0 200 200" xmlns="http://www.w3.org/2000/svg">
        <path fill="var(--js-coral)" d="M40.1,-60.4C54,-53.6,68.6,-45.8,69.2,-34.5C69.9,-23.2,56.6,-8.5,52.7,6.4C48.7,21.3,53.9,36.3,50.9,49.6C47.9,62.8,36.5,74.3,23.9,75.3C11.2,76.2,-2.8,66.7,-16,60.2C-29.1,53.6,-41.5,50.1,-54.5,42.9C-67.6,35.6,-81.4,24.7,-81.4,12.8C-81.3,1,-67.4,-11.7,-56.1,-21.1C-44.8,-30.5,-36.2,-36.7,-27.2,-45.8C-18.3,-54.9,-9.2,-67,2,-70.1C13.1,-73.2,26.3,-67.3,40.1,-60.4Z" transform="translate(100 100)" />
      </svg>      
    </div>
  </div>
</template>



<style scoped>

.Bio {
  position: relative;
  color: var(--js-mud);  

  .Bio--shape {
    position: absolute;
    width: 125%;
    top: -90%;
    left: -10%;
    z-index: -1;
  }
}

</style>