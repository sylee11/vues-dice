<template>
  <div>
      <button class="control btn-new"><i class="ion-ios-plus-outline"></i>GAME TÀI XỈU</button>
            <button class="control btn-roll"
                v-on:click="reNewGame"
            ><i class="ion-ios-loop"></i>Roll dice</button>
            <!-- <button class="control btn-hold"><i class="ion-ios-download-outline"></i>Hold</button> -->
            <!-- <input type="number" placeholder="Final score" class="final-score"> -->
  </div>
</template>

<script>
export default {
    name : 'controler',
    data() {
        return {}
    },
    methods : {
        reNewGame(){
            this.$emit('handleReNewGame')
        }
    }
}
</script>

<style>

</style>