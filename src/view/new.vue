<template>
  <div class="wrap">
    <div class="home-top">
      <div class="top-img">
        <div class="min-width padding-top">
          <div class="top-text-z">新闻动态</div>
          <div class="top-text-q">APE NEWS</div>
          <div class="yellow-box"></div>
          <div class="sub-text">
            <div>猩动态Marketing</div>
            <div>行业新闻Educational</div>
            <div>知识分享Knowledge</div>
          </div>
        </div>
      </div>
    </div>
    <div class="content min-width">
      <div class="item-tr">
        <div class="item-box">
          <img :src="require('@/assets/image/news.png')" class="news">
          <div class="dis-flex"> <div class="yellow-tips">2021.6.30</div></div>
          <div class="tittle">中国猩营销开工大吉</div>
          <div class="sub-text-z">期盼在新的一年里携手进取，共创佳绩！ 牛年大家一起牛起来</div>
          <div class="more">more</div>
        </div>
        <div class="item-box">
          <img :src="require('@/assets/image/news.png')" class="news">
          <div class="dis-flex"> <div class="yellow-tips">2021.6.30</div></div>
          <div class="tittle">中国猩营销开工大吉</div>
          <div class="sub-text-z">期盼在新的一年里携手进取，共创佳绩！ 牛年大家一起牛起来</div>
          <div class="more">more</div>
        </div>
        <div class="item-box">
          <img :src="require('@/assets/image/news.png')" class="news">
          <div class="dis-flex"> <div class="yellow-tips">2021.6.30</div></div>
          <div class="tittle">中国猩营销开工大吉</div>
          <div class="sub-text-z">期盼在新的一年里携手进取，共创佳绩！ 牛年大家一起牛起来</div>
          <div class="more">more</div>
        </div>
      </div>
      <div class="item-tr">
        <div class="item-box">
          <img :src="require('@/assets/image/news.png')" class="news">
          <div class="dis-flex"> <div class="yellow-tips">2021.6.30</div></div>
          <div class="tittle">中国猩营销开工大吉</div>
          <div class="sub-text-z">期盼在新的一年里携手进取，共创佳绩！ 牛年大家一起牛起来</div>
          <div class="more">more</div>
        </div>
        <div class="item-box">
          <img :src="require('@/assets/image/news.png')" class="news">
          <div class="dis-flex"> <div class="yellow-tips">2021.6.30</div></div>
          <div class="tittle">中国猩营销开工大吉</div>
          <div class="sub-text-z">期盼在新的一年里携手进取，共创佳绩！ 牛年大家一起牛起来</div>
          <div class="more">more</div>
        </div>
        <div class="item-box">
          <img :src="require('@/assets/image/news.png')" class="news">
          <div class="dis-flex"> <div class="yellow-tips">2021.6.30</div></div>
          <div class="tittle">中国猩营销开工大吉</div>
          <div class="sub-text-z">期盼在新的一年里携手进取，共创佳绩！ 牛年大家一起牛起来</div>
          <div class="more">more</div>
        </div>
      </div>
      <div class="item-tr">
        <div class="item-box">
          <img :src="require('@/assets/image/news.png')" class="news">
          <div class="dis-flex"> <div class="yellow-tips">2021.6.30</div></div>
          <div class="tittle">中国猩营销开工大吉</div>
          <div class="sub-text-z">期盼在新的一年里携手进取，共创佳绩！ 牛年大家一起牛起来</div>
          <div class="more">more</div>
        </div>
        <div class="item-box">
          <img :src="require('@/assets/image/news.png')" class="news">
          <div class="dis-flex"> <div class="yellow-tips">2021.6.30</div></div>
          <div class="tittle">中国猩营销开工大吉</div>
          <div class="sub-text-z">期盼在新的一年里携手进取，共创佳绩！ 牛年大家一起牛起来</div>
          <div class="more">more</div>
        </div>
        <div class="item-box">
          <img :src="require('@/assets/image/news.png')" class="news">
          <div class="dis-flex"> <div class="yellow-tips">2021.6.30</div></div>
          <div class="tittle">中国猩营销开工大吉</div>
          <div class="sub-text-z">期盼在新的一年里携手进取，共创佳绩！ 牛年大家一起牛起来</div>
          <div class="more">more</div>
        </div>
      </div>
      <submint></submint>
    </div>
  </div>
</template>

<script>
  import submint from '@/components/submitInput'
  export default {
    data() {
      return {}
    },
    components:{
      submint
    }
  }
</script>

<style scoped lang="scss">
  .wrap{
    padding-bottom: 147px;
    .home-top {
      .top-img {
        height: 32rem;
        width: 100%;
        background: url("../assets/image/home_4.png");
        background-size: 100% 100%;
        object-fit: cover;
        .top-text-z {
          color: #ffffff;
          font-size: 3.4rem;
        }
      }
    }
    .top-text-q {
      color: #ffffff;
      font-size: 2.4rem;
    }
    .padding-top {
      padding-top: 5.95rem;
      padding-left: 3.8rem;
    }
    .yellow-box {
      background: #ffed00;
      width: 30px;
      height: 6px;
      margin-top: 1.8rem;
      margin-bottom: 1.8rem;
    }
    .sub-text {
      display: flex;
      color: #ead800;
      font-size: 1rem;
      div {
        margin-right: 1rem;
      }
    }
    .item-tr{
      margin-top: 14px;
      display: flex;
      justify-content: space-between;
    }
    .item-box{
      width: 295px;
      height: 525px;
      margin-right: 27px;
    }
    .min-width{
      width: 1400px;
      margin: 0 auto;
    }
    .news{
      width: 100%;
    }
    .yellow-tips{
      font-size: 12px;
      padding: 3px 9px 3px 9px;
      background: #ffed00;
      color: #000000;
      display: flex;
      border-radius: 10px;
    }
    .dis-flex{
      display: flex;
      margin-top: 26px;
      margin-bottom: 28px;
    }
    .tittle{
      font-weight: bold;
      font-size: 20px;
      color: #000000;
      margin-bottom: 20px;
    }
    .sub-text-z{
      font-size: 16px;
      color: #8f8f8f;
    }
    .more{
      color: #000000;
      font-size: 18px;
      margin-top: 15px;
    }
  }
</style>