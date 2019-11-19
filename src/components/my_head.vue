<template>
    <div class="container">
        <header>
            <div class="myheader">
                <div class="myheader_left">
                    <img src="../assets/img/logo.png" alt="">
                </div>
                <div class="myheader_center">
                    <ul> 
                        <li class="links"><router-link class="active" to="">发现</router-link></li>
                        <li class="links"><router-link  to="">我的音乐</router-link></li>
                        <li class="links"><router-link  to="">音乐人</router-link></li>
                        <li class="links"><router-link  to="">客户端下载</router-link></li>
                        <li class="links"><router-link  to="">会员中心</router-link></li>
                    </ul>
                </div>
                <div class="myheader_right">
                        <input class="my_input" type="text">
                        <router-link  to="" class="my_search" ></router-link>
                    <div class="d2_login">
                        <router-link  to="/login">登录</router-link>/
                        <router-link  to="/login">注册</router-link>
                    </div>
                </div>
            </div>
        </header>
    </div>
</template>
<script>
    
</script>
<style lang="less" scoped>
.container{
margin: 0 auto;
}
.myheader{
    display: flex;
    margin: 0 100px;
}
.myheader_left{
  height: 70px;
  line-height: 70px;
}

.myheader_left>img{
width:108px;
height:30px;
vertical-align: middle;
margin-right: 20px;
}
.myheader_center{
    width: 480px;
    height:70px;
    flex-grow: 2;
}
.myheader_center>ul{
    list-style: none;
    display: flex;
}
.myheader_center ul .links>a,.myheader_right .d2_login>a{
font-size:16px;
line-height: 70px;
color: #4a4a4a;
padding:0 20px;
text-decoration: none;
font-weight: 300;
transform:color .2s;
white-space: nowrap;
}
.myheader_center ul .links>a:hover{
    color:#f00;
}
.myheader_center ul .links>a.active{
font-weight: bold;
color: inherit;
}
.myheader_right{
    width:240px;
    height:70px;
    white-space: nowrap;
    display: flex;
    position: relative;
}
.myheader_right .my_input{
    border: 0;
    box-shadow: 0;
    outline: none;
    border-bottom: #000 solid 1px;
    width: 105px;
    height:32px;
    text-overflow: ellipsis;
    font-size: 100%;
    transition:width .3s;
    position: relative;
    top:20px;
}
.myheader_right .my_search{
    display: block;
    width:18px;height: 18px;
    border-radius: 100%;
    border: 1px solid #000;
    position: relative;
    margin: 0;
    top:25px;
    
}
.myheader_right .my_search:after{
    content: "";
    display: block;
    transform:rotate(45deg);
    width: 5px; height: 1px;
    position: absolute;
    top:17px;left: 15px;
    background-color: #000;
}
.myheader_right .d2_login{
margin-left: 30px;
}
.myheader_right .d2_login>a{
    padding: 0;
    
}


</style>