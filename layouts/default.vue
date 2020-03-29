<template>
  <div>
    <transition name="page" mode="out-in">
      <nuxt />
    </transition>
    <div class="mask">
      <div id="ken"></div>
    </div>
  </div>
</template>

<script lang="ts">
export default({
  transition:{
    name: "page"
  }
})
</script>

<style>
html {
  font-family: 'Source Sans Pro', -apple-system, BlinkMacSystemFont, 'Segoe UI',
    Roboto, 'Helvetica Neue', Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
}

body{
  background-image: linear-gradient(-45deg, #fff, #a5bccc,#3c78e7, #000);
  background-size: 400% 400%;
  animation: gradient 20s ease-in-out infinite;
}


@media screen and (max-width: 414px){
  #ken{
    width: 100vw;
    height: 100vw;
    margin: 0 auto;
    background-size: 50% 50%;
    background-repeat: no-repeat;
    animation: ken-chan 20s ease-in-out infinite;
    position: fixed;
    top: 25%;
    left: 0;
    right: 0;
    z-index: -1;
    opacity: 0.1;
  }
}
@media screen and (min-width: 415px){
  #ken{
    width: 100vh;
    height: 100vh;
    margin: 0 auto;
    background-size: 50% 50%;
    background-repeat: no-repeat;
    animation: ken-chan 20s ease-in-out infinite;
    position: fixed;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    z-index: -1;
    opacity: 0.1;
  }
}

.button--green {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #3b8070;
  color: #3b8070;
  text-decoration: none;
  padding: 10px 30px;
}

.button--green:hover {
  color: #fff;
  background-color: #3b8070;
}

.button--grey {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #35495e;
  color: #35495e;
  text-decoration: none;
  padding: 10px 30px;
  margin-left: 15px;
}

.button--grey:hover {
  color: #fff;
  background-color: #35495e;
}

.button--white {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid;
  text-decoration: none;
  padding: 10px 30px;
  margin-left: 15px;
  animation: color-change 20s ease-in-out infinite;
}

.button--grey:hover {
  color: #fff;
  background-color: #35495e;
}

.change_font{
  animation: font-change 20s ease-in-out infinite;
}

@keyframes font-change {
    0% {
      color: #fff;
    }
    25% {
      color: #a5bccc;
    }
    50% {
      color: #000;
    }
    75% {
      color: #3c78e7;
    }
    100% {
      color: #fff;
    }
}

@keyframes color-change {
    0% {
      border: 1px solid #fff;
      color: #fff;
    }
    25% {
      border: 1px solid #a5bccc;
      color: #a5bccc;
    }
    50% {
      border: 1px solid #000;
      color: #000;
    }
    75% {
      border: 1px solid #3c78e7;
      color: #3c78e7;
    }
    100% {
      border: 1px solid #fff;
      color: #fff;
    }
}

@keyframes ken-chan {
    0% {
      background-position: 50% 50%;
      opacity: 0;
      background-image: url("~assets/ken.png");
    }
    12.5% {
      background-position: 100% 50%;
      opacity: 0.1;
      background-image: url("~assets/ken.png");
    }
    25% {
      background-position: 50% 50%;
      opacity: 0;
      background-image: url("~assets/ken.png");
    }
    26% {
      background-image: url("~assets/black.png");
    }
    37.5% {
      background-position: 0% 50%;
      opacity: 0.1;
      background-image: url("~assets/black.png");
    }
    50% {
      background-position: 50% 50%;
      opacity: 0;
      background-image: url("~assets/black.png");
    }
    51% {
      background-image: url("~assets/ken.png");
    }
    62.5% {
      background-position: 50% 100%;
      opacity: 0.1;
      background-image: url("~assets/ken.png");
    }
    75% {
      background-position: 50% 50%;
      opacity: 0;
      background-image: url("~assets/ken.png");
    }
    76% {
      background-image: url("~assets/black.png");
    }
    87.5% {
      background-position: 50% 0%;
      opacity: 0.1;
      background-image: url("~assets/black.png");
    }
    100% {
      background-position: 50% 50%;
      opacity: 0;
      background-image: url("~assets/black.png");
    }
}

@keyframes gradient {
    0% {
        background-position: 0% 50%;
    }
    50% {
        background-position: 100% 50%;
    }
    100% {
        background-position: 0% 50%;
    }
}

  .page-enter, .page-leave{
    opacity: 0;

  }
  .page-enter-active, .page-leave-active {
    animation: pgIn 2s;
  }

@keyframes pgIn{
  0%{
    opacity: 0;
    transform: translateX(100px);
  }
  100%{
    opacity: 1;
    transform: translateX(0);
  }
}
</style>
