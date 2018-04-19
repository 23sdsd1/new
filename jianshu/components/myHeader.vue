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
                   写文章
                </a>
               
            </div>

            <div class="user">
                <div class="drop-down">
                    <nuxt-link to="/u/123" class="avatar">
                    <img src="~/assets/img/default-avatar.jpg" alt=""></nuxt-link>

                </div>
                   
                <ul>
                    <li>
                     <nuxt-link to="/">
                       <i class="fa fa-home">
                           我的主页
                       </i>
                     </nuxt-link>
                    </li>
                   <li>
                     <nuxt-link to="/">
                        <i class="fa fa-heart">
                           喜欢的文章
                        </i>
                     </nuxt-link>
                   </li>
                          <li>
                     <nuxt-link to="/">
                        <i class="fa fa-bookmark">
                           收藏
                        </i>
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
         </div>
      </nav>
      
  </div>
</template>


<script>

    export default {

    }

</script>

<style>

</style>

