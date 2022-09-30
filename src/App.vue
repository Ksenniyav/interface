import Header from '@/components/Header';
<template> 
<Header />
<div class="contaner-1">
<img src="@/content/chip2.svg" alt=""/>
</div>
<div class="contaner-2">
  <img src="@/content/fairfigtgame.jpg" alt=""/>
</div>
</template>


<script>
import './assets/global.css'
import Header from '@/components/Header'
export default {
  components: { Header}
}
</script>

<style>


#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
.contaner-2 {
  position: absolute;
  width: 460px;
  height: 329px;
  left: 730px;
  top: 150px;

  filter: drop-shadow(5px 5px 20px rgba(255, 255, 255, 0.25));
}
</style>

