<template>
  <div class="home">
    <head-nav-bar></head-nav-bar>
    <div class="home-content">
      <div class="content-aside">
        <div class="aside-top">
            <img class="aside-img" src="@/assets/logo.png">
        </div>
      </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import HeadNavBar from "@/components/headNavBar"

export default {
  name: 'HomeView',
  components: {
    HeadNavBar
  }
}
</script>

<style lang="less" scoped>

.home {
  width: 100%;
  height: 100%;
  position: relative;
  z-index: 2;
  &::after {
    content: '';
    box-shadow: 0 0 4px 3px rgba(0, 0, 0, .05);
    position: absolute;
    top: 0;
    bottom: 0;
    width: inherit;
    z-index: -1;
  }
}
.home-content{
  width: 100%;
  z-index: 2;
}
.content-aside{
  width: 232px;
  .aside-top{
    width: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 20px 20px;
    .aside-img{
      width: 114px;
      height: 114px;
      border-radius: 50%;
      background-color: red;
      transition: all 1s;
      cursor: pointer;
      &:hover{
        transform: rotateZ(720deg) scale(1.2);
      }
    }
  }
}
</style>
