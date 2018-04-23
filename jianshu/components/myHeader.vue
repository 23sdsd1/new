<template>
  
  <div>
      <nav class="navbar navbar-fixed-top">
         <div class="width-limit">
            <div class="logo">
                <nuxt-link to="/">
                  <img src="~/assets/img/nav-logo.png" alt="">
                </nuxt-link>
                  
            </div>
            <div class="article">
                <a href="" class="btn write-btn">
                  <i class="fa fa-edit">
 
                  </i>
                   写好文章
                </a>
               
            </div>                                    

            <div class="user"  @mouseover="isShow=true" @mouseout="isShow=false">
                <div class="drop-down"  id="avatar"> 
                    <nuxt-link to="/u/123" class="avatar">
                    <img src="~/assets/img/default-avatar.jpg" alt=""></nuxt-link>

                </div>
                   
                <ul class="drop-menu" id="menu" v-show="isShow">
                    <li>
                     <nuxt-link to="/">
                       <i class="fa fa-home">
                          
                       </i>
                        我的主页
                     </nuxt-link>
                    </li>
                   <li>
                     <nuxt-link to="/">
                        <i class="fa fa-heart">
                         
                        </i>
                          喜欢的文章
                     </nuxt-link>
                   </li>
                          <li>
                     <nuxt-link to="/">
                        <i class="fa fa-bookmark">
                        
                        </i>
                           收藏的文章
                     </nuxt-link>
                   </li>
                  <li>
                     <nuxt-link to="/settings/basic">
                         <i class="fa fa-cog">

                         </i>
                         设置
                     </nuxt-link>
                  </li>
                    
                    <li>
                     <nuxt-link to="/sign-out">
                          <i class="fa fa-sign-out">
                 
                          </i>
                       退出
                     </nuxt-link>
                    </li>
                  
                  
                </ul>
            </div>


            <!-- 右上角 -->
            <!-- 导航部分 -->
            <div class="container" >
                   <ul class="nav-list">
                     <li>
                  
                     <div class="navbar-header" id="navbarHeader"  data-mm='1'>
                        <div class="navbar-icon"></div>
                        <div class="navbar-icon"></div>
                        <div class="navbar-icon"></div>
                     </div>
                      
                      <section>
                          <div class="navbarfa">
                            <i class="fa fa-compass" id="c0"></i>
                            <p>发现</p>
                            
                          </div>
                          <div class="navbarfa">
                             <i class="fa fa-book" id="k0"></i>
                             <p>关注</p>
                          </div>
                          <div class="navbarfa" @mouseover="isShow1=true" @mouseout="isShow1=false">
                            <i class="fa fa-bell-o" id="o0" ></i>
                            <p>消息</p>
                            
                             <ul class="drop-menu1"  v-show="isShow1">
                             <li>
                                <nuxt-link to="/">
                                  <i class="fa fa-comment-o"></i>
                                   评论
                                 </nuxt-link>
                              </li>
                              <li>
                                <nuxt-link to="/">
                                  <i class="fa fa-envelope-o"></i>
                                  简讯
                                 </nuxt-link>
                              </li>
                               <li>
                                <nuxt-link to="/">
                                  <i class="fa fa-plus-square-o"></i>
                                  喜欢和赞
                                 </nuxt-link>
                                </li>
                               <li>
                                <nuxt-link to="/">
                                  <i class="fa fa-heart-o"></i>
                                  关注
                                 </nuxt-link>
                                </li>
                               
                           </ul>
                          </div>
                          <div class="navbarfa">
                            <form method="post">
                                      <input type="text" name="" id="" placeholder="搜索" class="search-input">
                                      <a href="#" class="search-b">
                                        <i class="fa fa-search"></i>
                                      </a>
                                  </form>
                          </div>

                      </section>

                    
                     </li>
                      <li>
                           <nuxt-link to="/" class="active">
                                  <i class="fa fa-compass" id="c1"></i>
                                  <span>发现</span>
                           </nuxt-link>
                      </li>
                      <li>
                            <nuxt-link to="/">
                                  <i class="fa fa-book" id="k1"></i>
                                  <span>关注</span>
                           </nuxt-link>

                      </li>
                      <li class="user" @mouseover="notifyShow=true" @mouseout="notifyShow=false" id="o1">
                             <nuxt-link to="">
                                  <i class="fa fa-bell-o" ></i>
                                  <span>消息</span>
                           </nuxt-link>
                           <ul class="drop-menu" v-show="notifyShow" >
                             <li>
                                <nuxt-link to="/">
                                  <i class="fa fa-comment-o"></i>
                                   评论
                                 </nuxt-link>
                              </li>
                              <li>
                                <nuxt-link to="/">
                                  <i class="fa fa-envelope-o"></i>
                                  简讯
                                 </nuxt-link>
                              </li>
                               <li>
                                <nuxt-link to="/">
                                  <i class="fa fa-plus-square-o"></i>
                                  喜欢和赞
                                 </nuxt-link>
                                </li>
                               <li>
                                <nuxt-link to="/">
                                  <i class="fa fa-heart-o"></i>
                                  关注
                                 </nuxt-link>
                                </li>
                               
                           </ul>
                      </li>
                       <li class="search">
                                  <form method="post">
                                      <input type="text" name="" id="" placeholder="搜索" class="search-input">
                                      <a href="#" class="search-btn">
                                        <i class="fa fa-search"></i>
                                      </a>
                                  </form>
                        </li>
                   </ul>
            </div>
         </div>
      </nav>
      
  </div>
