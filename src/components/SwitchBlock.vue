<template>
    <div class="switchBlock">
        <div class="switchBlock__swithcer">
            <p @click="switchState = 1" :class="switchState == 1 ? 'switchBlock__swithcer__chosen' : '' ">Open game</p>
            <p @click="switchState = 2" :class="switchState == 2 ? 'switchBlock__swithcer__chosen' : ''">Past game</p>
        </div>
        <div v-if="switchState === 1" style="height: 400px; overflow-y: scroll">
        <div v-for="i in 6" :key="i.id">
        <OpenGameCard />
        </div>
        </div>
        <div v-if="switchState ===2">
            <PastGameCard />
        </div>
    </div>
</template>

<script>
import OpenGameCard from './OpenGameCard.vue';
import PastGameCard from './PastGameCard.vue';
export default {
  components: { OpenGameCard, PastGameCard },
    data() {
        return {
            switchState: 1,
        };
    }
}
</script>

<style scoped>
.switchBlock {
    background: #FFFFFF;
    box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.25);
    border-radius: 24px;
    max-width: 864px;
    width: 100%;
    margin: 0 auto;
    padding: 30px 80px;
}
.switchBlock__swithcer {
    margin: 0 auto;
    display: flex;
    max-width: 234px;
    justify-content: space-between;
    width: 100%;
    border-bottom: 3px solid #FF7C06;
    font-weight: 700;
    font-size: 20px;
    line-height: 24px;
}
.switchBlock__swithcer:nth-child(-n+2) {
    cursor: pointer;
}
.switchBlock__swithcer__chosen {
    color: #FF7C06;
    border-bottom: 3px solid #FF7C06;
}
</style>