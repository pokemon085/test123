<template>
    <div class="movie_body">
        <ul>
            <li>
                <div class="pic_show">
                    <img src="/images/movie_1.jpg"></div>
                <div class="info_last">
                    <h2>無名之輩</h2>
                    <p>觀眾評
                        <span class="grade">9.2</span></p>
                    <p>主演: AAA,BBB,CCC</p>
                    <p>今天55家影院放映607場</p>
                </div>
                <div class="btn_mail">
                    購票
                </div>
            </li>
            <li>
                <div class="pic_show"><img src="/images/movie_2.jpg"></div>
                <div class="info_last">
                    <h2>致命守護者</h2>
                    <p>觀眾評<span class="grade">9.3</span></p>
                    <p>主演: AAA,BBB,CCC</p>
                    <p>今天55家影院放映443場</p>
                </div>
                <div class="btn_mail">
                    購票
                </div>
            </li>
            <li>
                <div class="pic_show"><img src="/images/movie_1.jpg"></div>
                <div class="info_last">
                    <h2>無名之輩3</h2>
                    <p>觀眾評<span class="grade">9.2</span></p>
                    <p>主演: AAA,BBB,CCC</p>
                    <p>今天55家影院放映607場</p>
                </div>
                <div class="btn_mail">
                    購票
                </div>
            </li>
            <li>
                <div class="pic_show"><img src="/images/movie_2.jpg"></div>
                <div class="info_last">
                    <h2>致命守護者2</h2>
                    <p>觀眾評<span class="grade">9.2</span></p>
                    <p>主演: AAA,BBB,CCC</p>
                    <p>今天55家影院放映607場</p>
                </div>
                <div class="btn_mail">
                    購票
                </div>
            </li>
             <li>
                <div class="pic_show"><img src="/images/movie_1.jpg"></div>
                <div class="info_last">
                    <h2>無名之輩4</h2>
                    <p>觀眾評<span class="grade">9.2</span></p>
                    <p>主演: AAA,BBB,CCC</p>
                    <p>今天55家影院放映607場</p>
                </div>
                <div class="btn_mail">
                    購票
                </div>
            </li>
            <li>
                <div class="pic_show"><img src="/images/movie_2.jpg"></div>
                <div class="info_last">
                    <h2>致命守護者4</h2>
                    <p>觀眾評<span class="grade">9.2</span></p>
                    <p>主演: AAA,BBB,CCC</p>
                    <p>今天55家影院放映607場</p>
                </div>
                <div class="btn_mail">
                    購票
                </div>
            </li>
        </ul>
    </div>
</template>

<script>
export default {
    name:"NowPlaying"
}
</script>
<style scoped>
    #content .movie_body{
        flex:1;
        overflow:auto;
    }
    .movie_body ul{
        margin:0 12px;
        overflow:hidden;
    }
    .movie_body ul li{
        margin-top:12px;
        display:flex;
        align-items:center;
        justify-content: space-between;
        border-bottom:1px #e6e6e6 solid;
        padding-bottom:20px;
    }
    .movie_body .pic_show{
        width:74px;
        height:100px;
    }
    .movie_body .pic_show img{
        width:100%;
    }
    .movie_body .info_list{
        margin-left:20px;
        flex:1;
        position:relative;
    }
    .movie_body .info_list h2{
        font-size:17px;
        line-height: 24px;
        width:150px;
        overflow:hidden;
        white-space: nowrap;
        text-overflow:ellipsis;

    }
    .movie_body .info_list p{
        font-size:13px;
        color:#666;
        line-height:22px;
        width:200px;
        overflow:hidden;
        white-space:nowrap;
        text-overflow:ellipsis;
    }
    .grade{

        font-size:700;
        color:#faaf00;
        font-size:15px;
    }
    .movie_body .info_list .btn-mail{
        margin:0 5px;
    }

    .movie_body .info_list img{
        width:50px;
        position:absolute;
        right:10px;
        top:5px;
    }
    .movie_body .btn_mall , .movie_body .btn_mail{
        width:47px;
        height:27px;
        line-height: 28px;
        text-align:center;
        background-color:#f03d37;
        color:#fff;
        border-radius: 4px;
        font-size: 14px;
        cursor: pointer;
    }
    .movie_body .btn_pre{
        background-color:#3c9fe6
    }
</style>