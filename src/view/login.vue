<template>
  <el-row>
    <el-col>
      <el-form ref="form" model="form" labelWidth="0">
        <div class="login-form-tab">
          <img class="login-form-logo" src="static/image/logo.png">
          <span class="login-form-title">Vue Admin</span>
        </div>
        <el-form-item>
          <el-input v-model="form.name" placeholder="用户名">
            <template slot="prepend">
              <i class="fa fa-user" aria-hidden="true"></i>
            </template>
          </el-input>
        </el-form-item>
        <el-form-item>
          <el-input v-model="form.password" placeholder="密   码">
            <template slot="prepend">
              <i class="fa fa-lock" aria-hidden="true"></i>
            </template>
          </el-input>
        </el-form-item>
        <el-form-item>
          <el-button type="primary" autofocus="true">登录</el-button>
        </el-form-item>
        <p class="login-form-tips">
          <span>用户名：admin</span>&nbsp;&nbsp;
          <span>密  码：admin</span>
        </p>
      </el-form>
    </el-col>
  </el-row>
</template>

<style>
  .el-row, .el-col {
    height: 100%;
  }

  .el-form {
    box-shadow: 0 0 100px rgba(0, 0, 0, .08);
    margin: -160px 0 0 -160px;
    border-radius: 4px;
    position: absolute;
    text-align: center;
    width: 256px;
    height: 256px;
    padding: 32px;
    top: 50%;
    left: 50%;
  }

  .login-form-tab {
    margin-bottom: 24px;
    line-height: 40px;
    cursor: pointer;
    height: 40px;
    color: #666;
  }

  .login-form-logo {
    margin-right: 8px;
    width: 40px;
  }

  .login-form-title {
    vertical-align: text-bottom;
    text-transform: uppercase;
    display: inline-block;
    font-size: 16px;
  }

  .login-form-tips {
    text-align: center;
    margin-top: 16px;
    font-size: 12px;
    color: #CCC;
  }

  .el-button {
    width: 100%;
  }

  .fa {
    width: 24px;
    text-align: center;
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
