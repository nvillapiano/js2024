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
  <div class="titles fraunces">
    <h1 class="title">
      Joanna Solotaroff
    </h1>
    <h2 class="sub-title">
      Producer / Death Doula
    </h2>
  </div>
</template>



<style scoped>

  .titles {
    width: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    margin-top: 5vh;
  }

  .title {
    font-size: 10vw;
    font-style: italic;
  }

  .sub-title {
    color: var(--js-mud);
  }

</style>