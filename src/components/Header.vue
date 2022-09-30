<template>
    <header>
        <div class='logo'>
            <img src="../content/titleHeader.svg" alt="">
        </div>
        <div class='button1'>
        <HeaderButton >
            Connect
        </HeaderButton>
        </div>
    </header>
</template>

<script>
import HeaderButton from './HeaderButton.vue';
export default {
    name: "Header-main",
    components: { HeaderButton }
}
</script>

<style scoped>
header {
    width: 100%;
    background: #FFFFFF;
    box-shadow: 0px 4px 31px; 
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
        padding: 32px 64px;

}
.logo {
  filter: drop-shadow(0px 4px 4px rgba(0, 0, 0, 0.1));
}

header:nth-child(-n+1) {
    cursor: pointer;
}
</style>