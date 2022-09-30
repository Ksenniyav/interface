import Header from '@/components/Header';
<template> 
<Header />
<div class="contaner" >
  <div class="contaner-1">
<img src="@/content/chap2.svg" alt=""/>
</div>
<div class="contaner-2">
  <img src="@/content/logo.svg" alt=""/>
</div>
<div class="contaner-3">
<img src="@/content/chap1.svg" alt=""/>
</div>
</div>
<switch-block />
</template>


<script>
import './assets/global.css'
import Header from '@/components/Header'
import SwitchBlock from './components/SwitchBlock.vue'
export default {
  components: { Header, SwitchBlock}
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
  /* position: absolute;
  width: 460px;
  height: 329px;
  left: 730px;
  top: 150px; */

  filter: drop-shadow(5px 5px 20px rgba(255, 255, 255, 0.25));
}
.contaner {
  display: flex;
  justify-content: center;

}
</style>

