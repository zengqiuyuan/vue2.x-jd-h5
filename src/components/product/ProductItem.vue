<template>
    <div class="product-item">
      <div class="product-item-img">
        <slot name="product-item-img"></slot>
      </div>
      <div class="product-item-desc">
        <slot name="product-item-desc"></slot>
      </div>
      <div class="product-item-price">
        <div class="product-item-money">
          <slot name="product-item-price"></slot>
        </div>
        <div class="product-item-lable">
          <slot name="product-item-lable"></slot>
        </div>
      </div>
    </div>
</template>

<script>
    export default {
        name: "ProductItem"
    }
</script>

<style scoped>
  .product-item{
    width: 45%;
    padding-bottom: 0;
    border-radius: 0.4rem;
    overflow: hidden;
    float: left;
    margin-top: 10px;
    margin-left: 10px;
    font-size: 14px;
    box-shadow: 0 0px 1px #fbfff8;
    background-color: white;
  }
  .product-item-desc{
    box-sizing: border-box;
    word-break: break-all;
    overflow:hidden;
    text-overflow:ellipsis;
    display:-webkit-box;
    -webkit-box-orient:vertical;
    -webkit-line-clamp:2;
    padding: 0 4px;
  }
  .product-item-price{
    font-size: 13px;
    overflow: hidden;
    position: relative;
    height: 1.3rem;
    right: 40px;
    padding-bottom: 10px;
    margin-top: 5px;
  }
  .product-item-money{
    color: #fa2c19;
    display: inline-block;
    margin-right: 10px;
  }
  .product-item-lable{
    border: 1px solid #fa2c19;
    color: #fa2c19;
    display: inline-block;
    font-size: 12px;
    padding: 0 3px;
    margin-right: 5px;
    line-height: 14px;
    height: 14px;
    border-radius: 0.1rem;
  }

</style>
