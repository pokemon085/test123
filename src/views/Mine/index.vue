<template>
    <div id="main">
 
      <headerTab :title="title"/>
      <div id="content">
        <login />
      </div>
      <tab-bar /> 
  </div>
</template>
<script>
import headerTab from '@/components/HeaderTab';
import tabBar from '@/components/TabBar';
import login from '@/components/Login';
export default {
   name:'Mine',
   components:{
     headerTab,
     tabBar,
     login
   },
   data(){
     return{
       title:"我的喵喵"
     }
   }
};
</script>

<style></style>