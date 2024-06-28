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
<div class="Work">
  <h2>
    Work with Me
  </h2>
  <div class="form">
    <span>Hey Joanna! My name is</span><input type="text" name="name" id="name" placeholder="Your prefered name"><span>. You can reach me at </span><input type="email" name="email" id="email" placeholder="Your e-mail address"><span>.    
    In a few words, I'd like to share with you the following opportunity:</span>
    <textarea name="body" id="body" cols="30" rows="10" placeholder="Your message to me"></textarea>
    <button>Hit me up!</button>
  </div>
</div> 
</template>



<style scoped>

.Work {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin: 0 10vw;

  .form {
    font-size: 2rem;

    input {
      background: none;
      border: none;
      border-bottom: 2px solid var(--js-ruby);
      font-size: 2rem;
      color: var(--js-white);
      mix-blend-mode: initial;
      padding: 0 1rem;
      text-align: left;
      transition: border-bottom 0.3s;

      &:focus,
      &:focus-visible,
      &:focus-within {
        outline: none;
        border-bottom-color: var(--js-white);
      }
    }

    input::placeholder {
      color: var(--js-white);
    }

    textarea {
      display: block;
      width: 100%;
      aspect-ratio: 2/1;
      margin: 2rem 0 0 0;
    }
  }
}


</style>