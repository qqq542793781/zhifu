<template>
  <div class="left-div">
     <ul>
         <li v-for="gr in xxlist">
             <span><img :src="gr.touxiang" width="222" height="190" class="touxiang"/></span>
             <span class="name">{{gr.name}}</span><br/><br/>
             <span class="fontstyle"><i class="icon iconfont icon-geren11"></i>{{gr.chusheng}}</span><br/>
             <span class="fontstyle"><i class="icon iconfont icon-dizhi"></i>{{gr.dizhi}}</span><br/>
             <span class="fontstyle"><i class="icon iconfont icon-dianhuaphone349"></i>{{gr.lianxi}}</span><br/>
             <span class="fontstyle"><i class="icon iconfont icon-youxiang"></i>{{gr.youxiang}}</span>
         </li>
     </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      xxlist: [
        {
          name:'匡凯',
          touxiang:
            "https://ss1.bdstatic.com/70cFuXSh_Q1YnxGkpoWK1HF6hhy/it/u=2088161779,514597462&fm=27&gp=0.jpg",
          chusheng: " 1997/9/15",
          dizhi: " 湖南省常德市",
          lianxi: " 18773659851",
          youxiang: " 542793781@qq.com"
        }
      ],
    };
  }
};
</script>

<style scoped>
.left-div {
  width: 300px;
  height: 800px;
  background-color: #79c2f0;
  margin-left: auto;
  margin-right: auto;
  margin-top: 75px;
  border-radius: 15px 0 0 15px;
}
.left-div ul li {
  list-style: none;
  color: #f5f5f5;
  font-size: 17px;
}
.touxiang {
  border-radius: 50%;
  border: 3px solid #9d9d9d;
}
.fontstyle {
  padding-left: 35px;
}
.name{
    font-size: 30px;
    text-align: center;
    margin-left: 85px;
}
</style>
