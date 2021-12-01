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
        <div class="product-item-tag">
          <slot name="product-item-tag"></slot>
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
  .product-item-img{

  }
  .product-item-desc{
    height: 40px;
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
    padding-bottom: 10px;
  }
  .product-item-money{
    color: #fa2c19;
    display: inline-block;
    padding: 0 5px 0 4px;
    position: relative;
    top: 1px;
    height: 25px;
    line-height: 25px;
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
  .product-item-tag{
    display: block;
    position: absolute;
    top: 0.15rem;
    right: -0.3em;
    text-align: center;
    color: grey;
    font-size: .5rem;
    height: 1.1rem;
    line-height: 1.1rem;
    padding: 0 0.5em;
    background-color: #f0f2f5;
    border-radius: 0.55rem;
  }

</style>
