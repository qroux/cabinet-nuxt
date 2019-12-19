<template>
  <div>
    <MyNavbar />
    <transition name="slide" mode="out-in">
      <nuxt />
    </transition>
  </div>
</template>

<script>
import MyNavbar from './MyNavbar.vue'

export default {
  components: {
    MyNavbar
  }
}
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
  background-color: #f5f5f5;
}

*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
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
/*custom css*/
.banner {
  /* The image used */
  background: linear-gradient(rgba(0, 0, 0, 0.15), rgba(0, 0, 0, 0.15));
  /* Full height */
  min-height: 94vh;
  margin-top: 5px;

  /* Center and scale the image nicely */
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}
.text-container {
  color: white;
  padding: 15px;
}
.text-bg {
  color: black;
  background-color: rgba(255, 255, 255, 0.7);
  word-break: break-all;
}
/*custom transitions*/
.slide-enter-active {
  animation: slide-in 500ms ease-out forwards;
}
/*.slide-leave-active {
  animation: slide-out 10000ms ease-in forwards;
}*/
@keyframes slide-in {
  from {
    transform: translateY(-10px);
    opacity: 0;
  }
  to {
    transform: translateY(0);
    opacity: 1;
  }
}
/*@keyframes slide-out {
  from {
    transform: translateY(0);
    opacity: 1;
  }
  to {
    transform: translateY(-10px);
    opacity: 0;
  }
}*/
</style>
