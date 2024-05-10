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
      <span>J</span>
      <span>o</span>
      <span>a</span>
      <span>n</span>
      <span>n</span>
      <span>a</span>
      <span>&nbsp;</span>
      <span>S</span>
      <span>o</span>
      <span>l</span>
      <span>o</span>
      <span>t</span>
      <span>a</span>
      <span>r</span>
      <span>o</span>
      <span>f</span>
      <span>f</span>
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
    align-items: flex-start;
    justify-content: center;
    margin-top: 5vh;
    margin-left: 5rem;
  }

  .title {

    span {
      display: inline-block;
      color: var(--js-ruby);
      transition: all .2s ease-in-out;

      &:hover {
        color: var(--js-coral);
        transform: translateY(-2vh);        
      }
    }
  }

  .sub-title {
    font-size: clamp(3rem, 3.5vw, 3.5rem);
    color: var(--js-mud);
    font-weight: 600;
    margin-block: 0 2rem;
    mix-blend-mode: multiply;    
  }

</style>