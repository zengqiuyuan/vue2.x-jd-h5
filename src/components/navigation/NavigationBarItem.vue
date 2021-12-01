<template>
    <div class="nav-item">
      <div class="nav-item-left">
        <slot name="nav-item-left"></slot>
      </div>
      <div class="nav-item-center">
        <slot name="nav-item-center"></slot>
      </div>
      <div  class="nav-item-left">
        <slot name="nav-item-right"></slot>
      </div>
    </div>
</template>

<script>
    export default {
        name: "NavigationBarItem"
    }
</script>

<style scoped>
  .nav-item{
    width: 100%;
    display: flex;
    text-align: center;
    line-height: 44px;
    color: white;
    font-size: 15px;
  }
  .nav-item-left{
    width: 50px;
    height: 44px;
    margin-left: 10px;
    margin-right: 10px;
  }
  .nav-item-center{
    width: 100%;
    height: 44px;
  }
</style>
