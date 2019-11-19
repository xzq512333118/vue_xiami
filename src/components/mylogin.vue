<template>
        <div class="login_conten"> 
                <div class="login_inner">      
                   <div class="my_loginsty"> 
                       <router-link to="/" class="span"></router-link>
                       <video src="../assets/img/login_img/a29ccbee1e9a1624832ef6d32c80225b.mp4" loop muted autoplay="autoplay"></video>
                       <img src="../assets/img/login_img/TB1e63KC1uSBuNjy1XcXXcYjFXa-170-210.png" alt="">
                   </div>
                   <div class="login_form" :class="zhuceno">
                       <div class="login_form_tab">
                           <span title="扫码登录" :class="smclass"  @click="qiehuan(-1)"></span>
                           <span title="账户登录" :class="zhclass"  @click="qiehuan(1)"></span>
                       </div>
                       <div class="login_qrcode" :class="zhclass" data-qie="zqie">
                           <div>扫码登录</div>
                           <div></div>
                           <div>
                                  虾米APP扫一扫，登录安全又快速<br>
                                  虾米APP - 个人中心 - 右上角
                           </div>
                       </div>
                       <div class="login_inpt" :class="smclass" data-qie="zqie">
                           <div>
                               <span data-sp="zhshou" :class="styclass" @click="zhangshou(1)">账户登录</span>
                               <span data-sp="zhshou" :class="ctyclass" @click="zhangshou(-1)">手机验证码</span>
                           </div>
                        <div class="login_zhanghu " data-sp="zhangphone" :class="dsclass">
                           <div>
                               <label for="account">账号</label>
                               <input id="account" type="text" placeholder="请输入邮箱或手机">
                           </div>
                           <div>
                                  <label for="account">密码</label>
                                  <input id="password" type="password" placeholder="请输入密码">
                           </div> 
                           <div id="drag">
                                  <div class="drag_bg"></div>
                                  <div class="drag_text">向右滑动</div>
                                  <div class="handler handler_bg">&gt;&gt;</div>
                           </div>
                           <div>
                              <button class="btn" >登录</button>
                           </div>
                           <div>
                               <router-link  to="" @click.native="zhuc1(1)" >注册</router-link><router-link to="">忘记密码？</router-link>
                           </div>
                           <div>
                               <router-link to=""><img src="../assets/img/login_img/taobaologo.png" alt=""></router-link>
                               <router-link to=""><img src="../assets/img/login_img/weibologo.png" alt=""></router-link>
                               <router-link to=""><img src="../assets/img/login_img/weixinlogo.png" alt=""></router-link>
                               <router-link to=""><img src="../assets/img/login_img/qq_logo.png" alt=""></router-link>
                           </div>
                         </div>
                         <!-- 手机登录界面 -->
                         <div class="login_phone" :class="daclass" data-sp="zhangphone">
                             <div>
                                 <label for="">手机号</label>
                                 <span>+86</span>
                                 <input type="text" placeholder="请输入手机号">
                             </div>
                             <div id="drag">
                                  <div class="drag_bg"></div>
                                  <div class="drag_text">向右滑动</div>
                                  <div class="handler handler_bg">&gt;&gt;</div>
                              </div>
                             <div>
                                 <label for="">验证码</label>
                                 <input type="text" placeholder="请输入验证码"><button>发送验证码</button>
                             </div>
                             <div>
                                 <button class="btn" >登录</button>
                             </div>
                             <div>
                                 <router-link  to="" @click.native="zhuc1(1)">注册</router-link>
                                 <router-link to="">联系客服</router-link>
                            </div>
                         </div>
                       </div>
                   </div>
                   <!-- 注册页面html -->
                   <div class="zhuce_content" :class="zhuce">
                       <div>
                           <span>新用户注册</span><span>轻松两步即可完成注册</span>
                       </div>
                      <div>
                          <label for="">手机号</label>
                          <span>+86</span>
                          <input type="text" placeholder="请输入手机号">
                      </div>
                      <div id="drag">
                           <div class="drag_bg"></div>
                           <div class="drag_text">向右滑动</div>
                           <div class="handler handler_bg">&gt;&gt;</div>
                       </div>
                      <div>
                          <label for="">验证码</label>
                          <input type="text" placeholder="请输入验证码"><button>发送验证码</button>
                      </div>
                      <div>
                          <button class="btn">注册</button>
                      </div>
                      <div>
                          <span><input type="radio">
                              我同意
                                  <router-link to="//act.xiami.com/wow/xiami/act/protocol" target="_blank" rel="noreferrer noopener">虾米音乐用户服务协议</router-link><br>
                                  及<router-link to="//act.xiami.com/wow/xiami/act/legal-agreement" target="_blank" rel="noreferrer noopener">知识产权声明及隐私权政策</router-link>
                          </span>
                      </div>
                      <div>
                          <router-link to="" @click.native="zhuc1(-1)">返回登录</router-link>
                      </div>
                   </div>
                </div>
              </div>
