<template>
    <div class="nav-bar">
      <slot></slot>
    </div>
</template>

<script>
    export default {
        name: "NavigationBar"
    }
</script>

<style scoped>
.nav-bar {
  display: flex;
  height: 44px;
  background-color: #ff322d;
}
</style>
