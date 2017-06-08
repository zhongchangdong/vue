<template>
  <div>
    <div class="close w" >
       <a href=""><img src="../assets/images/w2.jpg" alt=""></a>
        <a href=""><img src="../assets/images/team-2.jpg" alt=""></a>
        <a href=""><img src="../assets/images/w1.jpg" alt=""></a>
    </div>

            <div class="w clear ">
                <div class="exhibition">
                    <h1>{{ reqards }}</h1>
                     <p>{{ reqards1 }}</p>
                       <p>{{ reqards2 }}</p>
                         <h1>{{ reqards3 }}</h1>
                         <div class="list">
                          <ul>
                            <li v-for="list in msg">
                            <img :src="list.sort" alt="">
                         </li>
                    </ul>
                </div>
            </div>
         </div>
<div class="ckg clear">
        <img src="../assets/images/quote.jpg" alt="">
        <p>银器需要抛光的家具可以用一个好的除尘现今
             <br>
               我们越来越重视环保的生活方式。我们不像以
            <br>
                前一样经常买，买，买，而是最大化利用家中的
            <br>
                现有物品。</p>
            <span></span>
        </div>

<div class="serve w clear">
    <p>技术服务</p>
    <div  v-for="togo in productList">
        <h1 >{{togo.title}}</h1>
       <ul >
        <li  v-for="bbs in togo.list">
            <img :src="bbs.url" alt="">
            <span>基本上没有人喜欢手忙脚乱的清晨时光。
        <br>
            尤其是你还在和父母共用一间
             <br>
            浴室时。
            还有家里的兄弟姐妹。'</span>
            <h3><a href="">{{bbs.yuedu}}</a></h3>
        </li>
         </ul>
    </div>

</div>
    </div>
</template>

<script>
      export default {
            data () {
                return {
                    reqards: '关于',
                    reqards1:"我们不相信会有完美无缺的家，但是我们相信家能够完美彰显房子主人的风格特点。有了这些创意和灵感，就可以打造出一方你",
                    reqards2 :'喜欢称其为家的空间',
                    reqards3:'最新设计',
                    msg:[
                    {
                        sort:'./static/images/blog-1.jpg',
                    }
                    ,{
                         sort:'./static/images/blog-1.jpg',
                    },{
                         sort:'./static/images/blog-1.jpg',
                    },{
                         sort:'./static/images/blog-1.jpg',
                    },{
                         sort:'./static/images/blog-1.jpg',
                    },{
                         sort:'./static/images/blog-1.jpg',
                    }
                    ,{
                          abc:'./static/images/blog-1.jpg'
                    }
                    ],


         }
      }
}

</script>

<style>


.close img {
  width:300px;
  height:300px;
 margin-left:80px;

}
</style>