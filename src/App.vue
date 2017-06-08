<template>
  <div>

      <div class="j_hader">
          <div class=" w ">
          <div >
              <img src="./assets/images/logo1.png"alt="">
          </div>
          <div class="fr clear">
          <a href="">
             <strong>联系我们:<i>(800)</i></strong>
            <p>138000</p>
          </a>

          </div>
          </div>
      </div>
       <Vav></Vav>
        <router-view></router-view>

     <!-- 轮播图 -->
      <div  class=" slideshow clear">
          <Regards></Regards>

      </div>
    <div class="foot clear">
    <div class="w ">
        <div class="buttom" v-for="alue in foot">
        <h3>{{alue.name}}</h3>
        <ul>
        <li v-for="item in alue.list">
          <a href="#">{{item.titlt}}</a>
        </li>
        </ul>
        </div>
        <input type="text" name="" value="" Placeholder="请输入您的信息">
        <p class="bs">Copyright © 2016.公司所有的注册名称和服务</p>
    </div>
</div>

  </div>
</template>
<script>


import  Regards  from './components/regards.vue'
import  Vav  from './components/nav.vue'
  export default {
  components:{
      Regards,
      Vav
},
      data() {
         return {
          foot: {
            bbs: {
              name:'产品',
              list:[
              {
              titlt:'主页',
              url:"xxxxxx"
             }, {
              titlt:'普通住在',
              url:"xxxxxx"
             }, {
              titlt:'主页',
              url:"xxxxxx"
             }, {
              titlt:'商品',
              url:"xxxxxx"
             }, {
              titlt:'主页',
              url:"xxxxxx"
             }, {
              titlt:'主页',
              url:"xxxxxx"
             },

              ]
            },
           bbs2: {
              name:'关于我们',
              list:[
              {
              titlt:'主页',
              url:"xxxxxx"
             }, {
              titlt:'主页',
              url:"xxxxxx"
             }, {
              titlt:'主页',
              url:"xxxxxx"
             }, {
              titlt:'主豪华装修',
              url:"xxxxxx"
             }, {
              titlt:'主页',
              url:"xxxxxx"
             }, {
              titlt:'主页',
              url:"xxxxxx"
             },

              ]
            },
             bbs3: {
              name:'播客',
              list:[
              {
              titlt:'普通住宅',
              url:"xxxxxx"
             }, {
              titlt:'大方',
              url:"xxxxxx"
             }, {
              titlt:'主页',
              url:"xxxxxx"
             }, {
              titlt:'设计',
              url:"xxxxxx"
             }, {
              titlt:'主页',
              url:"xxxxxx"
             }, {
              titlt:'主页',
              url:"xxxxxx"
             },

              ]
            },
             bbs4: {
              name:'产品',
              list:[
              {
              titlt:'主页',
              url:"xxxxxx"
             }, {
              titlt:'主页',
              url:"xxxxxx"
             }

              ]
            },

          }
         }
      }
  }
</script>


<style>
  body{
    background:url('./assets/images/bg.png');
  }
  *{
    margin: 0;
    padding: 0;
  }
  ul, li {
   list-style: none;
 }
 .clear{
  clear:both;
}

  .fl {
    float: left;

}
   .fr {
    float: right;

}
 a {
    text-decoration: none;
    color:#000000;
}
  .w {
    width:1200px;
    margin: 0 auto;
}

/* 头部 */
  .j_hader {
    height: 60px;
    background:#000000;
    position: relative;
    line-height: 60px;
}

.j_hader img {
    width:120px;
    height: 130px;
    position: absolute;
    top: 0;
    left:225px;
    z-index:9999;

}
.j_hader .fr {
  width:250px;
  height:60px;
  line-height: 60px;


}
.fr strong {
    color:#FFFFFF;
    float: left;
    font-size:20px;
}
.fr p {
  float: left;
  color:#FFFFFF;
  margin-left:10px;
  font-size:20px;

}
.fr i {
  color:green;
}
/* 底部 */
.foot {
  height: 400px;
  padding-top:20px;
  background:#4C4C4C;
  position: relative;

}

.buttom  {
    width:300px;
    height: 300px;
    float: left;
    text-align: center;
    position: relative;
}
.buttom  h3 {
    color:#FFFFFF;
    font-size:30px;
}
.buttom  li  {
     color:#777777;
     margin-top:10px;
}
.buttom  a {
color:#777777;
}
.bs{
  text-align: center;

}

input {
  position: absolute;
  top: 120px;
  right:120px;
  width:200px;
  height: 38px;
  background:#333333;
  color:#FFFFFF;
  font-size:16px;
  padding-left: 5px;

}
</style>

