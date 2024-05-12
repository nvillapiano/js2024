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
    <div class="Portfolio">
    <h2 class="lilita">Creative Portfolio</h2>
    <ul class="list">
        <li>
        <h3>Comedy</h3>
        <a href="http://www.google.com">2 Dope Queens</a>
        <a href="http://www.google.com">Conan OBrien Needs a Friend</a>
        <a href="http://www.google.com">May I Elaborate with JB Smoove</a>
        </li>
        <li>
        <h3>Narrative</h3>
        <a href="http://www.google.com">This American Life</a>
        <a href="http://www.google.com">Finally a Show</a>
        <a href="http://www.google.com">Longest Shortest Time</a>
        </li>
        <li>
        <h3>End of life</h3>
        <a href="http://www.google.com">Scattered</a>
        <a href="http://www.google.com">Death, Sex and Money</a>
        <a href="http://www.google.com">Finally a Show</a>
        </li>
    </ul>
    </div>   
</template>



<style scoped>

.Portfolio {
  width: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;

  h1 {
    display: block;
  }

  p {
    display: block;
  }

  .list {
    text-align: left;
    width: clamp(5rem, 60vw, 60rem);
    margin: 0 auto;    
    padding: 4rem;
    border: 1rem dotted var(--js-white);
    position: relative;

    &::after {
      content: '';
      position: absolute;
      top: 1rem;
      left: 1rem;
      width: calc(100% - 2rem);
      height: calc(100% - 2rem);
      background: var(--js-straw);
      z-index: 0;
    }

    li {
      list-style: none;
      display: flex;
      align-items: flex-start;
      flex-direction: column;
      margin-bottom: 4rem;
      position: relative;
      z-index: 2;

    }
  }
}

</style>