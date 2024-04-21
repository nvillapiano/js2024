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
    <section class="Content-panel Portfolio">
      
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

</style>