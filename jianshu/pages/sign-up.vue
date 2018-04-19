<template>
  
  <div class="sign">
       <!-- logo -->
    <div class="logo">
        <nuxt-link to="/">
            <img src="~/assets/img/logo.png" alt="">
        </nuxt-link>
    </div>
     <div class="main">
        <div class="title">
            <h4>
                <nuxt-link to="/sign-in">
                   登录
                
                </nuxt-link>

                <b>.</b>
                 <nuxt-link class="active"  to="/sign-up">
                   注册
                
                </nuxt-link>


            </h4>

        </div>
      <!-- form -->
        <div class="js-form">
              <form method="post">
                <div class="input-prepend">
                  <input type="text"  placeholder="手机号或邮箱">
                  <i class="fa fa-user"></i>
                </div>

                <div  class="input-prepend" >
                  <input type="text" placeholder="密码" >
                  <i class="fa fa-phone"></i>
                </div>
                <div  class="input-prepend ssm">
                  <input type="text" placeholder="手机验证码">
                  <i class="fa fa-shield"></i>
                  <a href="" class="send-ssm">发送验证码</a>
                </div>
                <div class="input-prepend">
                    <input type="text" placeholder="设置密码">
                    <i class="fa fa-lock"></i>

                </div>
                
                  

                  

                  <button class="sign-up-btn">注册</button>
                  <p class="sign-up-msg">
                      点击 “注册” 即表示您同意并愿意遵守简书
                      用户协议 和 隐私政策 。
                  </p>

              </form>

        </div>


          <!-- 第三方登录 -->
        <div class="more-sign">
              <p class="">社交账号注册</p>

              <ul>
                  <li>
                     <nuxt-link to="/">
                      <i class="weixin fa fa-weixin"></i>
                     </nuxt-link>

                  </li>
              
                   <li>
                      <nuxt-link to="/">
                      <i class="qq fa fa-qq"></i>
                     </nuxt-link>
                  </li>

              </ul>

        </div>
 
     
        
    </div>    
  </div>
</template>


<script>
export default {
  // 设置页面的标题以及描述，关键字等原信息
  layout: "sign",
  head: {
    title: "注册-简书",
    meta: [
      { charset: "utf-8" },
      { name: "keywords", content: "注册页面" },
      { name: "description", content: "注册简书" },
      { name: "author", content: "沈龙" }
    ]
  },
  data() {
    return {
      name: "登录"
    };
  }
};
</script>


<style scoped>
/* .sign .js-form .input-prepend:nth-of-type(3){
   margin-bottom: 20px;
} */
</style>
