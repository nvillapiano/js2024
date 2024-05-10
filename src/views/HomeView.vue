<script setup>
import Headshot from '../components/Headshot.vue'
import Badge from '../components/Badge.vue'
import Bio from '../components/Bio.vue'
</script>

<template>
  <main>
    <!-- <h1>Homepage content</h1> -->
    <Badge></Badge>
    <section class="Content-panel Bio">
      <Bio></Bio>
      <Headshot></Headshot>
    </section>
    <section class="Content-panel CreativePortfolio">
      <div class="portfolio-list">
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
    </section>
    <section class="Content-panel CreativePortfolio">
      <h2>
        Work with Me
      </h2>

    </section>
  </main>
</template>

<style scoped>

.Content-panel {
  --contentMargin: 4rem;
  display: flex;
  block-size: 100%;
  gap: 6rem;
  padding-inline: var(--contentMargin);
  align-items: center;
  justify-content: space-between;

  &.Bio {
    margin-block: 4rem 0;
  }
}


.CreativePortfolio {
    min-height: 18rem;
    background: var(--js-grass);
    position: relative;
    margin-top: 10rem;
    padding: 8rem 4rem 8rem 4rem;
    margin-bottom: -8rem;

    &::before {
      content: '';
      position: absolute;
      top: -9rem;
      left: 0;
      width: 100%;
      height: 10rem;
      background: var(--js-grass);
      clip-path: polygon(100% 100%, 0% 100% , 0.00% 66.67%, 2.00% 66.37%, 4.00% 65.50%, 6.00% 64.07%, 8.00% 62.15%, 10.00% 59.80%, 12.00% 57.10%, 14.00% 54.14%, 16.00% 51.05%, 18.00% 47.91%, 20.00% 44.85%, 22.00% 41.97%, 24.00% 39.38%, 26.00% 37.16%, 28.00% 35.39%, 30.00% 34.15%, 32.00% 33.46%, 34.00% 33.37%, 36.00% 33.86%, 38.00% 34.92%, 40.00% 36.52%, 42.00% 38.59%, 44.00% 41.07%, 46.00% 43.86%, 48.00% 46.88%, 50.00% 50.00%, 52.00% 53.12%, 54.00% 56.14%, 56.00% 58.93%, 58.00% 61.41%, 60.00% 63.48%, 62.00% 65.08%, 64.00% 66.14%, 66.00% 66.63%, 68.00% 66.54%, 70.00% 65.85%, 72.00% 64.61%, 74.00% 62.84%, 76.00% 60.62%, 78.00% 58.03%, 80.00% 55.15%, 82.00% 52.09%, 84.00% 48.95%, 86.00% 45.86%, 88.00% 42.90%, 90.00% 40.20%, 92.00% 37.85%, 94.00% 35.93%, 96.00% 34.50%, 98.00% 33.63%, 100.00% 33.33%);      
    }
  }

.portfolio-list {
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

h2 {
  font-size: clamp(4rem, 10vw, 8rem);
  text-align: center;
  margin-bottom: 8rem;
}



</style>