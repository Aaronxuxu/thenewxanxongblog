<template>
  <div class="footer">
    <div class="footer-warning">
      <div class="footer-fs-title">鸡汤</div>
      <div class="footer-fs-main">
        <p>有志者事竟成</p>
        <p>多学习少做梦</p>
        <p>对得住自己亦要对得住别人</p>
      </div>
    </div>
    <div class="footer-warning">
      <div class="footer-fs-title">鸡汤</div>
      <div class="footer-fs-main">
        <p>有志者事竟成</p>
        <p>多学习少做梦</p>
        <p>对得住自己亦要对得住别人</p>
      </div>
    </div>
    <div class="footer-contact">
      <div class="footer-fs-title">联系方式</div>
      <div class="footer-fs-main">
        <p>www.xanxong.com</p>
        <p>+86 13129189764</p>
        <p>a470164479@gmail.com</p>
      </div>
    </div>
  </div>
</template>

<script lang="ts" setup>
</script>

<style lang="less" scoped>
.footer {
  display: flex;
  align-items: center;
  justify-content: space-around;
  padding: 25px;
  min-height: 220px;
  background-color: #1f1f1f;
  color: #fff;

  .footer-fs-title {
    line-height: 2;
    font-size: 23px;
    font-weight: 700;
  }
  .footer-fs-main {
    font-size: 18px;
    line-height: 2;
  }
  @media (max-width: 728px) {
    flex-direction: column;
    align-items: flex-start;
  }
}
</style>