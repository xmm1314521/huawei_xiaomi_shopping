<template>
  <div>
    <!-- menu -->
    <header>
      <ul id="menu">
        <li>
          <input id="check02" type="checkbox" name="menu" />
          <label for="check02"><span style="color: white;">=</span></label>
          <ul class="submenu">
            <li><a href="#">首页</a></li>
            <li>
              <router-link to="/mi">
                <a href="#">小米官网</a>
              </router-link>
            </li>
       
          </ul>
        </li>
      </ul>
    </header>
    <!--侧边导航-->
    <div id="cebiandaohang_div">
      <nav class="mainMenu">
        <ul>
          <li><a href="#a1" class="active" data-target="a1">手机</a></li>
          <li><a href="#a2" data-target="a2">笔记本电脑</a></li>
          <li><a href="#a3" data-target="a3">精品平板</a></li>
          <li><a href="#a4" data-target="a4">智能穿戴</a></li>
          <li><a href="#a5" data-target="a5">智慧屏</a></li>
          <li><a href="#a6" data-target="a6">智能家居</a></li>
          <li><a href="#a7" data-target="a7">热销配件</a></li>
          <li><a href="#a8" data-target="a8">生态精品</a></li>
          <li><a href="#a9" data-target="a9">精选配件</a></li>
        </ul>
      </nav>
    </div>
    <div>
      <!--头部-->
      <div><Header></Header></div>
      <!--侧边菜单-->
      <div style="margin-top:60px"><top-banner></top-banner></div>
    </div>

    <!--顶部轮播-->
    <slider></slider>
    <!--公告-->
    <br /><br /><br />
    <lastNav></lastNav>
    <!--热销-->
    <Hot></Hot>
    <!--产品列表-->
    <Product></Product>
    <!--底部-->
    <Footer></Footer>
  </div>
</template>

<script>
import Header from '@/components/huawei/Header.vue'
import lastNav from '@/components/huawei/lastNav.vue'
import Footer from '@/components/huawei/Footer.vue'
import Hot from '@/components/huawei/Hot.vue'
import Product from '@/components/huawei/Product.vue'
import slider from '@/components/huawei/slider.vue'
import TopBanner from '@/components/huawei/TopBanner.vue'
export default {
  name: 'huawei',
  components: {
    Header,
    lastNav,
    Footer,
    Hot,
    Product,
    slider,
    'top-banner': TopBanner
  },
  data() {
    return {}
  },
  computed: {},
  methods: {}
}
</script>
<style scoped></style>
