<template>
  <div id="particlesId">
    <div id="app">
      <!--
          https://aplayer.moefe.org/docs/guide/
          fixed:是否开启吸底模式     boolean
          mini:如果开启吸底模式，该选项可以控制播放器展开或收起    boolean
          theme:设置播放器默认主题颜色    string
          volume:设置播放器的音量   number
          mutex:是否开启互斥模式    boolean
          listFolded:是否折叠播放列表    boolean
          listMaxHeight:设置播放列表最大高度，单位为像素   number
      -->
      <aplayer autoplay :lrcType="3" :fixed="true"  :mini='true' :mutex='true' :listFolded="listFolded" mode='random' :audio="music"/>        
      <router-view/>
    </div>
  </div>
</template>

<script>
import particles from 'particles.js'
import particlesConfig from '../static/json/particles.json'
// import Aplayer from 'vue-aplayer'
export default {
  name: 'App',
  components:{
    // Aplayer
  },
   data () {
    return {
      listFolded:true,
      music:[
             {
              name: '东西（Cover：林俊呈)',
              artist: '纳豆',
              url: 'https://cdn.moefe.org/music/mp3/thing.mp3',
              cover: 'https://p1.music.126.net/5zs7IvmLv7KahY3BFzUmrg==/109951163635241613.jpg?param=300y300',
              lrc: 'https://cdn.moefe.org/music/lrc/thing.lrc'
            }, 
            {
              name: '响喜乱舞（Cover：MARiA）',
              artist: '泠鸢yousa',
              url: 'https://cdn.moefe.org/music/mp3/kyoukiranbu.mp3',
              cover: 'https://p1.music.126.net/AUGVPQ_rVrngDH9ocQrn3Q==/109951163613037822.jpg?param=300y300',
              lrc: 'https://cdn.moefe.org/music/lrc/kyoukiranbu.lrc'
            },
            {
              name: '此生不换',
              artist: '胡歌',
              url: 'https://amayaliu.cn/Music/%E6%AD%A4%E7%94%9F%E4%B8%8D%E6%8D%A2.mp3',
              cover:'//pic.xiami.net/images/album/img10/84110/3341821409825873.jpg?x-oss-process=image/resize,limit_0,m_fill,s_410/quality,q_80/format,jpg',
              lrc: 'https://www.amayaliu.cn/APlayer/lrc/%E9%9D%92%E9%B8%9F%E9%A3%9E%E9%B1%BC%20-%20%E6%AD%A4%E7%94%9F%E4%B8%8D%E6%8D%A2.lrc'
            },
      ]       
              
              
              
          


    }
   },
    created () {
      // this.$refs.aplayer.showLrc();  //显示歌词
      // this.$refs.aplayer.hideLrc();//隐藏歌词
      // this.$refs.aplayer.toggleLrc();//反选
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
          model: { jsonPath: './static/live2dw/live2d-widget-model-shizuku/assets/shizuku.model.json' },
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
