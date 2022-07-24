<template>
  <div class="head-nav-bar">
    <div class="name">
      <div class="name-logo">
        <img src="@/assets/logo.jpg">
      </div>
    </div>
    <div>

    </div>
  </div>
</template>

<script>
export default {
  name: "HeadNavBar"
}
</script>

<style lang="less" scoped>
.head-nav-bar {
  width: 100%;
  background-color: #FFFFFF;
  padding: 12px 28px;
  display: flex;
  align-items: center;
  position: relative;
  &::after{
    position: absolute;
    content: '';
    top: 0;
    bottom: 0;
    width: inherit;
    left: 0;
    box-shadow: 0 2px 2px 2px rgba(0, 0, 0, .05);
  }
  .name {
    display: flex;
    align-items: center;

    .name-logo {
      width: 36px;
      height: 36px;
      border-radius: 50%;
      padding: 6px;
      background-color: #000000;

      img {
        width: 100%;
        height: 100%;
        border-radius: 50%;
      }
    }
  }
}
</style>