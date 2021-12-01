<template>
  <div class="view">
    <!--    头部导航搜索-->
    <div class="header">
      <navigation-bar>
        <navigation-bar-item>
          <i slot="nav-item-left" class="iconfont icon-category"></i>
          <div class="nav-center" slot="nav-item-center">
            <span style="color: red;float: left;margin-left: 20px;">JD</span><span style="margin-left: 7px;font-size: 16px;color: #c4cabc;float: left">|</span>
            <input class="nav-center-input" type="text" value="请输入">
          </div>
          <div slot="nav-item-right">登录</div>
        </navigation-bar-item>
      </navigation-bar>
    </div>
    <div class="content">
      <!--      轮播图-->
      <div class="content-rotation-chart">
        <img v-show="index == n"
             v-for="(item,index) in imgList"
             :key="index"
             :src="item" alt="" width="95%">
        <!--        <div class="content-rotation-chart-arrow"></div>-->
        <!--        <div class="content-rotation-chart-arrow"></div>-->
        <div class="content-rotation-chart-li">
          <span v-for="(item1,index1) in imgList" :key="index1" :class="index1 == n ? 'active_span' : ''"></span>
        </div>
      </div>
      <!--      商品分类-->
      <div class="content-category">
        <product-category-item>
          <img slot="category-img" src="../assets/img/category/1.jpg" alt="" width="40px" height="40px">
          <span slot="category-title">京东超市</span>
        </product-category-item>
        <product-category-item>
          <img slot="category-img" src="../assets/img/category/2.jpg" alt="" width="40px" height="40px">
          <span slot="category-title">京东服饰</span>
        </product-category-item>
        <product-category-item>
          <img slot="category-img" src="../assets/img/category/3.jpg" alt="" width="40px" height="40px">
          <span slot="category-title">数码电器</span>
        </product-category-item>
        <product-category-item>
          <img slot="category-img" src="../assets/img/category/1.jpg" alt="" width="40px" height="40px">
          <span slot="category-title">京东超市</span>
        </product-category-item>
        <product-category-item>
          <img slot="category-img" src="../assets/img/category/2.jpg" alt="" width="40px" height="40px">
          <span slot="category-title">京东服饰</span>
        </product-category-item>
        <product-category-item>
          <img slot="category-img" src="../assets/img/category/1.jpg" alt="" width="40px" height="40px">
          <span slot="category-title">京东服饰</span>
        </product-category-item>
        <product-category-item>
          <img slot="category-img" src="../assets/img/category/3.jpg" alt="" width="40px" height="40px">
          <span slot="category-title">京东服饰</span>
        </product-category-item>
        <product-category-item>
          <img slot="category-img" src="../assets/img/category/1.jpg" alt="" width="40px" height="40px">
          <span slot="category-title">京东服饰</span>
        </product-category-item>
        <product-category-item>
          <img slot="category-img" src="../assets/img/category/3.jpg" alt="" width="40px" height="40px">
          <span slot="category-title">京东服饰</span>
        </product-category-item>
        <product-category-item>
          <img slot="category-img" src="../assets/img/category/2.jpg" alt="" width="40px" height="40px">
          <span slot="category-title">京东服饰</span>
        </product-category-item>
      </div>
      <!--      京东秒杀-->
      <div class="content-product-seckill">
        <div class="seckill-more">
          <span>京东秒杀</span>
          <span style="color: #ff322d;float: right">更多秒杀></span>
        </div>
        <div class="seckill-product">
          <div class="seckill-product-item">
            <img src="../assets/img/category/11.jpg" alt="">
            <span>￥88</span>
          </div>
          <div class="seckill-product-item">
            <img src="../assets/img/category/12.jpg" alt="">
            <span>￥68</span>
          </div>
          <div class="seckill-product-item">
            <img src="../assets/img/category/13.jpg" alt="">
            <span>￥38</span>
          </div>
          <div class="seckill-product-item">
            <img src="../assets/img/category/11.jpg" alt="">
            <span>￥88</span>
          </div>
          <div class="seckill-product-item">
            <img src="../assets/img/category/13.jpg" alt="">
            <span>￥38</span>
          </div>
          <div class="seckill-product-item">
            <img src="../assets/img/category/11.jpg" alt="">
            <span>￥88</span>
          </div>
          <div class="seckill-product-item">
            <img src="../assets/img/category/13.jpg" alt="">
            <span>￥38</span>
          </div>
          <div class="seckill-product-item">
            <img src="../assets/img/category/11.jpg" alt="">
            <span>￥88</span>
          </div>
        </div>
      </div>
      <!--      展示商品-->
      <div class="content-product-exhibition">
        <product-item>
          <img slot="product-item-img" src="../assets/img/category/20.png" width="100%" alt="">
          <span slot="product-item-desc">拉面说 招牌日式豚骨叉烧拉面方便速食拌面非油炸拉面216.8g</span>
          <span slot="product-item-price">￥88</span>
          <span slot="product-item-lable">闪购</span>
        </product-item>
        <product-item>
          <img slot="product-item-img" src="../assets/img/category/21.png" width="100%" alt="">
          <span slot="product-item-desc">美国belli孕妇防晒霜孕妇专用护肤品怀孕期哺乳期用化妆品孕产妇隔离霜孕妇BB霜</span>
          <span slot="product-item-price">￥288</span>
          <span slot="product-item-lable">闪购</span>
        </product-item>
        <product-item>
          <img slot="product-item-img" src="../assets/img/category/11.jpg" width="100%" alt="">
          <span slot="product-item-desc">昂秀外语 21天搞定全部英语语法—英语入门英语口语学习必经之路</span>
          <span slot="product-item-price">￥99</span>
          <span slot="product-item-lable">闪购</span>
        </product-item>
        <product-item>
          <img slot="product-item-img" src="../assets/img/category/12.jpg" width="100%" alt="">
          <span slot="product-item-desc">拉面说 招牌日式豚骨叉烧拉面方便速食拌面非油炸拉面216.8g</span>
          <span slot="product-item-price">88</span>
          <span slot="product-item-lable">闪购</span>
        </product-item>
      </div>
    </div>
    <div class="bottom">
      <tab-bar>
        <tab-bar-item>
          <i slot="item-icon" class="iconfont icon-home"></i>
          <div slot="item-text">首页</div>
        </tab-bar-item>
        <tab-bar-item>
          <i slot="item-icon" class="iconfont icon-all"></i>
          <div slot="item-text">分类</div>
        </tab-bar-item>
        <tab-bar-item>
          <i slot="item-icon" class="iconfont icon-cart-Empty"></i>
          <div slot="item-text">购物车</div>
        </tab-bar-item>
        <tab-bar-item>
          <i slot="item-icon" class="iconfont icon-bussiness-man"></i>
          <div slot="item-text">我的</div>
        </tab-bar-item>
      </tab-bar>
    </div>
  </div>
