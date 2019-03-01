<template>
    <div class="btn-frame">
        <div class="single-bar"></div>
        <div class="single-bar"></div>
        <div class="single-bar"></div>
        <div class="single-bar"></div>
        <div class="single-bar"></div>
    </div>
</template>

<script>
export default {
  name: 'btn-frame',
  props: ['barList', 'barLen']
}
</script>

<style lang="scss" scoped>
  .btn-frame{
    position: fixed;
    bottom: 10px;
    width: 3rem;
    box-shadow: 2px 2px 10px #9d9d9d;
    $darkBack:rgb(111,111,111);
    $lightBack:rgb(11,211,211);
    .single-bar:nth-child(2n-1){
      width: 3rem;
      height: 3rem;
      background: $darkBack;
      /*transition: all .5s linear .2s;*/
    }
    .single-bar:nth-child(2n){
      width: 3rem;
      height: 3rem;
      background: $lightBack;
      /*transition: all .2s linear .2s;*/
    }
    .single-bar:hover{
      /*width: 2rem;*/
      /*height: 2rem;*/
    }
  }

</style>
