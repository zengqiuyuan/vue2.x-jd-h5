<template>
 <div id="tab-bar">
   <slot></slot>
 </div>
</template>
<script>
  export default {
    name:'TabBar'
  }
</script>
<style>
  #tab-bar{
    display: flex;
    background-color: rgba(238, 238, 238, 0.22);
    font-size: 20px;
    position: fixed;
    left: 0;
    right: 0;
    bottom: 0;
    box-shadow: 0 -1px 1px rgba(128, 128, 128, 0.25);
  }
</style>
