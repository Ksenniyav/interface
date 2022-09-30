<template>
  <button class="headerButton">
    <p><slot/></p>
  </button>
</template>

<script>
export default {
}
</script>

<style scoped>
.headerButton {
  width: 160px;
  height: 40px;
  background: #E45C00;
  box-shadow: 0px 4px 5px rgba(0, 0, 0, 0.1);
  border-radius: 8px;
  font-weight: 500;
  font-size: 20px;
  border: none;
  line-height: 24px;
  color: #FFFFFF;
  cursor: pointer;
}

.p {
  font-size: 20px;
  line-height: 24px;
  font-family: 'Helvetica Neue';
  font-style: normal;
  font-weight: 500;
  color: #FFFFFF;
  }
</style>
