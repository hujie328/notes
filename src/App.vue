<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<style lang="less">
*{
  padding: 0;
  margin: 0;
  outline: none;
  list-style: none;
  border: none;
  box-sizing: border-box;
}
html,body{
  width: 100%;
  height: 100%;
}
@media (max-width: 768px) {
  #app{
    padding: 0;
  }
}
@media (min-width: 1000px) {
  #app{
    padding: 0 200px;
  }
}
#app{
  width: 100%;
  height: 100%;
  overflow: hidden;
  background-color: #efefef;
}
</style>
