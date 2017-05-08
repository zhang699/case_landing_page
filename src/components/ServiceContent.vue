<template>
  <section class="service-content">
    <div class="center-flex-items header">
      <h1>服務內容</h1>
    </div>
    <hr/>
    <div class="center-flex-items flex-wrap">
      <div class="column pad column-center-flex-item">
        <h2>企業內部培訓</h2>
        <p>協助企業導入React.js + Node.js 的全端開發</p>
      </div>
      <div class="column pad column-center-flex-item">
        <img src="../assets/configuration.svg" class="content-img" />
      </div>
    </div>
    
    <div class="center-flex-items flex-wrap">
      <div class="column pad column-center-flex-item pull-left">
        <h2>影像辨識</h2>
        <p class="description">協助企業使用Google Cloud Vision 進行影像處理</p>
      </div>
      <div class="column pad column-center-flex-item">
        <img src="../assets/eye.svg"
            class="content-img" />
      </div>

    </div>
  </section>
</template>
<script>
  export default {
    name: 'ServiceContent',
    data() {
      return {

      }
    }
  }
</script>

<style lang="scss" scoped>

  @import '../assets/common.scss';
  .service-content {

  }
  .description {
  }
  .header {
    color: black;
  }
  hr {
    border-color: black;
  }

 
</style>