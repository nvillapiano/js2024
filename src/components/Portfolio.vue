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
      <div class="blob">
        <svg viewBox="0 0 200 200" xmlns="http://www.w3.org/2000/svg">
          <path fill="var(--js-grass)" d="M40.1,-60.4C54,-53.6,68.6,-45.8,69.2,-34.5C69.9,-23.2,56.6,-8.5,52.7,6.4C48.7,21.3,53.9,36.3,50.9,49.6C47.9,62.8,36.5,74.3,23.9,75.3C11.2,76.2,-2.8,66.7,-16,60.2C-29.1,53.6,-41.5,50.1,-54.5,42.9C-67.6,35.6,-81.4,24.7,-81.4,12.8C-81.3,1,-67.4,-11.7,-56.1,-21.1C-44.8,-30.5,-36.2,-36.7,-27.2,-45.8C-18.3,-54.9,-9.2,-67,2,-70.1C13.1,-73.2,26.3,-67.3,40.1,-60.4Z" transform="translate(100 100)" />
        </svg>              
      </div>
    </div>   
</template>



<style scoped lang="scss">

.Portfolio {
  width: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  // 
  position: relative;

  h1 {
    display: block;
  }

  p {
    display: block;
  }

  .blob {
    width: 100%;
    height: 100%;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translateX(-50%) translateY(-50%);
    z-index: -1;
    margin-left: -5vw;

    svg {
      transform: rotate(180deg);
    }
  }

  .list {
    // outline: 1px solid red;
    width: 60%;
    margin: 0 auto;
    
    a, a:hover, a:active, a:visited {
      color: var(--js-mud);
      display: block;
    }

  }

  li {
    margin-top: 4rem;
  }
}

</style>