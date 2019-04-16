<template lang="pug">
  .login-box
    .login-bg-box
      .login-main-box
        .login-logo-box
          img(:src="require('@/assets/img/login/logo.png')")
        .hot-line-label 咨询热线：0318-8855666
        .login-bottom-right-bg-box
        .login-item-box
          label 手机号码：
          input(placeholder="11位数字" type="text")
        .login-item-box
          label 密码：
          input(placeholder="不少于六位" type="password")
        .login-item-box
          label 验证码：
          input(placeholder="六位数字" type="text")
        .login-item-box
          label 类型：
          input(type="radio")
          label 学员
          input(type="radio")
          label 教师
</template>

<script>
export default {
  name: 'Login',
  data () {
    return {

    }
  }
}
</script>

<style lang="scss" scoped>
  .login-box{
    width: 100%;
    height: 100%;
    position: relative;
    background: url("../../assets/img/login/bg.png");
    .login-bg-box{
      position: absolute;
      left: 50%;
      top: 50%;
      margin-left: -445px;
      margin-top: -260px;
      width: 890px;
      height: 520px;
      background: #FFFDF9;
      border: 1px solid #D3D3D3;
      border-radius: 4px;
      .login-main-box{
        width: 100%;
        height: 100%;
        position: relative;
        .login-bottom-right-bg-box{
          position: absolute;
          bottom: 0;
          right: 0;
          width: 324px;
          height: 214px;
          background: url("../../assets/img/login/login-bg.png") no-repeat;
          background-position: bottom right;
        }
        .login-logo-box{
          position: absolute;
          top: 20px;
          left: 20px;
          width: 191px;
          height: 74px;
          img{
            width: 100%;
            height: 100%;
          }
        }
        .hot-line-label{
          position: absolute;
          right: 20px;
          top: 20px;
          font-family: PingFangTC-Regular;
          font-size: 18px;
          color: #232323;
        }
      }
    }
  }
</style>
