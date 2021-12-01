<template>
    <div class="category">
      <div class="category-item">
        <slot name="category-img"></slot>
      </div>
      <div class="category-title">
        <slot name="category-title"></slot>
      </div>
    </div>
</template>

<script>
    export default {
        name: "ProductCategoryItem"
    }
</script>

<style scoped>
.category{
  width: 20%;
  text-align: center;
  display: block;
  float: left;
}
.category-item{
  padding-top: 10px;
}
.category-title{
  display: block;
  margin-top: 0.3rem;
  font-size: .6rem;
}
</style>
