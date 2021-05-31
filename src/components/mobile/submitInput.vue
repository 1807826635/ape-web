<template>
  <div class="submit">
    <div class="min-width text-center">
      <img :src="require('@/assets/image/text.png')" class="text-img">
      <div>
        <div class="form">
          <div class="form-tr">
            <input placeholder="姓名" class="flex-input"/>
            <input  placeholder="电话" class="flex-input"/>
          </div>
          <div class="form-tr">
            <input placeholder="机构名称*" class="line-input"/>
          </div>
          <div class="form-tr">
            <input placeholder="机构地址*" class="line-input"/>
          </div>
          <div class="tittle">
            机构情况
          </div>
          <div class="form-tr margin-top">
            <input placeholder="全职员工人数" class="flex-input"/>
            <input  placeholder="兼职员工人数" class="flex-input"/>
          </div>
          <div class="form-tr margin-top">
            <input placeholder="校区数量" class="flex-input"/>
            <input  placeholder="校区总面积" class="flex-input"/>
          </div>
          <div class="form-tr margin-top">
            <input placeholder="创立年数" class="flex-input"/>
            <input  placeholder="在读学院数量" class="flex-input"/>
          </div>
          <div  class="form-tr margin-top" >
            <textarea rows="3" class="area-input"  cols="20"></textarea>
          </div>
          <div class="submit-btn">提交</div>
          <div class="secret">填写资料严格保密，仅用于活动对接咨询，不会泄露给任何第三方</div>
        </div>
      </div>
    </div>
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
  .submit{
    width: 100%;
    margin-top: 7.25rem;
    .text-img{
      width: 21rem;
      margin:  0 auto;
    }
    .text-center{
      text-align: center;
    }
    .min-width{
      width: 100%;
      margin:  0 auto;
    }
    .form{
      width: 26.9rem;
      text-align: center;
      margin:  0 auto;
      margin-top: 2.75rem;
      .form-tr{
        display: flex;
        justify-content: center;
        .flex-input{
          flex: 1;
          margin-right: 0.2rem;
          height: 1.5rem;
          padding-left: 0.7rem;
          font-size: 0.8rem;
        }
      }
      .line-input{
        width: 100%;
        height: 1.5rem;
        padding-left: 0.7rem;
        margin-top: 0.5rem;
        font-size: 0.8rem;
      }
    }
    .margin-top{
      margin-top: 0.5rem;
    }
    .area-input{
      height: 5rem;
      width: 100%;
      font-size: 0.8rem;
    }
    .tittle{
      text-align: left;
      color: #000000;
      font-size: 1rem;
      margin-top: 1.75rem;
      margin-bottom: 1.75rem;
    }
    .secret{
      font-size: 0.5rem;
      color: #000000;
      margin-top: 0.5rem;
    }
    .submit-btn{
      background: #ffed00;
      padding-top: 0.5rem;
      padding-bottom: 0.5rem;
      margin-top: 1.1rem;
      letter-spacing: 15.5px;
    }
  }

</style>