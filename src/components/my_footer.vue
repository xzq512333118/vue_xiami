<template>
        <div class="container">
                <div class="my_foot_top">
                    <div class="my_foot">
                        <div>
                            <ul class="footer_ul">
                                <li><a class="footer_title" href="">关于虾米</a></li>
                                <li><a href="">关于我们</a></li>
                                <li><a href="">虾米招聘</a></li>
                                <li><a href="">联系我们</a></li>
                                <li><a href="">知识产权声明及隐私权政策</a></li>
                                <li><a href="">联系客服</a></li>
                                <li><a href="">意见反馈</a></li>
                                <li><a href="">回旧版</a></li>
                            </ul>
                        </div>
                        <div>
                                <ul class="footer_ul">
                                    <li><a class="footer_title" href="">入驻虾米</a></li>
                                    <li><a href="">音乐人</a></li>
                                    <li><a href="">音乐专栏</a></li>
                                </ul>
                        </div>
                        <div>
                                    <ul class="footer_ul">
                                        <li><a class="footer_title" href="">资料补全</a></li>
                                        <li><a href="">添加资料</a></li>
                                        <li><a href="">大家想要的专辑</a></li>
                                        <li><a href="">音频上传</a></li>
                                        <li><a href="">MV上传</a></li>
                                    </ul>
                        </div>
                        <div>
                            <ul class="footer_ul">
                                <li><a class="footer_title" href="">桌面端</a></li>
                                <li><a href="">PC电脑</a></li>
                                <li><a href="">苹果电脑</a></li> 
                            </ul>
                        </div>
                        <div>
                            <span class="footer_title">合作伙伴</span>
                            <img src="../assets/img/footer_img/)FBZRD@Z(`YQA8P86[A7_[I.png" alt="">
                        </div>
                    </div>
                    <div class="my_footer_center">
                            <p>关于我们</p>
                            <img src="../assets/img/footer_img/JV`PPO}4WB95JHL{S(DPKBC.png" alt="">
                    </div>
                    <div class="my_footer_right">
                        <p>虾米音乐App</p>
                        <img src="../assets/img/footer_img/TB1td6jIpOWBuNjy0FiXXXFxVXa-300-300.png" alt="">
                    </div>
                </div>
                <div class="my_footer_b">
                    <div class="my_footer_b_one">
                        <ul>
                            <li><a href="">淘宝网</a></li>
                            <li><a href="">天猫</a></li>
                            <li><a href="">支付宝</a></li>
                            <li><a href="">飞猪</a></li>
                            <li><a href="">聚划算</a></li>
                            <li><a href="">阿里云</a></li>
                            <li><a href="">阿里妈妈</a></li>
                            <li><a href="">1688</a></li>
                        </ul>
                    </div>
                    <div>
                            © 2007 - 2019 杭州阿里巴巴音乐科技有限公司
                    </div>
                </div>
                <div class="my_footer_b">
                    <div class="my_footer_b_two">
                        <ul>
                            <li><a href="">Alios</a></li>
                            <li><a href="">阿里通讯</a></li>
                            <li><a href="">万网</a></li>
                            <li><a href="">UC</a></li>
                            <li><a href="">阿里游戏</a></li>
                            <li><a href="">大麦网</a></li>
                            <li><a href="">一淘</a></li>
                            <li><a href="">狂野飙车9</a></li>
                        </ul>
                    </div>
                    <div>
                            浙网文[2018]3192-218号 浙ICP备18050417号-2 阿里巴巴旗下网站
                    </div>
                </div>
            </div>
</template>
<script>
     
</script>
<style scoped>
.container{
    background-color: #1a1a1a;
    padding: 20px 0px 114px;
    margin: 0 auto;
}
.my_foot_top{
    display: flex;
    margin: 0 auto;
    max-width: 1170px;
    min-width: 850px;
    border-bottom:1px solid #333;
    padding-bottom:2rem;
    margin-bottom: 20px;
}
.footer_ul,.my_footer_b ul{
    display: flex;
    list-style: none;
}
.footer_ul>li>a,div .footer_title{
    color: #fff;
    margin-right: 15px;
    font-size:12px;
   
}
.footer_ul .footer_title, div .footer_title{
    color: #999999;
    display: inline-block;
    width:56px; 
    font-weight: 300;
}
.my_foot>div~div{
    margin-top: 15px;
}
div .footer_title+img{
    vertical-align: top;
}
.my_footer_center{
    margin-left:12rem;
}
.my_footer_right{
    margin-left:7rem;
}
.my_footer_b{
    display: flex;
    justify-content: space-between;
    margin: 0 auto;
    max-width: 1170px;
    min-width: 850px;
}
.my_footer_center>p,.my_footer_right>p,.my_footer_b ul li a{
    color: #999;
    font-weight: 300;
    font-size:12px;
    margin-bottom:10px; 
    transition: color;
}
.my_footer_b ul li a:hover{
    color: #fff;
}
.my_footer_right>img{
width: 150px;
}
.my_footer_b>div>ul>li+li::before{
    color: #4d4d4d;
    content:"|";
    padding: 0 8px;
}
.my_footer_b .my_footer_b_one+div,.my_footer_b .my_footer_b_two+div{
font-size: 12px;
font-weight: 300;
color: #4d4d4d;
}
</style>