<template>
  <div id="sign-template">
    <nuxt/>

          


  </div>
</template>

<script>
// import Vue from 'vue'
// import BootstrapVue from 'bootstrap-vue'
// Vue.use(BootstrapVue)
// // 首先引入bootstrap.css文件，加载bootstrap样式
// import 'bootstrap/dist/css/bootstrap.css'

// // 引入bootstrap-vue.css文件
// import 'bootstrap-vue/dist/bootstrap-vue.css'

export default {};
</script>

<style>
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
</style>
