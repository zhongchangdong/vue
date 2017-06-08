<template>
    <div>

          <div :class="{rgb:a}">

              <div class="stool w">
                  <img src="../assets/images/1.png" alt="">
                  <div class="stool_right">
                      <h1>{{datum}}</h1>
                      <p>{{datum1}}</p>
                  </div>
              </div>
          </div>
  <div class="close w" >
       <a href=""><img src="../assets/images/b1.png" alt=""></a>
        <a href=""><img src="../assets/images/13.jpg" alt=""></a>
        <a href=""><img src="../assets/images/r-2.jpg" alt=""></a>
    </div>
    </div>
</template>

<script >
     export default {
        data(){
            return{
                    a:true,
                    datum:'欢迎您来到家具设计中心',
                    datum1:'我们不相信会有完美无缺的家，但是我们相信家能够完美彰显房子主人的风格特点。在家里，一切风格和功能有了这些创意和灵感，就可以打造出一方你喜欢称其为家的空间。',
            }
        }
     }
</script>

<style>
.rgb{
background:#333333;
height:320px;

 }

.stool  img {
padding-top:20px;
width:282px;
height:280px;
border-radius:50%;
float: left;

}
.stool_right {
    padding-top: 75px;
    width:538px;
    float: left;
    margin-left: 80px;

}
.stool_right h1 {
     color:#FAFAFA;

}
.stool_right p {
margin-top:10px;
color:#FAFAFA;
line-height: 25px;
}
</style>

