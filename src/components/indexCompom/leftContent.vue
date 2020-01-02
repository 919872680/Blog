
<template>
    <div class="Am_Subject">
       <div class="Am_Sub" style="visibility: visible;opacity: 1;transform: matrix3d(1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1);transition: opacity 0.6s ease-in-out 0s, transform 0.6s ease-in-out 0s;">
            <div class="SubImgDiv">
                <img src="../../assets/img/下载.jpeg" class="SubImg" alt="">
            </div>
            <div class="Am_SubCont">
                <p>
                    <span class="Am_SubTile">【H5播放器之——APlayer】</span>
                    <br/>
                    <span class="Am_SubDate">
                        <span class="Am_YdAAuthor">
                            <img class="Am_SubTX" src="http://img5.imgtn.bdimg.com/it/u=2836714648,3992381933&fm=11&gp=0.jpg" alt="">
                             Amaya丶夜雨  |    H5播放器  |  2019-11-18 10:25:03  
                        </span>
                    </span>
                    <br/>
                    <span class="AM_SubAuxiliary">
                        APlayer是一款H5音乐播放器，拥有各种你想要的播放模式。它的地址是https://aplayer.js.org。本着太久没有鼓捣一些玩意，弄了一个以前想写的播放器(效果见右下角)  ，没时间写就找了一个，还有太多东西要更新了，一直拖着。。。。  
                    </span>
                </p>
            </div> 
       </div>
         
    </div>
  </template>
  
  <script>
  export default {
    name: 'HelloWorld',
    data () {
      return {
        msg: 'Welcome to Your Vue.js App'
      }
    }
  }
  </script>
  
  <!-- Add "scoped" attribute to limit CSS to this component only -->
  <style scoped>
    .Am_Subject {
        float: left;
        width: 70%;
        height: 100%;
        background-color: rgba(255, 255, 255, 0.70);
        padding: 20px 0;
        margin-top: 25px;
    }
    .Am_Sub:hover {
        box-shadow: 0 0 10px #cbcbcb;
        /* box-shadow: 0 0 25px rgba(74, 59, 114,1); */
        transition: all 0.5s !important;
    }
    .Am_Sub:nth-child(1) {
        margin-top: 0px;
    }
    .Am_Sub {
        width: 95%;
        height: 150px;
        margin: auto;
        margin-top: 20px;
        /* border: 1px solid red; */
        overflow: hidden;
    }
    .SubImgDiv {
        float: left;
        width: 238px;
        height: 150px;
        overflow: hidden;
    }
    .SubImg {
        width: 238px;
        height: 150px;
        transition: all 1s;
    }
    .all{
        transition-property: all;
        transition-duration: 1s;
        transition-timing-function: ease;
        transition-delay: 0s;
    }
    .SubImg:hover {
        transform: scale(1.05);
    }
    .Am_SubCont {
        float: left;
        height: 150px;
        width: 67.8%;
        margin-left: 2%;
        text-shadow: 0 0 15px #fff, 0 0 30px #fff;
    }
    .Am_SubTile {
        line-height: 30px;
        font-size: 15px;
        color: #000;
    }
    .Am_SubDate {
        line-height: 30px;
        font-size: 10px !important;
        color: #3e3e3e;
    }
    .Am_SubTX {
        vertical-align: middle;
        width: 18px;
        height: 18px;
        border-radius: 50%;
    }
    .Am_SubDescribe {
        line-height: 20px;
        font-size: 12px;
        color: #262626;
    }
  </style>
