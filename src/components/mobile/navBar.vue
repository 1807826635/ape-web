<template>
  <div class="body">
    <div class="nar-bar">
      <div class="menu">
        <div class="line-box">
          <div  @click="menuClick()" :class="{ middleline: true, menulineactive: sidebarIsShow }">
            <!--<div class="middleline"></div>-->
          </div>
        </div>
      </div>
    </div>
    <transition name="side-op">
      <div class="sidebarbgc"@click="menuClick"  v-if="sidebarIsShow">
        <div class="sidebarwhite" @click.stop="onStop" :class="{ graybgc: true, graybgcactive: sidebarIsShow,transformLeft: showLeft}">
            <div class="">
              <div class="menu-item-box">
                <div><router-link :to="{name:'mobile-index'}">首页</router-link></div>
                <div>猩营销ABOUT US</div>
                <div>猩方案SOLUTION</div>
                <div>猩案列CASES</div>
                <div> 猩观点POINT</div>
                <div>猩学院STUDY</div>
              </div>
            </div>
        </div>
      </div>
    </transition>
    <router-view></router-view>
    <bottom></bottom>
  </div>
</template>
<script>
  import bottom from '@/components/mobile/bottom'

  export default {
    data() {
      return {
        sidebarIsShow: false,
        showLeft: false
      }
    },
    methods: {
      menuClick() {
        this.sidebarIsShow = !this.sidebarIsShow
        setTimeout(()=>{
          this.showLeft =  !this.showLeft
        },200)
      },
      onGoTo(name){
        this.$router.push(name)
      },
      onStop(){}
    },
    components: {
      bottom
    }
  }
</script>
<style lang="scss" scoped>
  .body {
    position: relative;
    z-index: 9;
    width: 100%;
    .nar-bar {
      position: fixed;
      top: 0px;
      margin: 0 auto;
      width: 100%;
      background: #ffed00;
      height: 64px;
      z-index: 12;
      line-height: 64px;
    }
   .menu{
     position: relative;
   }
    .logo {
      width: 64px;
    }
    .middleline {
      z-index: 3;
      display: inline-block;
      line-height: 65px;
      width: 55px;
      height: 5px;
      border-radius: 3px;
      background-color: #ffffff;
      position: relative;
      transition: all 0.5s ease;
      &::before { //前一条线
        content: "";
        position: absolute;
        width: 55px;
        height: 5px;
        bottom: 17px;
        border-radius: 3px;
        background-color: #ffffff;
        transition: all 0.5s ease;
      }
      &::after { //后一条线
        content: "";
        position: absolute;
        width: 55px;
        height: 5px;
        top: 17px;
        border-radius: 3px;
        background-color: #ffffff;
        transition: all 0.5s ease;
      }
    }
    .menulineactive {
      display: inline-block;
      z-index: 3;
      line-height: 65px;
      width: 55px;
      height: 5px;
      border-radius: 3px;
      background-color: #ffffff;
      position: relative;
      transform: rotate(45deg); //中间的线顺时针旋转45°

      &::before {
        content: "";
        position: absolute;
        width: 55px;
        height: 5px;
        bottom: 0px;
        border-radius: 3px;
        background-color: #ffffff;
        transition: all 0.5s ease;
        opacity: 0;
      }
      &::after {
      transform: rotate(-90deg); //上方的线逆时针旋转90°
      transform-origin: 19px -6px;
      }
    }
    .sidebartransition {
      &-enter {
        transform: translateX(-100%); //整体划入之前隐藏在最左侧
      }
      &-enter-active {
        transition: all1s ease; //划入过渡，用时0.5s
      }
      &-leave-to {
        transform: translateX(-120%); //整体划出之后隐藏在最左侧，之所以设置为-120%，见后文
      }
      &-leave-active {
        transition: all 1s ease; //划出过渡，用时0.5s
      }
    }
    .side-op{
      &-enter {
        opacity: 0;

      }
      &-enter-active {
        transition: all 0.5s ease; //划入过渡，用时0.5s
      }
      &-leave-to {
        opacity: 0;
      }
      &-leave-active {
        transition: all 0.5s ease; //划出过渡，用时0.5s
      }
    }
    .transformLeft{
      transform: translateX(0%) !important;
      transition: all 0.5s ease; //划出过渡，用时0.5s
    }
    .sidebarwhite{
      transition: all 0.5s ease; //划出过渡，用时0.5s
      transform: translateX(-100%);
    }
    .graybgc {
      position: absolute;
      height: 100%;
      z-index: 11;
      background: #ffffff;
    }
    .graybgcactive {
      width: 69%; //当侧边栏显示时，即sidebarIsShow为true时，灰色滑块变动宽度为120%
    }
    .line-box{
      position: absolute;
      right: 0.5rem;
    }
    .sidebarbgc {
      position: fixed;
      top: 0;
      left: 0;
      z-index: 10;
      width: 100%;
      height: 100%;
      background: rgba(19, 19, 19, 0.3);
    }
    .menu-item-box{
      display: flex;
      flex-direction: column;
      padding-top: 22px;
      padding-left: 15px;
      margin-top: 71px;
      a:active {
        color: #ffed00;
      }
      a{
        color: #000000;
      }
      div{
        margin-bottom: 25px;
        color: #000000;
        font-size: 13px;
        opacity: 0.8;
      }
    }
  }

</style>