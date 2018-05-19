<template>
  <div class="info">
    <el-row>
      <el-col :span='7' class="left">
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
         <div class="jineng">
           <span class="jineng-title">技能掌握</span>
           <ul>
           <li><span>photoshop</span>:<span>良好</span></li>
           <li><span>AngularJS</span>:<span>熟悉</span></li>
           <li><span>VueJS:</span> <span>熟练</span></li>
           <li><span>javascript:</span><span>熟悉</span></li>
           <li><span>html/css:</span><span>熟悉</span></li>
           <li><span>react:</span><span>了解</span></li>
           <li><span>jQuery:</span><span>良好</span></li>
           <li><span>bootstrap:</span><span>良好</span></li>
           <li><span>C#:</span><span>熟悉</span></li>
           <li><span>ajax:</span><span>良好</span></li>
           <li><span>axios:</span><span>良好</span></li>
         </ul>
         <span class="beizhu">会使用gulp以及webpack<br>进行前端项目的打包</span>
         </div>
        </div>
      </el-col>
      <el-col :span='17' class="right">
        <el-tabs>
          <el-tab-pane label="求职意向">
            <ul>
              <li v-for="yx in yixiang">
                <span>行业：{{yx.hangye}}</span>
                <span class="font-jiange1">地点：{{yx.didian}}</span><br/>
                <span>职业：{{yx.zhiye}}</span>
                <span class="font-jiange2">期望薪资：{{yx.xinzi}}</span><br/>
                <span>到职时间：{{yx.daogang}}</span>
                <span class="font-jiange3">类型：{{yx.leixing}}</span>
              </li>
            </ul>
          </el-tab-pane>
          <el-tab-pane label="教育背景">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;毕业于湖南文理学院计算机专业/本科。</el-tab-pane>
          <el-tab-pane label="工作经验">
            &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
            应届毕业生，暂无相关专业工作经验。<br>
            &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;其他工作经历：
            <span class="time2">2015/9-2016/2</span><span>服务员</span><span>(兼职)(餐饮部)</span>
            <div class="gongzuo">
              <span>工作描述：</span><span>主要负责上菜和清洁大堂卫生</span><br>
              <span class="time2">2016/4-2018/1</span><span>在一家小型影楼担任摄影师和修片人员</span><br>
              <span>工作描述：</span><span>主要客户婚礼现场的拍摄立即婚纱照的后期修图(兼职)</span>
            </div>
            </el-tab-pane>
          <el-tab-pane label="自我评价">
            <span>
            &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;好学、好钻研、有良好的自学能力。为人热心，良好的心理素质。能快速融入新环境，
            但不喜欢频繁的更换环境。思维活跃，在压力和困难面前有良好的分析能合解决问题的能力，也是一个富有团队精神的人，有良好的前端开发能力，
            能够相互协作和充分的沟通具有开发能力，故而来贵公司谋求网页前端开发职位
            </span>
          </el-tab-pane>
        </el-tabs>
      </el-col>
      <el-col :span='17' class="dibu">
      <div class="info1">
        <div class="info1-title">
          <span class="aihao">兴趣爱好</span>
        </div>
        <div class="info1-info">
          <ul>
            <li><i class="icon iconfont icon-icon10"></i></li>
            <li><i class="icon iconfont icon-huihuaban"></i></li>
            <li><i class="icon iconfont icon-PingPong"></i></li>
            <li><i class="icon iconfont icon-yinyue"></i></li>
          </ul>
        </div>
      </div>
      <div class="info2">
        <div class="info2-title">
            <span class="jingyan">项目经验</span>   
        </div>
        <div class="info2-biaoti">
            <span class="time1">2017/10/20-2018/2/20</span><span class="tiaoti">学生信息管理系统的设计与实现</span>
        </div>
        <div class="info2-info">
            <span class="info2-info-miaoshu">
              &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;在该项目中所使用的技术有：数据库使用Sql server 2008, 后端使用 Visual Studio 2012的MCV框架,
              前端使用AngularJS。该项目是现在流行的前后端分离的项目。实现了信息的添加、修改、查询（包含模糊查询）、删除。该系统分普通用户以及管理员用户。
              管理员用户权限最大，可以删除、添加普通用户的信息，也可以操作其他信息，而普通用户的权限要小很多。只能进行查询，以及部分信息的添加修改。
            </span>
            <br>
            <br>
            <span>责任描述:&nbsp;&nbsp;主要负责数据库的设计与前端页面的搭建和逻辑和响应式效果以及后端部分业务逻辑的书写</span>
            <br>
            <br>
            <span>采用的技术有：javascript、angularJS、jqeury、css、asp.net以及SQL server。</span>
        </div>
      </div>
      </el-col>
    </el-row>
  </div>
