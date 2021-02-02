<template>
<div class="city_body">
    <div class="city_list">
        <div class="city_hot">
            <h2>熱門城市</h2>
            <ul class="clearfix">
                <li>上海</li>
                <li>北京</li>
                <li>上海2</li>
                <li>北京2</li>
                <li>上海3</li>
                <li>北京3</li>
            </ul>
        </div>
        <div class="city_sort">
            <div>
                <h2>a</h2>
                <ul>
                    <li>阿拉聯盟</li>
                    <li>安山</li>
                    <li>安裝</li>
                    <li>安陽</li>
                </ul>
            </div>
            <div>
                <h2>b</h2>
                <ul>
                    <li>阿拉聯盟2</li>
                    <li>安山2</li>
                    <li>安裝2</li>
                    <li>安陽2</li>
                </ul>
            </div>
            <div>
                <h2>c</h2>
                <ul>
                    <li>阿拉聯盟3</li>
                    <li>安山3</li>
                    <li>安裝3</li>
                    <li>安陽3</li>
                </ul>
            </div>
            <div>
                <h2>d</h2>
                <ul>
                    <li>阿拉聯盟4</li>
                    <li>安山4</li>
                    <li>安裝4</li>
                    <li>安陽4</li>
                </ul>
            </div>
        </div>
    </div>
     <div class="city_index">
        <ul>
            <li>a</li>
            <li>b</li>
            <li>c</li>
            <li>d</li>
        </ul>  
    </div>
</div>
</template>

<script>
export default {
    name:'City'
}
</script>
<style scoped>
    #content .city_body{
        /* margin-top:45px; */
        display:flex;
        width:100%;
        /* position:absolute; */
        top:0;
        bottom:0;
    }
    .city_body .city_list{
        flex:1;
        overflow:auto;
        background: #fff5f0;
    }
    .city_body .city_list::-webkit-scrollbar{
        background-color:transparent;
        width:0;
    }
    /* .city_body .city_hot{
        margin-top:20px;
    } */
    .city_body .city_hot h2{
        padding-left:15px;
        line-height:30px;
        font-size:14px;
        background: #f0f0f0;
        font-weight: normal;
    }
    .city_body .city_hot ul li{
        float:left;
        background:#fff;
        width:29%;
        height:33px;
        margin-top:15px;
        margin-left:3%;
        padding:0 4px;
        border:1px solid #e6e6e6;
        border-radius:3px;
        line-height: 33px;
        text-align:center;
        box-sizing:border-box;
    }
    .city_body .city_sort div{
        margin-top:20px;
    }
    .city_body .city_sort h2{
        padding-left:15px;
        line-height: 30px;
        font-size:14px;
        background:#f0f0f0;
        font-weight: normal;
    }
    .city_body .city_sort ul{
        padding-left:10px;
        margin-top:10px;
    }
    .city_body .city_sort ul li{
        line-height: 30px;
    }
    .city_body .city_index{
       
       display: flex;
        width:20px;
        flex-direction:column;
        justify-content:center;
        text-align:center;
        border-left:1px #e6e6e6 solid;
    }

</style>