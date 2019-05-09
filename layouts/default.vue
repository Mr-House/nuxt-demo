<template>
  <div>
    <a-back-top />
    <a-layout id="layout-top-side" style="margin: 0 50px">
      <a-layout-header
        class="header"
        :style="{ background: '#fff', height: '433px', padding: '0' }"
      >
        <div class="logo">
          <img src="../static/image/logo.jpg" />
        </div>
        <a-menu
          mode="horizontal"
          :default-selected-keys="['1']"
          :style="{
            backgroundColor: 'rgb(28, 97, 162)',
            color: '#fff'
          }"
        >
          <a-menu-item key="1">首页</a-menu-item>
          <a-menu-item key="2">平台简介</a-menu-item>
          <a-menu-item key="3">采购公告</a-menu-item>
          <a-menu-item key="4">中标公告</a-menu-item>
          <a-menu-item key="5">服务指南</a-menu-item>
          <a-menu-item key="6">新闻动态</a-menu-item>
        </a-menu>
        <a-carousel arrows :autoplay="true">
          <div
            slot="prevArrow"
            class="custom-slick-arrow"
            style="left: 10px;zIndex: 1"
          >
            <a-icon type="left-circle" />
          </div>
          <div slot="nextArrow" class="custom-slick-arrow" style="right: 10px">
            <a-icon type="right-circle" />
          </div>
          <div>
            <img src="../static/image/banner1.jpg" width="100%" />
          </div>
          <div>
            <img src="../static/image/banner2.jpg" width="100%" />
          </div>
          <div>
            <img src="../static/image/banner3.jpg" width="100%" />
          </div>
          <div>
            <img src="../static/image/banner4.jpg" width="100%" />
          </div>
        </a-carousel>
      </a-layout-header>
      <a-layout>
        <a-layout-sider width="250" style="background:#fff">
          <div
            :style="{
              padding: '10px',
              background: 'rgb(28, 97, 162)',
              color: '#fff'
            }"
          >
            <span>按采购组织查看项目</span>
          </div>
          <a-menu
            mode="inline"
            :default-selected-keys="['1']"
            :style="{ height: '100%', borderRight: 0 }"
          >
            <a-menu-item key="1">久泰集团有限公司</a-menu-item>
            <a-menu-item key="2">久泰能源科技有限公司</a-menu-item>
            <a-menu-item key="3">久泰能源内蒙古有限公司</a-menu-item>
            <a-menu-item key="4">久泰能源(准格尔)有限公司</a-menu-item>
            <a-menu-item key="5">久泰能源(广州)有限公司</a-menu-item>
            <a-menu-item key="6">久泰能源(张家港)有限公司</a-menu-item>
            <a-menu-item key="7">久泰能源(北京)有限公司</a-menu-item>
            <a-menu-item key="8">山东联建华星精瓷有限公司</a-menu-item>
            <a-menu-item key="9">山东兴泰机械装备工程有限责任公司</a-menu-item>
            <a-menu-item key="10">内蒙古久泰新材料有限公司</a-menu-item>
            <a-menu-item key="11">鄂尔多斯市久泰建筑安装有限公司</a-menu-item>
            <a-menu-item key="12">久泰集团销售有限责任公司</a-menu-item>
            <a-menu-item key="13">内蒙古久泰新材料销售有限公司</a-menu-item>
          </a-menu>
        </a-layout-sider>
        <a-layout style="padding: 0 15px 15px">
          <a-layout-content>
            <nuxt />
          </a-layout-content>
          <a-layout-footer style="text-align: center">
            Copyright © 2019 Savor,All Rights Reserved.
          </a-layout-footer>
        </a-layout>
        <div :style="{ background: '#fff' }">
          <div
            :style="{
              padding: '10px',
              background: 'rgb(28, 97, 162)',
              color: '#fff'
            }"
          >
            <span>供应商登录</span>
          </div>
          <a-form
            :style="{
              background: '#fff',
              textAlgin: 'center',
              marginLeft: '20px',
              marginTop: '10px'
            }"
          >
            <a-form-item label="用户名" style="margin-bottom: 10px">
              <a-input
                v-decorator="[
                  'username',
                  {
                    rules: [{ required: true, message: '请输入用户名!' }]
                  }
                ]"
              />
            </a-form-item>
            <a-form-item label="密码" style="margin-bottom: 10px">
              <a-input
                v-decorator="[
                  'password',
                  {
                    rules: [{ required: true, message: '请输入密码!' }]
                  }
                ]"
              />
            </a-form-item>
            <a-form-item
              :wrapper-col="{ span: 21, offset: 3 }"
              :style="{ marginTop: '20px' }"
            >
              <a-button
                type="primary"
                :style="{ background: 'rgb(28, 97, 162)', width: '150px' }"
                html-type="submit"
              >
                登录
              </a-button>
              <div :style="{ marginLeft: '5px' }">
                <a>用户注册</a>
                <a-divider type="vertical"></a-divider>
                <a>忘记密码?</a>
              </div>
            </a-form-item>
          </a-form>
        </div>
      </a-layout>
    </a-layout>
  </div>
</template>

<style>
html {
  font-family: 'Source Sans Pro', -apple-system, BlinkMacSystemFont, 'Segoe UI',
    Roboto, 'Helvetica Neue', Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

.logo {
  background-image: url('../static/image/head_bg.jpg');
}

*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
}

.button--green {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #3b8070;
  color: #3b8070;
  text-decoration: none;
  padding: 10px 30px;
}

.button--green:hover {
  color: #fff;
  background-color: #3b8070;
}

.button--grey {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #35495e;
  color: #35495e;
  text-decoration: none;
  padding: 10px 30px;
  margin-left: 15px;
}

.button--grey:hover {
  color: #fff;
  background-color: #35495e;
}
.ant-carousel /deep/ .slick-slide {
  text-align: center;
  height: 253px;
  line-height: 160px;
  overflow: hidden;
}

.ant-carousel /deep/ .custom-slick-arrow {
  width: 25px;
  height: 25px;
  font-size: 25px;
  color: #fff;
  background-color: rgba(31, 45, 61, 0.11);
  opacity: 0.3;
}
.ant-carousel /deep/ .custom-slick-arrow:before {
  display: none;
}
.ant-carousel /deep/ .custom-slick-arrow:hover {
  opacity: 0.5;
}
.ant-carousel >>> .slick-slide img {
  color: #fff;
}
</style>
