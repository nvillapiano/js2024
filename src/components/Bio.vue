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
  </div>
</template>



<style scoped>

.Bio {
  color: var(--js-mud);

  h2 {
    font-size: 2.5rem;
    font-weight: 600;
    margin-block: 0 2rem;
  }

  p {
    font-size: 1.5rem;
  }
}

</style>