</template>
<script>
export default {
data(){
    return{
         smclass:{
             dengshao:true,
         },
         zhclass:{
             dengshao:false
         },
         styclass:{
             sty:true,
         },
         ctyclass:{
             sty:false,
         },
         dsclass:{
            dengshao:false 
         },
         daclass:{
             dengshao:true
         },
         zhuce:{
            zhucenone:true
         },
         zhuceno:{
            zhucenone:false
         }
    }
},
methods:{
qiehuan(e){
    if(e==1){
      this.zhclass.dengshao=true
      this.smclass.dengshao=false
    }else{
      this.zhclass.dengshao=false
      this.smclass.dengshao=true
    }
},
zhangshou(e){
 if(e==1){
     this.styclass.sty=true;
     this.ctyclass.sty=false;
     this.dsclass.dengshao=false;
     this.daclass.dengshao=true;
 }else{
    this.styclass.sty=false;
     this.ctyclass.sty=true;
     this.dsclass.dengshao=true;
     this.daclass.dengshao=false;
 }
},
zhuc1(e){
    if(e==1){
    this.zhuce.zhucenone=false
    this.zhuceno.zhucenone=true
 }else{
    this.zhuce.zhucenone=true
    this.zhuceno.zhucenone=false
 }
}
}

}
</script>
<style scoped>
    .login_inner{
    width:600px;
    height: 470px;
    display: flex;
    position: fixed;
    top: 50%;
    left: 50%;
    margin-left: -300px;
    margin-top: -235px;
}
/* 点击注册加class */
.login_inner .zhucenone{
display: none;
}
/* 左侧 */
.login_inner .my_loginsty{
    height: 470px;
    position: relative;
}
.login_inner .my_loginsty .span{
background-image: url("../assets/img/login_img/gb_img.png");
background-size: cover;
display: block;
width: 20px;
height: 20px;
position: absolute;
top: 5px;
left: 15px;
z-index: 1000;
}
.login_inner .my_loginsty>span:hover{
    cursor: pointer;
}
.login_inner .my_loginsty video{
    width: 220px;
    height:470px;
}
.login_inner .my_loginsty img{
    width: 86px;
    height: 106px;
    position: absolute;
    top: 50%;
    left:50%;
    margin-top: -53px;
    margin-left: -43px;
    
}
/* 右侧 账号登录界面右上角 */
.login_inner .login_form{
    width: 360px;
    height: 470px;
    background-color: #fff;
    box-sizing: border-box;
}
.login_inner .login_form_tab{
    width: 56px;
    position: absolute;
    right: 20px;
}
.login_inner .login_form_tab>:first-child{
    display: block;
    background-image: url("../assets/img/login_img/smdl.png");
    width:56px;
    height: 56px;
}
.login_inner .login_form_tab>:first-child:hover{
    cursor:pointer;
}
.login_inner .login_form_tab>:last-child{
    display: block;
    background-image: url("../assets/img/login_img/zhdl.png");
    width:56px;
    height: 56px;
   
}
/* 点击切换登录或扫码图片 */
.login_inner .login_form_tab .dengshao{ 
    display: none;
}
.login_inner .login_form_tab>:last-child:hover{
    cursor:pointer;
}
/* 账号登录内容 */
.login_inner .login_inpt,.login_inner .login_qrcode{
    padding:56px 40px 0;
}
/* 点击切换账号页面或二维码页面 */
.login_inner  .dengshao{
display: none;
}
.login_inner .login_inpt>:first-child{
    margin-bottom: 35px;
}
.login_inner .login_inpt>:first-child span{
    font-size: 18px;
    color:#999;
    cursor: pointer;
}
.login_inner .login_inpt>:first-child>:first-child{
    margin-right: 32px;
}  
/* 点击切换账号或手机登录 */
.login_inner .login_inpt div .sty{
    font-weight: bold;
    color: #ff410f
}
.login_inner .login_inpt .login_zhanghu.dengshao,.login_inner .login_inpt .login_phone.dengshao{
display: none;
}
.login_inner .login_inpt .login_zhanghu{
    display: flex;
    flex-direction: column;
}
 .login_inner .login_inpt .login_zhanghu div~div{
    margin: 20px 0 0 0;
} 
.login_inner .login_inpt .login_zhanghu div:nth-child(1) label,.login_inner .login_inpt div:nth-child(2) label,.login_inner .login_inpt .login_phone div:first-child>label,.login_inner .login_inpt .login_phone div:nth-child(3)>label{
    display: block;
    margin-bottom: 10px;
    color: #999;
    font-size: 12px;
}
.login_inner .login_inpt .login_zhanghu div:nth-child(1) input,.login_inner .login_inpt .login_zhanghu div:nth-child(2) input,.login_inner .login_inpt .login_phone div:first-child>input,.login_inner .login_inpt .login_phone div:nth-child(3)>input{
    border:none;
    width:100%;
    height: 30px;
    border-radius: 5px;
    background-color: #f7f7f7;
    outline: none;
}
/* 拖拽验证 */
.login_conten #drag{ 
    position: relative;
    background-color: #e8e8e8;
    width: 280px;
    height: 34px;
    line-height: 34px;
    text-align: center;
    border-radius: 5px;
}
#drag .handler{
    position: absolute;
    top: 0px;
    left: 0px;
    width: 40px;
    height: 32px;
    border: 1px solid #ccc;
    cursor: move;
    margin-top:0;
    text-align: center;
}
.handler_bg{
    background: #fff  no-repeat center;
}
.handler_ok_bg{
    background: #fff  no-repeat center;
}
#drag .drag_bg{
    background-color: #7ac23c;
    height: 34px;
    width: 0px;
}
#drag .drag_text{
    position: absolute;
    top: -20px;
    width: 280px;
}
/* 登录按钮 */
.zhuce_content div:nth-child(5) button,.login_inner .login_inpt .login_zhanghu div:nth-child(4) button,.login_inner .login_inpt .login_phone div:nth-child(3)>button,.login_inner .login_inpt .login_phone div:nth-child(4)>button{
    font-size: 24px;
    border-radius: 16px;
    width: 100%;
    height: 48px;
    color:#ccc;
    background-color: #f2f2f2;
    cursor: not-allowed;
    border: none;
    outline: none;
}
.login_inner .login_inpt .login_zhanghu div:nth-child(5),.login_inner .login_inpt .login_phone div:last-child{
    display: flex;
    justify-content: space-between;
    align-items: center;
}
.login_inner .login_inpt .login_zhanghu div:nth-child(5) a,.login_inner .login_inpt .login_phone div:last-child a,.login_inner .login_inpt .login_zhanghu div:nth-child(3) >span,.login_inner .login_inpt .login_phone div:nth-child(2)>span{
text-decoration: none;
color: #4a4a4a;
font-size: 12px;
}
.login_inner .login_inpt .login_zhanghu div:last-child{
    display: flex;
    justify-content: center;
    align-items: center;
}
.login_inner .login_inpt .login_zhanghu div:last-child :last-child>img{
margin-left: 10px; 
}
/* 手机验证码内容 */
.login_inner .login_inpt .login_phone div:first-child~div{
margin: 20px 0 0 0;
} 
.login_inner .login_inpt .login_phone div:first-child>input,.login_inner .login_inpt .login_phone div:nth-child(3)>input{
    width: 170px;
}
.login_inner .login_inpt .login_phone div:nth-child(3)>button,.zhuce_content div:nth-child(4) button{
width:100px;
height: 30px;
font-size: 12px;
border-radius: 5px;
}
.login_inner .btn{
background-color: #ff410f !important;
cursor: pointer !important;
color: #fff !important;
}
/* 右侧扫码登录界面内容 */
.login_inner .login_qrcode div:first-child{
    font-size: 18px;
    font-weight: 700;
    color: #4a4a4a;
    text-align: center;
    margin-bottom: 50px;
}
.login_inner .login_qrcode div:nth-child(2){
    background-image: url("../assets/img/login_img/O1CN0164a6NX1GQAWd1oNky616-2-xcode.png");
    background-size: cover;
    width: 168px;
    height: 168px;
    margin: 0 auto;
}
.login_inner .login_qrcode div:last-child{
    font-size: 12px;
    color: #4a4a4a;
    margin-top: 15px;
    text-align: center;
}
/* 以下为注册页面css */
/* 设置注册页面大小 */
.zhuce_content{
    width: 360px;
    height: 470px;
    padding: 64px 40px 0;    
    background-color:#fff;
    box-sizing: border-box;
}
/* 设置标题大小颜色 */
.zhuce_content div:first-child span:first-child{
    font-size: 18px;
    font-weight: bold;
}
/* 设置标题行第二个span样式 */
.zhuce_content div:first-child span:first-child+span{
    margin-left: 8px;
    font-style: normal;
    font-size: 12px;
    color: #999;
}

.zhuce_content div:nth-child(2)>label,.zhuce_content div:nth-child(4)>label{
    display: block;
    margin-bottom: 10px;
    color: #999;
    font-size: 12px;
}
.zhuce_content div:nth-child(2) input{
    width: 170px;
}

.zhuce_content div:nth-child(2) input,.zhuce_content div:nth-child(4) input{
    border: none;
    width: 64%;
    height: 30px;
    border-radius: 5px;
    background-color: #f7f7f7;
    outline: none;
}
.zhuce_content div:nth-child(4) button{
    color: #ccc;
    background-color: #f2f2f2;
    cursor: not-allowed;
    border: none;
    outline: none;
}

.zhuce_content div:nth-child(6){
    margin-top: -10px!important;
    font-size: 12px;
    line-height: 20px;
    color: #999;
    text-align: center;
    margin-top: 20px !important;
}
.zhuce_content div~div{
    margin-top: 20px;
}
.zhuce_content div:last-child{
    text-align: center;
}
.zhuce_content div:last-child>a{
    font-size: 12px;
    color: #4a4a4a;
}
.handler .handler_bg{
    text-align: center;
}
</style>