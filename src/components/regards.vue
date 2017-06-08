<template>
    <div>
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
                     productList: {

                    app: {
                      title: '01/家居',

                  list: [
                    {
                      name: '01/家居',
                      url: './static/images/ww1.jpg',
                      yuedu:'阅读更多'

                    },

                  ]
                    },
                    app1: {
                    title: '01/家居',

                  list: [
                    {
                    url: './static/images/ww1.jpg',
                    yuedu:'阅读更多'


                    },
                      ]
                     },
                     app2: {
                      title: '01/家居',
                  list: [
                    {
                    name: '家居',
                    url: './static/images/ww1.jpg',
                        yuedu:'阅读更多'
                    },
                  ]
                    },

                    app3: {
                      title: '01/家居',
                  list: [
                    {
                    name: '91助手',
                    url: './static/images/ww1.jpg',
                     yuedu:'阅读更多'

                    },
                  ]
                },

             }
         }
      }
}

</script>

<style>
.exhibition {

height:785px;
    }
.exhibition h1 {
text-align: center;
color:#8B4513;
line-height:100px;
}
.exhibition  p {
    text-align: center;

}
.list li{
min-width:220px;
float: left;
margin-left:35px;
margin-top:20px;

}
.ckg{
position: relative;
}

.ckg p {
padding-top:200px;
position: absolute;
top: 0;
left: 0;
color:#F5FAFA;
font-size:24px;
padding-left:52px;
line-height: 35px;
}

.serve p {
margin-top:50px;
text-align: center;
color:#8B455C;
font-weight:700;
font-size:40px;

}
.serve  div {
 padding-top:50px;
 float: left;


}
.serve  div img {
 width:250px;

}

.serve h1 {
color:#8B455C;
}
.serve  div span{
display: block;
color:#000000;
line-height: 30px;

}
.serve div h3{
    margin-top:10px;
    margin-bottom: 50px;
}
.serve div  a {
color:#8B455C;
border-top:4px solid #8B455C;

}

</style>