<template>
  <div class="bottom">
    <img :src="require('@/assets/image/bottom-logo.png')" class="one-png">
    <img :src="require('@/assets/image/bottom-text.png')" class="two-png">
    <img :src="require('@/assets/image/bottom-code.png')" class="three-png">
    <img :src="require('@/assets/image/bottom-bottom.png')" class="four-png">
  </div>
</template>
<script>
  export default {
    data() {
      return {}
    }
  }
</script>
<style scoped lang="scss">
  .bottom{
    width: 100%;
    background: #ffed00;
    padding-top: 2rem;
    padding-bottom: 1rem;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    .one-png{
      width: 160px;
    }
    .two-png{
      width:100%;
      margin-top: 26px;
    }
    .three-png{
      width: 160px;
      margin-top: 40px;
    }
    .four-png{
      width: 172px;
      margin-top: 40px;
    }
  }
</style>