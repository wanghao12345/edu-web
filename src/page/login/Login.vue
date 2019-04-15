<template lang="pug">
  .login-box
    .login-bg-box
      .login-main-box
        .login-logo-box
          img(:src="require('@/assets/img/login/logo.png')")
        .login-bottom-right-bg-box
</template>

<script>
export default {
  name: 'Login'
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
      }
    }
  }
</style>
