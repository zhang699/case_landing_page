<template>
  <section class="service-content">
    <div class="center-flex-items header">
      <h1>服務內容</h1>
    </div>
    <hr/>
    <div class="center-flex-items flex-wrap">
      <div class="column pad column-center-flex-item">
        <h2>企業內部培訓</h2>
        <p class="service-content-text">協助企業導入React.js + Node.js 全端開發。套用時下最流行的 Javascript 全端技術，讓培訓人員在<b><u>三個月</u></b>內學會前後端開發，無論是<b><u>IoT的即時監控或社群相關應用程式</u></b>都能夠駕馭自如。</p>
      </div>
      <div class="column pad column-center-flex-item">
        <img src="../assets/configuration.svg" class="content-img" />
      </div>
    </div>
    
    <div class="center-flex-items flex-wrap">
      <div class="column pad column-center-flex-item pull-left">
        <h2> 協助企業使用 Google Cloud Vision 影像辨識</h2>
        <p class="service-content-text">Google Vision 是強大的影像處理服務，可以辨識上千種物品，然後進行分類。應用在<b><u>證件辨識系統</u></b>上，可以節省可觀的人力成本。</p>
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
  .service-content-text {
    line-height: 30px;
    text-align: left;
  }
  .pad {
    padding: 20px 20px;
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