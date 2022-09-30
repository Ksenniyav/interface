<template>
    <header>
        <div class='logo'>
            <img src="../content/titleHeader.svg" alt="">
        </div>
        <div class='button1'>
        <HeaderButton />
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
    display: absolute;
    width: 1920px;
    height: 120px;
    left: 0px;
    top: 0px;
    background: #FFFFFF;
    box-shadow: 0px 4px 31px; 
}
.logo {
    position: absolute;
    width: 200px;
    height: 56.77px;
    left: 64px;
    top: 32px;
    filter: drop-shadow(0px 4px 4px rgba(0, 0, 0, 0.1));
}

header:nth-child(-n+1) {
    cursor: pointer;
}
</style>