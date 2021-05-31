<template>
  <div class="body">
    <div class="nar-bar">
      <div class="dis-be">
        <div class="left-box">
          <router-link :to="{name:'home'}">
          <img  class="logo" :src="require('@/assets/image/logo.png')"/>
          </router-link>
        </div>
        <div class="right-box">
          <div >
            <router-link :to="{name:'home'}">猩营销ABOUT US</router-link>
          </div>
          <div><router-link :to="{name:'services-solutions'}">猩方案SOLUTION</router-link>
          </div>
          <div>
            <router-link :to="{name:'case-presentation'}">
              猩案列CASES
            </router-link>
          </div>
          <router-link :to="{name:'list-cases'}">
          <div> 猩观点POINT</div>
          </router-link>
          <router-link :to="{name:'news'}">
          <div>猩学院STUDY</div>
          </router-link>
        </div>
      </div>
    </div>
    <router-view></router-view>
    <bottom></bottom>
  </div>
</template>
<script>
  import bottom from '@/components/bottom'
  export default {
    data() {
      return {}
    },
    components:{
      bottom
    }
  }
</script>
<style lang="scss" scoped>
  .body{
    width: 100%;
  }
  .nar-bar{
    margin:  0 auto;
    width: 100%;
    background: #ffed00;
    height: 2rem;
    line-height: 2rem;
  }
  .logo{
     width: 64px;
  }
  .left-box{
    display: flex;
    align-items: center;
    margin-left: 36px;
    align-items: center;
    img{
      display: flex;
      align-items: center;
    }
  }
  .right-box{
    display: flex;
    align-items: center;
  }
  .dis-be{
    display: flex;
     width: 1400px;
    justify-content: space-between;
    align-items: center;
    margin:  0 auto;
    align-content: center;
    a{
      font-size: 0.8rem;
      color: #898667 !important;
    }
    div{
      font-size: 0.8rem;
      color: #898667 !important;
      margin-right: 31px;
    }
  }
</style>