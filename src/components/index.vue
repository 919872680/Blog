
<template>
    <div>
       <header id="herds">
         <div  class="herdsNav">
            <img src="http://img5.imgtn.bdimg.com/it/u=2836714648,3992381933&fm=11&gp=0.jpg" alt="" title="前端'小白'鼠——点击查看">
            <div class="Amaya_liu"> Amaya丶呵呵</div>
            <ul class="NavRight">
               <li class="buttonBox" id="first">
                 <button >首页</button>
                 <div class="border"></div>
                 <div class="border"></div>
               </li>
               <li class="buttonBox" id="first">
                 <button >1283</button>
                  <div class="border"></div>
                  <div class="border"></div>
               </li>
               <li class="buttonBox" id="first">
                  <button >9798</button>
                  <div class="border"></div>
                  <div class="border"></div>
               </li>
            </ul>
         </div>
       </header>
       <div class="conent" style="height:5000px">
          <!-- 左布局 -->
          <leftContent/>
          <!-- 右布局 -->
          <rightNavigation/>
       </div>
    </div>
  </template>
  
  <script>
  import rightNavigation from './indexCompom/rightNavigation'
  import leftContent from './indexCompom/leftContent'
  export default {
    name: 'HelloWorld',
    components:{
      rightNavigation,
      leftContent
    },
    data () {
      return {
        msg: 'Welcome to Your Vue.js App'
      }
    }
  }
  </script>
  
  <!-- Add "scoped" attribute to limit CSS to this component only -->
  <style scoped>
      .herds { width: 100%;height: 90px;background: rgba(255, 255, 255, 0.52);border-bottom-left-radius: 20px;border-bottom-right-radius: 20px;font-size: 14px;box-shadow: 0 0 25px rgba(74, 59, 114,1);}
      .herds-nav {position: fixed;width:100%;top: -90px;-webkit-transition: top .5s;-moz-transition: top .5s;-o-transition: top .5s;transition: top .5s;}
      .herds-nav-appear {top: 0;}
      .herdsNav {
          margin: 0 auto;
          width: 1200px;
          height: 62px;
          border-radius: 10px;
          background: rgba(255, 255, 255, 0.52);
      }
      @media screen and (max-width: 1200px) {
        .herdsNav {
          width: 100% !important;
        } 
      }
      .herdsNav img {
          float: left;
          width: 62px;
          height: 62px;
          border-radius: 50%;
      }
      .Amaya_liu {
          float: left;
          margin-left: 15px;
          height: 62px;
          line-height: 62px; 
      }
      .NavRight {
          float: right;
      }
      @media (max-width: 991px) and (min-width: 750px) {
        .NavRight {
            margin-right: 20px;
        }
      }
      .buttonBox {
          position: relative;
          float: left;
          margin: 0 15px;
          line-height: 62px;
      }
      .NavRight button {
          width: 100px;
          height: 37px;
          position: relative;
          background: rgba(74, 59, 114,0.8);
          text-transform: uppercase;
          color: white;
          letter-spacing: 1px;
          border: none;
          font-size: 14px;
          outline: none;
          font-family: "华文楷体";
      }
      .border {
          position: absolute;
          background: none;
          transition: all .5s ease-in-out;
      }
      .all {
        transition-property: all;
        transition-duration: 0.5s;
        transition-timing-function: ease-in-out;
        transition-delay: 0s;
      }
      .buttonBox:hover .border{
          width: 102px !important;
          height: 37px !important;
      }
      #first > .border:nth-of-type(1) {
          top: 12px;
          left: -1px;
          border-left: 1px solid white;
          border-top: 1px solid white;
          width: 20px;
          height: 20px;
      }
      #first > .border:nth-of-type(2) {
          bottom: 11px;
          right: -1px;
          border-right: 1px solid white;
          border-bottom: 1px solid white;
          width: 20px;
          height: 20px;
      }
      /* 内容 */
      .conent{
        width: 1200px;
        margin: 0 auto;
      }
  </style>
