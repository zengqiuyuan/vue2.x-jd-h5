<template>
  <div class="tab-bar-item">
    <slot name="item-icon"></slot>
    <slot name="item-text"></slot>
  </div>
</template>
<script>
  export default {
      name:'TabBarItem'
  }
</script>
<style>
  .tab-bar-item{
    flex: 1;
    text-align: center;
    font-size: 14px;
    height: 49px;
    margin-top: 2px;
    margin-bottom: 2px;
    color: #303639;
  }
  .tab-bar-item i {
    height: 25px;
    width: 25px;
  }
</style>