</template>

<script>
  import TabBar from '@/components/tabbar/TabBar'
  import TabBarItem from '@/components/tabbar/TabBarItem'
  import NavigationBar from  '@/components/navigation/NavigationBar'
  import NavigationBarItem from  '@/components/navigation/NavigationBarItem'
  import ProductCategoryItem from '@/components/category/ProductCategoryItem'
  import ProductItem from '@/components/product/ProductItem'
  export default {
    name: 'Home',
    components:{
      TabBar,
      TabBarItem,
      NavigationBar,
      NavigationBarItem,
      ProductCategoryItem,
      ProductItem
    },
    data() {
      return {
        imgList: [
          require('@/assets/img/category/4.jpg'),
          require('@/assets/img/category/5.jpg'),
          require('@/assets/img/category/6.jpg'),
          require('@/assets/img/category/7.jpg'),
          require('@/assets/img/category/8.jpg'),
        ],
        n: 0,
      }
    },
    mounted() {
      this.go()
    },
    methods:{
      go(){
        // this.$post('/Get/list2').then(res => {
        //   console.log(res,"res");
        // });
        setInterval( ()=> {
          this.n++;
          if(this.n == this.imgList.length){
            this.n = 0
          }
        },2000)
      }
    },
  }
</script>

<style>
  body {
    margin: 0;
    padding: 0;
    background-color: #f6f6f6;
  }
  .view{

  }
  .header .bottom{
    height: 50px;
    background: #ddd;
    position: absolute;
    width: 100%;
  }
  .content{
    width: 100%;
    position: absolute;
    top: 50px;
    bottom: 50px;
    overflow-y: auto;
  }
  .content-rotation-chart{
    margin-left: 10px;
    /*height: 150px;*/
  }
  .content-rotation-chart-li{
    position: absolute;
    top: 120px;
    left: 150px;
  }
  .content-rotation-chart-li span.active_span{
    background-color: #ff322d;
  }
  .content-rotation-chart-li span {
    box-sizing: border-box;
    border-radius: 50%;
    height: 0.35rem;
    width: 0.35rem;
    background: hsla(0,0%,100%,.6);
    margin: 0 2px;
    display: inline-block;
    opacity: 1;
  }
  .nav-center{
    height: 30px;
    width: 270px;
    border: 0;
    line-height: 30px;
    border-radius: 15px;
    background-color: white;
    margin-top: 8px;
    color: gray;
  }
  .nav-center-input{
    border: 0;
    width: 100px;
    color: gray;
    position: absolute;
    top: 13px;
    left: 130px;
  }
  .content-category{
    height: 180px;
    color: #666;
  }
  .content-product-seckill{
    box-shadow: 1px 1px 1px #fffdfc;
    background: url("../assets/img/category/8.png");
    background-color: white;
    background-size: contain;
    border-radius: 0.6rem;
    overflow: hidden;
    padding-bottom: 15px ;
    width: 93%;
    margin-left: 10px;
  }
  .seckill-more{
    height: 2.5rem;
    margin-top: 0.4rem;
    margin-right: 0.25rem;
    margin-left: -13rem;
    font-size: .8rem;
    color: #333;
  }
  .seckill-product {
    width: 100%;
    color: red;
    box-sizing: border-box;
    overflow: scroll;
    white-space: nowrap;
    display: flex;
  }
  .seckill-product::-webkit-scrollbar {
    display: none;
  }
  .seckill-product-item{
    display: flex;
    flex-direction: column;
    margin-left: 11px;
  }
  .seckill-product-item img{
    width: 45px;
    height: auto;
  }
  .seckill-product-item span{
    margin-top: 5px;
    font-size: 12px;
  }
</style>
