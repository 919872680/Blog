
<template>
    <div class="Am_Recommend">
        <div class="BorderL BoxShadowHui">
            <img class="TitlImgA" src="../../assets/img/TitlImgB.jpg" alt="">
            <div class="Am_ReTopTowTile">
                <span class="fff fontSize14 ">Amaya丶夜雨博客</span> &nbsp; <span class="fontSize12 gray2">深圳前端"小白"鼠</span>
            </div>
            <div class="Am_ReTopTowCont">
                <ul>
                    <li>
                        文章
                        <br>
                        <b>2</b>
                    </li>
                    <li>
                        文章
                        <br>
                        <b>2</b>
                    </li>
                    <li>
                        文章
                        <br>
                        <b>2</b>
                    </li>
                    <li>
                        文章
                        <br>
                        <b>2</b>
                    </li>
                </ul>
            </div>
        </div>

       <div id="" class="BoxShadowHui BorderL Am_ReTopThr">
           <div class="Am_ReTopThrCont">
                你必须非常努力，才能看起来毫不费劲。 <br/>
                You have to work very hard to look effortless.
           </div>
           <div class="Am_ReTopThrTile">
                <svg style="margin-top:8px;" width='100%' height='100%' xmlns="http://www.w3.org/2000/svg">
                    <g>
                        <text font-size="18" text-anchor="middle" x="50%" y="50%" text-transform="uppercase" fill="none"  stroke="#3498db" text-shadow="0 0 1px #3498db" stroke-width="1px" stroke-dasharray="90 310">
                            ♪♫Autograph♫♪
                            <animate attributeName="stroke-dashoffset" begin="-1.5s" dur="6s" from="0" to="-400" repeatCount="indefinite"></animate>
                        </text>
                        <text font-size="18" text-anchor="middle" x="50%" y="50%" text-transform="uppercase" fill="none"  stroke="#f39c12" text-shadow="0 0 1px #3498db" stroke-width="1px" stroke-dasharray="90 310">
                            ♪♫Autograph♫♪
                            <animate attributeName="stroke-dashoffset" begin="-3s" dur="6s" from="0" to="-400" repeatCount="indefinite"></animate>
                        </text>
                        <text font-size="18" text-anchor="middle" x="50%" y="50%" text-transform="uppercase" fill="none"  stroke="#e74c3c" text-shadow="0 0 1px #3498db" stroke-width="1px" stroke-dasharray="90 310">
                            ♪♫Autograph♫♪
                            <animate attributeName="stroke-dashoffset" begin="-4.5s" dur="6s" from="0" to="-400" repeatCount="indefinite"></animate>
                        </text>
                        <text font-size="18" text-anchor="middle" x="50%" y="50%" text-transform="uppercase" fill="none"  stroke="#9b59b6" text-shadow="0 0 1px #3498db" stroke-width="1px" stroke-dasharray="90 310">
                            ♪♫Autograph♫♪
                            <animate attributeName="stroke-dashoffset" begin="-6.5s" dur="6s" from="0" to="-400" repeatCount="indefinite"></animate>
                        </text>
                    </g>
                </svg>
           </div>
       </div>

        <div id="" class="BoxShadowHui BorderL Am_ReTopThr">
           <div class="Am_ReTopFourCont">
                <ul>
                    <li>HTML</li>
                    <li>CSS</li>
                    <li>Javascript</li>
                    <li>Ajax</li>
                    <li>Vue.js</li>
                    <li>Node.js</li>
                    <li>微信小程序</li>
                </ul>
           </div>
           <div class="Am_ReTopThrTile text_shadowZ">
                <span class="red">♪</span>技<span class="red">♫</span>术<span class="mus">♪</span><span class="red">♪</span>版<span class="red">♫</span>块<span class="mus">♪</span>
           </div>
       </div>

        <div id="" style="text-align:left;" class="BoxShadowHui BorderL Am_ReTopThr">
           <div class="Am_ReTopFiveCont">
                <ul>
                    <li>
                         Amaya丶夜雨
                    </li>
                    <li>
                        <a href="http://mail.qq.com/cgi-bin/qm_share?t=qm_mailme&email=919872680@qq.com">
                            919872680@qq.com
                        </a>
                    </li>
                    <li>
                        暂无信息
                    </li>
                </ul>
           </div>
           <div class="Am_ReTopThrTile text_shadowZ" style="text-align:center;">
                 <span class="red">♪</span>联<span class="red">♫</span>系<span class="mus">♪</span><span class="red">♪</span>方<span class="red">♫</span>式<span class="mus">♪</span>
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
  <style>
    .Am_Recommend {
        float: right;
        width: 27%;
        height: 100%;
        /* background-color: rgba(129, 119, 127, 0.40); */
        /* background: #9c9c9c; */
        /* box-shadow: 0 0 10px #cbcbcb; */
        margin-bottom: 0px;
    }
    .Am_ReTopTow {
        margin-top: 25px;
        width: 100%;
        height: 377px;
        background-color: rgba(129, 119, 127, 0.40);
    }
    .TitlImgA {
        display: block;
        width: 100%;
    }
    .Am_ReTopTowTile {
        position: relative;
        margin-top: -50px;
        display: block;
        width: 100%;
        height: 50px;
        line-height: 50px;
        background-color: rgba(129, 119, 127, 0.60);
        text-align: center;
    }
    .fontSize14 {
        font-size: 14px;
    }
    .fff {
        color: #fff;
    }
    .gray2 {
        color: #d4d4d4;
    }
    .fontSize12 {
        font-size: 12px;
    }
    .Am_ReTopTowCont {
        width: 99.6% !important;
        margin: auto;
        height: 75px;
        background: #fff;
    }
    .Am_ReTopTowCont ul li {
        float: left;
        width: 79.88px;
        line-height: 22px;
        text-align: center;
        margin-top: 17px;
        border-right: 1px solid #d3d3d3;
    }
    .Am_ReTopTowCont ul li:last-child {
        border-right: none !important;
    }
    .BoxShadowHui {
        box-shadow: 0 0 10px #cbcbcb;
    }
    .BorderL {
        border-left: 0.3px solid #e2dbb9;
        border-top: 0.3px solid #cbcbcb;
        border-bottom: 0.3px solid #cbcbcb;
        border-right: 0.3px solid #cbcbcb;
    }
    .Am_ReTopThr {
        margin-top: 25px;
        width: 100%;
        height: 250px;
        background-color: rgba(129, 119, 127, 0.40);
        text-align: center;
    }
    .Am_ReTopThrCont {
        margin: 60px 0 30px 0;
        width: 100%;
        height: 100px;
        line-height: 40px;
        font-size: 14px !important;
        color: #000;
        text-shadow: 0 0 5px #fff, 0 0 10px #fff, 0 0 15px #fff, 0 0 20px #FF1177, 0 0 35px #FF1177, 0 0 40px #FF1177, 0 0 50px #FF1177, 0 0 75px #FF1177;
    }
    .Am_ReTopThrTile {
        width: 99.6%;
        margin: auto;
        height: 60px;
        background: #fff;
        line-height: 60px;
    }
    .Am_ReTopFourCont {
        width: 100%;
        height: 173px;
    }
    .Am_ReTopFourCont ul {
        margin: 15px 0 0 7px;
    }
    .Am_ReTopFourCont ul li {
        float: left;
        padding: 2px 4px;
        margin: 3px 7px;
        color: #f0ff29;
        box-shadow: 0 0 10px #cbcbcb;
        font-size: 14px;
    }
    .text_shadowZ {
        text-shadow: 3px 1px 2px #6839aa;
    }
    .red {
        color: red;
    }
    .mus {
        color: #1e90ff;
    }
    .Am_ReTopFiveCont{
        width: 90%;
        height: 178px;
        margin: 10px auto 0;
    }
    .Am_ReTopFiveCont ul li {
        border-bottom: 0.3px solid #b7b7b7;
        line-height: 40px;
    }
  </style>
