<template>
  <div class="Badge">
    <div class="Badge--shape">
    
    </div>
    <div class="Badge--text">
      <a class="Badge--text" href="#hireme">Hire Me</a>
    </div>
    
  </div>
</template>



<style scoped lang="scss">

@keyframes spin {
  from {
    transform: rotate(0deg);
  }

  to {
    transform: rotate(180deg);
  }
}

.Badge {
  --badgeSize: 6rem;
  --badgeRadius: .75rem;
  block-size: var(--badgeSize);
  aspect-ratio: 1/1;  
  position: absolute;
  top: 4rem;
  right: 4rem;  
  display: flex;
  align-items: center;
  justify-content: center;    


  &--shape {
    position: absolute;
    block-size: 100%;
    aspect-ratio: 1/1;
    background: var(--js-plum);
    text-align: center;
    transform: rotate(20deg);
    border-radius: var(--badgeRadius);
    z-index: -1;
    //
    animation-name: spin;
    animation-duration: 1.5s;    
    animation-iteration-count: infinite;
    animation-direction: normal;


    &::before {
      content: "";
      position: absolute;
      top: 0;
      left: 0;
      block-size: var(--badgeSize);
      aspect-ratio: 1/1;
      background: var(--js-plum);
      transform: rotate(135deg);    
      border-radius: var(--badgeRadius);
    }    
  }

  &--text {    
    
    a, a:active, a:visited, a:focus, a:hover, a:link {
      color: var(--js-white);
      text-decoration: none;
      font-size: 1.4rem;
      font-weight: 500;
      padding: 3rem 1rem;
      text-wrap: nowrap;
      mix-blend-mode: normal;
    }    
  }

  &:hover {
      
    .Badge--shape {      
    }
  }

}

</style>