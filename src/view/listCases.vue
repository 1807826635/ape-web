<template>
  <div class="wrap">
    <div class="home-top">
      <div class="top-img">
        <div class="min-width padding-top">
        </div>
      </div>
    </div>
    <div class="flex min-width mar-top">
      <div class="">
        <div>重庆涪陵 福音国际教育 携手 中国猩营销</div>
        <div class="gey-text">成功招生700人，业绩实收62万    执行老师郭伦行</div>
      </div>
      <div class="yellow">2016.6.30</div>
    </div>
    <div class="min-width">
      <div class="yellow-box"></div>
      <img :src="require('@/assets/image/one-1.png')" class="one">
      <div class="evaluate">学员评价Student evaluation</div>
      <img :src="require('@/assets/image/two-2.png')" class="one">
      <div class="evaluate">客户评价Customer evaluation</div>
      <img :src="require('@/assets/image/three-3.png')" class="one">
      <div class="person">
        <div class="left-box">
          <img :src="require('@/assets/image/three-3.png')" class="head">
          <div >深圳红舞鞋 </div>
          <div>负责人 小玉</div>
        </div>
        <div class="right-box">
          认真负责，用心的为校区考虑，设心处地的寻找符合当地的方案，全体员工通过此次活动，
          <br>
          学习到很多很实在的专业知识，并可以在日后的教学
        </div>
      </div>
      <div class="share">

      </div>
    </div>
    <div></div>
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
  .top-img {
    height: 32rem;
    width: 100%;
    background: url("../assets/image/home_2.png");
    background-size: 100% 100%;
    object-fit: cover;
    .top-text-z {
      color: #ffffff;
      font-size: 3.4rem;
    }
  }
  .flex{
     display: flex;
    align-items: center;
    justify-content: space-between;
  }
  .min-width{
    width: 1400px;
    margin: 0 auto;
  }
  .gey-text{
    font-size: 0.8rem;
    color: #8f8f8f;
  }
  .yellow{
    padding: 7px 9px 7px 9px;
    background: #ffed00;
    color: #000000;
    font-size: 1rem;
    border-radius: 3px;
  }
  .yellow-box{
    width: 30px;
    height: 6px;
    margin-top: 60px;
    background: #ffed00;
    margin-bottom: 50px;
  }
  .one{
    width: 100%;
  }
  .mar-top{
    margin-top: 70px;
  }
  .evaluate{
    font-weight: 600;
    color: #000000;
    font-size: 2rem;
    margin-top: 93px;
    margin-bottom: 60px;
  }
  .person{
    padding: 72px 86px 49px 109px;
    display: flex;
    .left-box{
      margin-right: 110px;
      div:first-child{
        margin-top: 30px;
      }
      div {
        white-space: nowrap;
        font-size: 0.8rem;
      }
    }
    .head{
      width: 72px;
      height: 72px;
      border-radius: 50%;
    }
    .right-box{
      font-size: 0.8rem;
      color: #000;
      line-height: 2rem;
    }
  }
</style>