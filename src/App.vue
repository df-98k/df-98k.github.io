<template>
  <div id="app">
    <!-- 顶部 Header 区域 -->
    <mt-header fixed title=" Vue项目" class="header"></mt-header>

    <!-- 中间的 路由 router-view 区域  主要是路由的内容-->
<transition mode='out-in' >
      <router-view>



      </router-view>
</transition>
  

    <!-- 底部 TabBar 区域 -->
    <nav class="mui-bar mui-bar-tab">
      <router-link to="/home" class="mui-tab-item ">
        <span class="mui-icon mui-icon-home"></span>
        <span class="mui-tab-label">首页</span>
      </router-link>
      <router-link to="/member" class="mui-tab-item">
        <span class="mui-icon mui-icon-email"></span>
        <span class="mui-tab-label">会员</span>
      </router-link>
      <router-link to="/shopcar" class="mui-tab-item">
        <span class="mui-icon mui-icon-home mui-icon-extra-cart mui-icon-extra">
          <span class="mui-badge">0</span>
        </span>

        <span class="mui-tab-label">购物车</span>
      </router-link>
      <router-link to="/search" class="mui-tab-item">
        <span class="mui-icon mui-icon-search"></span>
        <span class="mui-tab-label">搜索</span>
      </router-link>
    </nav>
     


  </div>
</template>

<script>


</script>


<style lang="scss" scoped>

 
	.v-enter, 
	.v-leave-to {
		opacity: 0;
	}
	.v-enter {
		transform: translateX(100%);
	}
	.v-leave-to {
		transform: translateX(-100%);
		position: absolute;
	}
	.v-enter-active,
	.v-leave-active {
		transition: all .4s ease;
	}

  
#app{
  padding-top: 40px;
  	overflow-x: hidden;
}

</style>
