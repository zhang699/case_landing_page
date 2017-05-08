<template>
  <div class="nav-bar center-flex-items">
    <div class="nav-bar-content center-flex-items">
    <img src="../assets/work.svg" class="title-icon" />
    <h3 class="title">{{title}}</h3>
    <ul class="nav-bar-items center-flex-items">
      <ol v-for="item in items" class="nav-bar-item">
        <div>
          {{item}}
        </div>
      </ol>
    </ul>
    </div>
  </div>

</template>

<script>
  export default {
    name: 'NavBar',
    data() {
      return {
        items : ['服務內容', '趕快聯絡'],
        title: '全端工作坊',
      }
    }
  }
</script>

<style lang="scss">
  @import '~scss-utils/scss-utils.scss';
  @import '../assets/common.scss';


  $BACKGROUND_COLOR : white;
  $FONT_COLOR: black;
  $NAV_BAR_HEIGHT: 60px;
  .nav-bar-items {
  }
  .title-icon {
    width: 36px;
    height: 36px;
  }
  .nav-bar {
    position: fixed;
    top: 0;
    width: 100%;
    height: $NAV_BAR_HEIGHT;
    background-color: $BACKGROUND_COLOR;
    z-index: 99;
    color: $FONT_COLOR;
    border-bottom: 2px solid #ccc;
  }
  @include respond-to(350px) {
    .nav-bar {
      
      h3 {
        font-size: 16px;
      }

      ol {
        font-size: 10px;
      }
    }
  }
   .nav-bar + * {
     margin-top: $NAV_BAR_HEIGHT;
   }

  .nav-bar-content {
    margin: 10px 10px;
    height: 100%;
    width: 100%;
  }
  .title {
    color: $FONT_COLOR;
  }

</style>