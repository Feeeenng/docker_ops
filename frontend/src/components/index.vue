<template>
  <div>
    <div>
  <el-menu theme="light" :default-active="activeIndex" class="el-menu-demo" mode="horizontal" @select="handleSelect" default-active="2">
  <el-menu-item index="index" class="index-title-t1"><i class="el-icon-share"></i>Docker_ops</el-menu-item>
  <el-menu-item index="2" class="index-title-t2"><i class="el-icon-menu"></i>容器管理</el-menu-item>
  <el-menu-item index="3"><i class="iconfont icon-jingxiangcangku"></i>镜像管理</el-menu-item>
  <el-menu-item index="4"><i class="iconfont icon-warehouse"></i>仓库管理</el-menu-item>
  <el-menu-item index="5"><i class="iconfont icon-zhanghao"></i>账号管理</el-menu-item>
  <el-menu-item index="6"><i class="iconfont icon-rizhi"></i>日志记录</el-menu-item>
  <el-menu-item index="7" class="index-user"><i class="iconfont icon-yonghu"></i>Admin</el-menu-item>
</el-menu>
    </div>
    <div class="block" style="float: left;margin-left: 30px">
      <span class="wrapper">
        <el-button  type="primary" style="margin-top: 10px">
          <i class="iconfont el-icon-time" style="margin-right: 5px;float: left"></i>
          <p style="float: left">刷新</p>
        </el-button>
        <el-button type="success" >
          <i class="iconfont el-icon-plus" style="margin-right: 5px;float: left"></i>
          <p style="float: left">创建容器</p>
        </el-button>

      </span>
    </div>
</div>
</template>

<script>
  export default {
    data() {
      return {
        activeIndex: '1',
      };
    },
    methods: {
      handleSelect(key, keyPath) {
        console.log(key, keyPath);
      }
    }
  }
</script>

<style>
.index-title-t1{
  font-family:"Helvetica Neue" !important;
  /*border-right: 0.5px solid white;*/
}
.index-title-t2{
   font-size: inherit;
  font-style:normal;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
.icon-jingxiangcangku,.icon-warehouse,.icon-zhanghao,.icon-rizhi{
    font-size: 23px;
    margin-right: 10px;
}
.icon-yonghu{
  font-size: 23px;
  margin-left: 20px;
}
.el-menu-demo .index-user .icon-yonghu{
  margin-left: 10px;
  margin-right: 30px;
}
.el-menu-demo .index-user{
    float: right ;
    margin-right: 30px ;
  }
.block{

}


</style>
