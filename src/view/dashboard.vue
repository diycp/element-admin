<template>
  <el-row class="layout">
    <el-col :span="3" class="sider">
      <el-col :span="24" class="banner">
        <div class="banner">
        <img class="logo" src="static/image/logo.png">
        <span class="title">Vue Admin</span>
        </div>
      </el-col>
      <el-col :span="24" class="menu">
        <el-menu theme="dark">
          <el-menu-item index="2"><i class="el-icon-menu"></i>欢迎使用</el-menu-item>
          <el-menu-item index="2"><i class="el-icon-menu"></i>新手指南</el-menu-item>
          <el-submenu index="1">
            <template slot="title"><i class="el-icon-message"></i>基础组件</template>
            <el-menu-item-group>
              <template slot="title">Basic</template>
              <el-menu-item index="1-1">选项1</el-menu-item>
              <el-menu-item index="1-2">选项2</el-menu-item>
            </el-menu-item-group>
            <el-submenu index="1-4">
              <template slot="title">Form</template>
              <el-menu-item index="1-4-1">选项1</el-menu-item>
            </el-submenu>
            <el-submenu index="1-4">
              <template slot="title">Data</template>
              <el-menu-item index="1-4-1">选项1</el-menu-item>
            </el-submenu>
            <el-submenu index="1-4">
              <template slot="title">Notice</template>
              <el-menu-item index="1-4-1">选项1</el-menu-item>
            </el-submenu>
            <el-submenu index="1-4">
              <template slot="title">Navigation</template>
              <el-menu-item index="1-4-1">选项1</el-menu-item>
            </el-submenu>
            <el-submenu index="1-4">
              <template slot="title">Others</template>
              <el-menu-item index="1-4-1">选项1</el-menu-item>
            </el-submenu>
          </el-submenu>
          <el-menu-item index="3"><i class="el-icon-setting"></i>数据报表</el-menu-item>
          <el-menu-item index="3"><i class="el-icon-setting"></i>动画效果</el-menu-item>
          <el-menu-item index="3"><i class="el-icon-setting"></i>字体图标</el-menu-item>
          <el-menu-item index="3"><i class="el-icon-setting"></i>富文本编辑</el-menu-item>
          <el-menu-item index="2"><i class="el-icon-menu"></i>数据可视化</el-menu-item>
          <el-menu-item index="3"><i class="el-icon-setting"></i>主题设置</el-menu-item>
        </el-menu>
      </el-col>
    </el-col>

    <el-col :span="21" class="main">
      <el-col :span="24" class="header">
        <el-col :span="4" class="toggle">
        </el-col>
        <el-col :span="16" class="action">
        </el-col>
        <el-col :span="4" class="profile">
        </el-col>
      </el-col>
      <el-col :span="24" class="content"></el-col>
      <el-col :span="24" class="footer"></el-col>
    </el-col>
  </el-row>
</template>

<style>
  .layout, .sider, .main, .toggle, .action, .profile {
    background-color: #f8f8f8;
    height: 100%;
  }

  .sider {
    background-color: #1f2d3d;
    color: #999;
  }

  .main {
    /*background-color: #1c8de0;*/
  }

  .header, .banner {
    background-color: #fff;
    text-align: center;
    line-height: 80px;
    height: 80px;
  }

  .banner {
    cursor: pointer;
    color: #666;
  }

  .logo {
    vertical-align: middle;
    margin-right: 8px;
    width: 40px;
  }

  .title {
    vertical-align: text-bottom;
    text-transform: uppercase;
    display: inline-block;
    font-size: 16px;
  }

  .toggle {
    background-color: #11b95c;
  }

  .action {
    background-color: #ff4d51;
  }

  .profile {
    background-color: sienna;
  }

  .content {
    background-color: #1c8de0;
  }

  .footer {
    background-color: #1f2d3d;
    /*height: 64px;*/
  }

</style>

<script>
  import ElRow from 'element-ui/packages/row/src/row'
  import ElCol from 'element-ui/packages/col/src/col'
  export default {
    components: {
      ElCol,
      ElRow
    },
    data () {
      return {
        form: {
          name: '',
          region: '',
          date1: '',
          date2: '',
          delivery: false,
          type: [],
          resource: '',
          desc: ''
        }
      }
    },
    methods: {
      onSubmit () {
        console.log('submit!')
      }
    }
  }
</script>
