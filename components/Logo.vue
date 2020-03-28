<template>
    <img class="DragonLogo" src="~assets/white.jpg" alt="白い巨匠(BlackDragon)">
</template>
<style>
.DragonLogo {
  animation: 2s appear;
  margin: auto;
  border-radius: 100%;
  max-width: 30%;
  max-height: 30%;
}

@keyframes appear {
  0% {
    opacity: 0;
  }
  100% {
    opacity: 1;
  }
}
</style>