</template>

<script>
export default {
  name: "index",
  data() {
    return {
      yixiang: [
        {
          hangye: "计算机软件",
          didian: "深圳",
          zhiye: "web前端开发",
          xinzi: "4000~5000",
          daogang: "随时",
          leixing: "全职"
        }
      ],

      xiangxi: [
        {
          hunyin: "未婚",
          shengao: "172",
          nianling: "21",
          xingbie: "男"
        }
      ],
      xingqu: [
        {
          xingqu1: "篮球",
          xingqu2: "乒乓球",
          xingqu3: "音乐",
          xingqu4: "绘画"
        }
      ],
      xxlist: [
        {
          name: "匡凯",
          touxiang:
            "https://ss1.bdstatic.com/70cFuXSh_Q1YnxGkpoWK1HF6hhy/it/u=2088161779,514597462&fm=27&gp=0.jpg",
          chusheng: " 1997/9/15",
          dizhi: " 湖南省常德市",
          lianxi: " 18773659851",
          youxiang: " 542793781@qq.com"
        }
      ],
      jnlist: [
        {
          photoshop: "良好",
          angular: "熟悉",
          vue: "熟练",
          cxiapu: "熟悉"
        }
      ],
      shuzu:[
        1,2,3,4,5,6,7,8
      ]
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.time2 {
  font-size: 15px;
  color: #aaa;
}
.beizhu {
  color: #fff;
  padding: 20px;
}
.gongzuo {
  margin-left: 45px;
}
.jineng {
  text-align: center;
  padding-top: 10px;
}
.jineng-title {
  font-size: 25px;
  color: #fff;
}
.jineng ul li {
  margin-left: -40px;
}
.info1-info ul li {
  list-style: none;
  width: 100px;
  height: 95px;
  float: left;
  margin: 0 0 0 45px;
}
.info1-info ul li i {
  font-size: 40px;
}
.ceshi {
  width: 50px;
  height: 40px;
  background-color: #58a3e9;
}
.aihao {
  font-size: 23px;
  color: #58a3e9;
  padding-left: 20px;
}
.time1 {
  padding: 10px;
  font-size: 13px;
  color: #aaa;
}
.tiaoti {
  padding: 10px;
  font-weight: 600;
}
.info1 {
  width: 100%;
  height: 30%;
}
.info2 {
  width: 100%;
  height: 70%;
}
.info {
  height: 800px;
  margin-top: 75px;
  width: 1000px;
  margin-left: auto;
  margin-right: auto;
}
.info2-info {
  padding: 20px;
}

.info2 {
  padding: 10px;
}

.right {
  background-color: #eee;
  height: 300px;
  border-radius: 0 15px 0 0;
  font-size: 20px;
  padding: 10px;
}
.left {
  background-color: #58a3e9;
  height: 800px;
  border-radius: 15px 0 0 15px;
}
.right ul li {
  list-style: none;
}
.font-jiange1 {
  margin-left: 100px;
}
.font-jiange2 {
  margin-left: 80px;
}
.font-jiange3 {
  margin-left: 120px;
}
.left-div {
  width: 300px;
  height: 800px;
  margin-left: auto;
  margin-right: auto;
  margin-top: 35px;
  border-radius: 15px 0 0 15px;
}
.jingyan {
  font-size: 23px;
  color: #58a3e9;
  padding-left: 10px;
}
.dibu {
  height: 500px;
  background-color: #eee;
  border-radius: 0 0 15px 0;
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
.name {
  font-size: 30px;
  text-align: center;
  margin-left: 85px;
}
</style>
