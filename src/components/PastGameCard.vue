<template>
  <div class="swItem">
    <div class="swItem__values">
      <div class="swItem__values__main">
        <span>
          <span class="title--bold"> id: </span>
          1101001
        </span>
        <span>
          <span class="title--bold">Creator:</span>
          33123
        </span>
        <span>
          <span class="title--bold">Map:</span>
          taeoisr
        </span>
      </div>
      <div class="swItem__values__status">
        <span><span class="title--bold">Status:</span> Waiting for an opponent</span>
      </div>
      <div class="swItem__values__bet">
        <span><span class="title--bold">Bet per round:</span> 1 ROSE</span>
        <span><span class="title--bold">To deposit:</span> 25 ROSE</span>
      </div>
     
    </div>
    <div class="swItem__button">
      <div class="swItem__button__title">Current round 0/12</div>
      <div class="swItem__button__btn">
        <header-button>Join</header-button>
      </div>
    </div>
  </div>
   <div class="gameStatus">
        <div class="gameStatus__header">
           Players & stats: 
        </div>
        <div class="gameStatus__list">
          <div class="gameStatus__list__item">
              <div>0x23D...P11t (you): </div>
              <div>10 kills, 10 deaths, dep 22 Rose</div>
          </div>
            <div class="gameStatus__list__item">
                <div>Win: 8 ROSE</div>
                <div>Lose: 0 ROSE</div>
          </div>
          <div class="gameStatus__list__item">
              
                  <div>
                      0x4u5...Gt4k (enemy): 
                  </div>
                  <div>
                        6 kills, 6 deaths, dep 22 Rose
                  </div>
           
          </div>
          <div class="gameStatus__list__item">
                <div>Win: 0 ROSE</div>
                <div>Lose: 8 ROSE</div>
          </div>
        </div>
      </div>
</template>

<script>
import HeaderButton from "./HeaderButton.vue";
export default {
  components: { HeaderButton },
};
</script>

<style lang="scss" scoped>
.swItem {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  &__values {
    display: flex;
    flex-direction: column;
    gap: 20px;
    align-items: flex-start;
    &__main {
      display: flex;
      gap: 30px;
    }
  }
  &__button {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
  }
}
.gameStatus{
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    gap: 20px;
    border-bottom: 1px solid black;
    padding-bottom: 30px;
    &__list{
        display: flex;
        flex-direction: row;
        gap: 20px;
        &__item{
            display: flex;
            flex-direction: column;
            align-items: flex-start;
            font-size: 14px;
        }
    }
    }
    .title{
        &--bold{
            font-weight: 500;
        }
    }
</style>
