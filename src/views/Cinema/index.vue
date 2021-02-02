<template>
  <div id="main">
    <headerTab :title="title"/>
    <div id="content">
      <div class="cinema_menu">
        <div class="city_switch">
          全城<i class="iconfont icon-lower-triangle"></i>
        </div>
        <div class="brand_switch">
          品牌<i class="iconfont icon-lower-triangle"></i>
        </div>
        <div class="feature_switch">
          特色<i class="iconfont icon-lower-triangle"></i>
        </div>
      </div>
    </div>
    <ci-list />
    <tab-bar />
  </div>
</template>
<script>
import headerTab from '@/components/HeaderTab';
import tabBar from '@/components/TabBar';
import CiList from '@/components/CiList';
export default {
  name:'Cinema',
  components:{
      headerTab,
      tabBar,
      CiList
  },
  data(){
     return{
       title:"喵喵影院"
     }
   }
};
</script>

<style scoped>
#content .cinema_menu{
  width:100%;
  height:45px;
  border-bottom:1px solid #e6e6e6;
  display:flex;
  justify-content: space-around;
  align-items: center;
  background: white;
}
</style>
