<template>
  <div class="mycom">
    <p>名前: <slot name="name">tanizawakenta</slot></p>
    <p>住所: <slot name="address">kamata</slot></p>
    <p>name:<slot :userNm="userNm">{{ userNm.enName }}</slot></p>
  </div>
</template>
<script>
export default {
  name: 'MyCom',
  data () {
    return {
      userNm: {
        enName: 'Tanizawa Kenta',
        jpName: '谷澤健太' // ←slot内で参照したいデータ
      }
    }
  }
}
</script>
<style>
</style>