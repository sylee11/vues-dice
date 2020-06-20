<template>
  <div>
      <div class="player-panel" v-bind:class="{'winner': isWin == 0 }">
                <div class="player-name">TÀI</div>
                <div class="player-score">{{isWin == 0 ? point : ''}}</div>
            </div>
            
            <div class="player-panel" v-bind:class="{'winner': isWin == 1  }">
                <div class="player-name"  >XỈU</div>
                <div class="player-score">{{isWin == 1 ? point : ''}}</div>
            </div>
  </div>
</template>

<script>
export default {
    name: 'TaiXiu',
    data(){
        return {}
    },
    props : {
        point: Number,
        isWin : Number
    }
}
</script>

<style>

</style>