</template>


<script>
export default {
  // name:myHeader,
  data: function() {
    return {
      isShow: false,
      notifyShow: false,
      isShow1 :false
    };
  },
  // mounted:function(){
  //     var avatar = document.querySelector('#avatar')
  //     var menu = document.querySelector('#menu')
  //     avatar.onmouseover = function(){
  //         console.log(11111111111111)
  //         menu.style.display = 'block'

  //     }
  //     avatar.onmouseleave = function(){
  //         menu.style.display = 'none'
  //     }
  // }
  mounted: function() {
    var navbarHeader = document.querySelector("#navbarHeader");
    var section = document.querySelector("section");
    var navbarFa = document.querySelector("navbarfa");

    navbarHeader.onclick = function() {
      if (navbarHeader.getAttribute("data-mm") == 1) {
        console.log("333333333333333");
        section.style.height = "400px";
        section.style.transition = "all 0.5s";
        navbarHeader.setAttribute("data-mm", 2);
      } else {
        section.style.height = "0px";
        section.style.transition = "all 0.5s";
        navbarHeader.setAttribute("data-mm", 1);
      }
    };
  }
};
</script>

<style scoped>
nav {
  width: 100%;
  height: 56px;
}
.navbar {
  /* position: relative;
   min-height: 50px; */
  margin-bottom: 20px;
  border-width: 0 0 1px;
  border-color: #f0f0f0;
  background-color: #fff;
}
.navbar-fixed-top {
  position: fixed;
  left: 0;
  top: 0;
  z-index: 9999;
}

.navbar:before {
  content: "";
  display: table;
}
nav .width-limit {
  min-width: 768px;
  max-width: 1440px;
  /* height: 56px; */
  /* background-color: red; */
  margin: 0 auto;
}
nav .logo {
  float: left;
  height: 56px;
}
nav .logo img {
  height: 100%;
}
nav .write-btn {
  float: right;
  width: 100px;
  height: 40px;
  line-height: 40px;
  margin: 8px 15px 0;
  border-radius: 20px;
  font-size: 15px;
  color: #fff;
  background: #ea6f5a;
  text-align: center;
}

nav .write-btn:hover {
  background: #ec6149;
}

nav .user {
  position: relative;
  float: right;
}
nav .user .avatar {
  position: relative;
  display: block;
  width: 40px;
  height: 40px;
  margin: 8px 28px 8px 20px;
}
nav .user .drop-down:hover {
  background: #f5f5f5;
}
nav .user .avatar:before {
  content: "";
  position: absolute;
  border-left: 5px solid transparent;
  border-right: 5px solid transparent;
  border-top: 5px solid #999;
  top: 18px;
  right: -14px;
}
nav .user .avatar img {
  width: 100%;
  height: 100%;
  border-radius: 50px;
  border: 1px solid #eee;
}
nav .user .drop-menu {
  position: absolute;
  /* top:0; */
  box-shadow: 0 0 8px rgba(0, 0, 0, 0.1);
  min-width: 160px;
  z-index: 999;
  margin: 0;
  /* display: none; */
}

nav .user .drop-menu li a {
  padding: 10px 20px;
  display: block;
  line-height: 30px;
}
nav .user .drop-menu li a:hover {
  background: #f5f5f5;
}
nav .user .drop-menu li a i {
  margin-right: 10px;
  color: #ea6f5a;
  font-size: 18px;
  width: 20px;
  height: 20px;
  font-size: 20px;
  display: inline-block;
}
nav .nav-list {
  margin: 0;
}
nav .nav-list:after {
  content: "";
  height: 0;
  display: block;
  visibility: hidden;
  clear: both;
}
nav .nav-list > li {
  float: left;
  margin-right: 5px;
}
nav .nav-list > li a {
  display: block;
  height: 56px;
  line-height: 26px;
  padding: 15px;
}

