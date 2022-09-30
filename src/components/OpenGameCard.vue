<template>
  <div class="swItem">
        <div class="swItem__values">
          <div class="swItem__values__main">
                  <span>
                      <span>
                          id:
                      </span>
                      1101001
                  </span>
                  <span>
                      <span>Creator:</span>
                      33123
                  </span>
                  <span>
                      <span>Map:</span>
                      taeoisr
                  </span>
              </div>
          
          <div class="swItem__values__status">
         <span><span>Status:</span> Waiting for an opponent</span>  
          </div>
          <div class="swItem__values__bet">
              <span><span>Bet per round:</span> 1 ROSE</span>
              <span><span>To deposit:</span> 25 ROSE</span>
          </div>
        </div>
      <div class="swItem__button">
          <div class="swItem__button__title">
              Current round 0/12
          </div>
          <div class="swItem__button__btn">
              <header-button>Join</header-button>
          </div>
      </div>
      </div>
</template>

<script>
import HeaderButton from './HeaderButton.vue'
export default {
  components: { HeaderButton },

}
</script>

<style lang="scss" scoped >
.swItem{
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    border-bottom: 1px solid black;
    &__values{
        display: flex;
        flex-direction: column;
        gap: 20px;
        align-items: flex-start;
        &__main{
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
</style>