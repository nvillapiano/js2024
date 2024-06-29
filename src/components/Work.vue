<script setup>
import { ref, onMounted } from 'vue'
const inputName = ref()
const inputEmail = ref()

onMounted(() => {
  const inputNameEl = inputName.value;

  inputNameEl.addEventListener('change', nameChange);
  function nameChange(){
    const nameValue = inputNameEl.value
    const nameLength = nameValue.length
    const nameLengthAdj = nameLength + 2
    const nameWidthInit = 15

    inputNameEl.addEventListener("blur", (event) => {    
      event.target.style.maxWidth = nameLengthAdj + `rem`
      if (nameLength) {
        event.target.style.maxWidth = nameLengthAdj + `rem`
      } else {
        event.target.style.maxWidth = nameWidthInit + `rem`
      }
    });
  }

  const inputEmailEl = inputEmail.value;

  inputEmailEl.addEventListener('change', emailChange);
  function emailChange(){
    const emailValue = inputEmailEl.value
    const emailLength = emailValue.length
    const emailLengthAdj = emailLength + 4
    const emailWidthInit = 15.25

    inputEmailEl.addEventListener("blur", (event) => {    
      if (emailLength) {
        event.target.style.maxWidth = emailLengthAdj + `rem`
      } else {
        event.target.style.maxWidth = emailWidthInit + `rem`
      }
      
    });
  }

})


// const inputNameWidth = inputName.offsetWidth;
// console.log('inputNameWidth', inputNameWidth);


// inputName.addEventListener('change', valueChange);
// function valueChange(){
//   console.log("value changed");
// }
</script>

<template>
<div class="Work">
  <h2>
    Work with Me
  </h2>
  <div class="form">
    <span>Hey Joanna! My name is</span><input ref="inputName" type="text" name="name" id="name" placeholder="prefered name">.<span> You can reach me at </span><input ref="inputEmail" type="email" name="email" id="email" placeholder="e-mail address">.<span>    
    In a few words, I'd like to share with you the following opportunity:</span>
    <textarea name="body" id="body" placeholder="Let me tell you about my idea..."></textarea>
    <button>Hit me up!</button>
  </div>
</div> 
</template>



<style lang="scss">

%focusStyle {
  outline: none;
  border-bottom-color: var(--js-white);
}

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
      max-width: initial;
      transition: all 0.3s;

      &#name {
        max-width: 15rem;
      }

      &#email {
        max-width: 15.25rem;
      }

      // &:placeholder-shown {
      //   max-width: 16rem;
      // }

      &:focus,
      &:focus-visible,
      &:focus-within {
        @extend %focusStyle;
      }

      &::placeholder {
        color: var(--js-white);
      }
    }

    textarea {
      display: block;
      width: 100%;
      aspect-ratio: 2/1;
      margin: 1rem 0 0 0;
      @include textStyle__default();
      padding: 2rem 2rem;
      font-size: 1.25rem;
      width: 100%;
      height: 6lh;
      line-height: 1.5;
      border: 2px solid var(--js-white);
      transition: border-color 0.3s;
      border-radius: 3.5rem;

      &:focus,
      &:focus-visible,
      &:focus-within {
        outline: none;
        border-color: var(--js-ruby);
      }
    }

    button {
      margin-top: 2rem;
      margin-left: auto;
    }
  }
}
</style>