nav .nav-list > li a.active {
  color: #ea6f5a;
  background: none !important;
}
#only {
  /* color: #ea6f5a; */
}
nav .nav-list > li a:hover {
  background: #f5f5f5;
}
nav .nav-list > li a i {
  margin-right: 5px;
  font-size: 20px;
}
nav .nav-list .search {
  padding-left: 15px;
  margin-left: 10px;
}
nav .nav-list .search form {
  position: relative;
  margin-bottom: 20px;
  top: 9px;
}
nav .nav-list .search form input {
  width: 240px;
  height: 38px;
  font-size: 14px;
  padding: 0 40px 0 20px;
  border: 1px solid #eee;
  background: #eee;
  border-radius: 40px;
  transition: width 0.5s;
}
nav .nav-list .search form .search-input:focus {
  width: 320px;
}
nav .nav-list .search form .search-input:focus ~ .search-btn {
  background: #969696;
  color: #fff;
  border-radius: 50%;
}
nav .nav-list .search form .search-btn {
  position: absolute;
  width: 30px;
  height: 30px;
  top: 4px;
  right: 5px;
  color: #969696;
  text-align: center;
  padding: 0;
}

nav .nav-list .search form .search-btn:hover {
  background: none;
}
nav .nav-list .search form .search-btn i {
  display: block !important;
  margin: 0;
  text-align: center;
  line-height: 30px;
  font-size: 14px;
}
.navbar-header {
  width: 40px;
  height: 35px;
  border: 1px solid lightgray;
  margin-top: 10px;
  /* background-color: red; */
  display: none;
}
.navbar-header .navbar-icon {
  width: 20px;
  height: 2px;
  background: #888888;
  margin-top: 4px;
  margin-left: 10px;
}
.navbar-header .navbar-icon:nth-of-type(1) {
  margin-top: 10px;
}

section > .navbarfa {
  width: 100%;
  height: 15%;
  border-bottom: 1px solid #f0f0f0;
  border-top: 1px solid #f0f0f0;
}
section > .navbarfa > p {
  margin: 0;
  padding-top: 10px;
}
section {
  position: fixed;
  width: 100%;
  height: 0px;
  left: 0;
  text-align: center;
  /* display: none; */
  overflow: hidden;
}

section .navbarfa .search-input {
  position: relative;
  width: 100%;
  height: 38px;
  font-size: 14px;
  padding: 0 40px 0 20px;
  border: 1px solid #eee;
  background: #eee;
  border-radius: 40px;
}
section .navbarfa form .search-b {
  position: absolute;
  width: 30px;
  height: 30px;
  top: 50%;
  right: 2%;
  color: #969696;
  text-align: center;
  padding: 0;
}

section .navbarfa .search form .search-b i {
  display: block !important;
  margin: 0;
  text-align: center;
  line-height: 30px;
  font-size: 12px;
}
section .navbarfa form .search-input:focus ~ .search-b {
  background: #969696;
  color: #fff;
  border-radius: 50%;
}
section .navbarfa .drop-menu1 {
  position: absolute;
  top:140px;
 

  box-shadow: 0 0 8px rgba(0, 0, 0, 0.1);
  min-width: 160px;
  z-index: 999;
  margin: 0;
  
}

section .navbarfa:nth-of-type(1){
  margin-top: 10px;
  color: #ea6f5a;
}
#c0 {
  display: none;
  position: absolute;
  left: 215px;
  top: 22px;
  font-size: 20px;
  
}
#k0 {
  display: none;
  position: absolute;
  left: 215px;
  top: 80px;
  font-size: 20px;
}
#o0 {
  display: none;
  position: absolute;
  left: 215px;
  top: 140px;
  font-size: 20px;
}
section > .navbarfa:nth-of-type(2):hover {
  background: #f5f5f5;
}
section > .navbarfa:nth-of-type(3):hover {
  background: #f5f5f5;
}
@media (max-width:2000px){
  section{
    display: none;
  }
}
@media (max-width: 1440px) {
  nav .nav-list > li a i {
    display: none;
  }
  nav .nav-list .search form .search-input {
    width: 160px;
  }
  nav .nav-list .search form .search-input:focus {
    width: 200px;
  }
  section{
    display: none;
  }
}

@media (max-width: 1080px) {
  nav .nav-list li span {
    display: none;
  }
  nav .nav-list > li a i {
    display: block;
  }
    section{
    display: none;
  }
}

@media (max-width: 768px) {
  nav .nav-list li span {
    display: none;
  }
  /* nav .nav-list > li a i {
    display: none;
  } */
  #c1 {
    display: none;
  }
  .navbar-header {
    display: block;
  }
  #o1 {
    display: none;
  }
  #k1 {
    display: none;
  }
  nav .nav-list .search form {
    display: none;
  }
  section .navbarfa .drop-menu1 {
    display: none;
  }
  section{
    display: block;
  }
}
@media (max-width: 320px) {
  section{
    display: block;
  }
  section .navbarfa>p{
    float: left;
    margin-left: 30px;
  }
  #c0{
    display: block;
    left: 10px;
  }
  #k0{
    display: block;
    left: 10px;
  }
  #o0{
    display: block;
    left: 10px;
  }
   section .navbarfa .drop-menu1 {
    display: block;
  }
}
</style>

