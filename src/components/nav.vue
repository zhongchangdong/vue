<template>
  <div class="nav w clear">
      <ul class="nav">
            <router-link to="/hader" tag="li" active-class="active" >
                <a href="javascript:;">首页</a>
            </router-link>
            <router-link to="/follow" tag="li" active-class="active">
                <a href="javascript:;">关注</a>
            </router-link> <router-link to="/index" tag="li" active-class="active">
                <a href="javascript:;">房屋设计</a>
            </router-link> </router-link> <router-link to="/contact" tag="li" active-class="active">
                <a href="javascript:;">联系我们</a>
            </router-link>

        </ul>
</div>
</template>
<script>
</script>

<style>
    /* 导航 */
.nav {
  height: 50px;
  line-height: 50px;
  padding-left: 200px;


}
.nav  li {
  width:100px;
  height: 50px;
  float: left;
  margin-left:80px;
  font-size:20px;
  font-weight:900;

}
.nav li a:hover {
  display: block;
  color:green;
}

</style>