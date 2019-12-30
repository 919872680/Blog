<template>
  <div id="particlesId">
    <div id="app">
        <router-view/>
    </div>
  </div>
</template>

<script>
import particles from 'particles.js'
import particlesConfig from '../static/json/particles.json'
export default {
  name: 'App',
   data () {
    return {
    //  bodyBgImage: 'url(' + require('../assets/1.png') + ')'
    }
   },
    created () {
      var NowFrame=parseInt(Math.random()*3+1);
      document.getElementById('body').style.backgroundImage='url(' + require('./assets/img/'+NowFrame+'.jpg') + ')'
      document.getElementById('app').style.zIndex=999
      console.log(document.getElementById('app'))
      setTimeout(() => {
        window.L2Dwidget.init({
          pluginRootPath: 'static/live2dw/',
          pluginJsPath: 'lib/',
          pluginModelPath: 'live2d-widget-model-shizuku/assets/',
          tagMode: true,
          debug: false,
          model: { jsonPath: '/static/live2dw/live2d-widget-model-shizuku/assets/shizuku.model.json' },
          display: { position: 'right', width: 150, height: 300 ,hOffset: 10,vOffset:10 },
          mobile: { show: false },
          dialog:{default: true},
          log: true,
        })
      }, 1000)
    },
    mounted () {
      // 参数1 ，为div节点的id , 参数2，为particles.json配置文件
      particlesJS("particlesId",particlesConfig);
    },
    methods:{
      
    }
}
</script>

<style>
html, body, div, ul, li, h1, h2, h3, h4, h5, h6, p, dl, dt, dd, ol, form, input, textarea, th, td, select {
  margin: 0;
  padding: 0;
}
*{box-sizing: border-box;}
html, body {
  min-height: 100%;
}

body {
  font-family: "Microsoft YaHei";
  font-size:14px;
  color:#333;
  background-size: 100% 100%;
  background-repeat:no-repeat;
  background-attachment: fixed;
}
h1, h2, h3, h4, h5, h6{font-weight:normal;}
ul,ol {
  list-style: none;
}

img {
  border: none;
  vertical-align: middle;
}

a {
  text-decoration: none;
  color: #232323;
}

table {
  border-collapse: collapse;
  table-layout: fixed;
}
#app {
  position: absolute;
  width: 100%;
  top: 0;
  left: 0;
  z-index: 10;
}
#particlesId{
  position: absolute;
  width: 100%;
  height: 100%;
  background-repeat: no-repeat;
  background-size: cover;
  background-position: 50% 50%;
}
#particlesId .particles-js-canvas-el{
  position: fixed;
  top: 0;
  left: 0;
  z-index: 1;
}
</style>
