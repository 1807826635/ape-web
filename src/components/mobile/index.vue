<template>
  <div>
    <div class="ni-hao">你好</div>
    <div class="hao">好</div>
  </div>
</template>

<script>

  import CallApp from 'callapp-lib';

  export default {
    name: 'HelloWorld',
    data() {
      return {
        msg: 'Welcome to Your Vue.js App'
      }
    },
    mounted() {
      console.log()
    },
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .ni-hao {
    font-size: 0.8rem;
  }

  .hao {
    font-size: 16px;
  }
</style>
