<template>
  <div id="main">
 
      <headerTab :title="title"/>
        <div id="content">
          <div class="movie_menu">
            <router-link tag="div" to="/movie/city" class="city_name">
                <span>大連</span>
                <i>
                  <img src="/images/triangle.png">
                </i>
            </router-link>
            <div class="hot_switch">
                <router-link tag="div" to="/movie/nowPlaying" class="hot_item">正在熱映</router-link> 
                <router-link tag="div" to="/movie/comingSoon" class="hot_item">即將上映</router-link>
            </div>
            <router-link tag="div" to="/movie/search" class="search_entry">
                <i>
                  <img src="/images/search.png">
                </i>
            </router-link>
          </div>
          <keep-alive>
            <router-view />
          </keep-alive>

        </div>
      <tab-bar /> 
  </div>
  
 
</template>
<script>
import headerTab from '@/components/HeaderTab';
import tabBar from '@/components/TabBar';
export default {
   name:'Movie',
   components:{
     headerTab,
     tabBar
   },
   data(){
     return{
       title:"喵喵電影"
     }
   }
};
</script>

<style scoped>
/* #content{
  flex:1;
  overflow:auto;
  margin-bottom:50px;
  position: relative;
  display:flex;
  flex-direction:column;
} */
#content .movie_menu{
  width:100%;
  
  border-bottom:2px solid #e6e6e6;
  display:flex;
  justify-content: space-between;
}
.movie_menu .city_name{
  margin-left:20px;
  height:100%;
  width:60px;
  line-height: 44px;
  display:flex;
  justify-content: center;
  align-items:center;
  padding-top:2px;
}
.movie_menu .city_name i{
  width:10px;
  height:10px;
  margin-left:5px;
}

  /* display:flex;
  margin-top:-27px;
  height:10px;
 
  margin-left:40px; */
  /* line-height: 45px;
   width:10px;
  display:flex;
  justify-content: center;
  align-items:center */

.movie_menu .city_name img{
  width:100%;
  height:100%;
}
.movie_menu .city_name.active{
  color:#ef4238;
  border-bottom:2px #ef4238 solid;

}
.movie_menu .city_name.router-link-active{
  color:#ef4238;
  border-bottom:2px #ef4238 solid;

}
.movie_menu .hot_switch{
  display:flex;
  height:100%;
  line-height:45px;
}
.movie_menu .hot_item{
  font-size:15px;
  color:#666;
  width:80px;
  text-align:center;
  margin:0 12px;
  font-weight: 700;
}
.movie_menu .hot_item.active{
  color:#ef4238 ;
  border-bottom:2px #ef4238 solid;
}
.movie_menu .hot_item.router-link-active{
  color:#ef4238 ;
  border-bottom:2px #ef4238 solid;
}
.movie_menu .search_entry{
  margin-right:20px;
  width:20px;
  line-height: 45px;
  display:flex;
  justify-content: center;
  align-items:center;
  height: 45px;
}
.movie_menu .search_entry.active{
  color:#ef4238;
  border-bottom:2px #ef4238 solid;
}
.movie_menu .search_entry.router-link-active{
  color:#ef4238;
  border-bottom:2px #ef4238 solid;
}
.movie_menu .search_entry img{
  width:100%;
  height:100%;
}
</style>