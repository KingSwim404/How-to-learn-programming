# JavaScript—实现平移动画

[示例详细代码57](代码相关/demo57-JavaScript-animation.html)

- ### HTML代码：

  ```html
  <style>
  
       #div0 {
              width: 200px;
              height: 200px;
              margin: 100px auto;
              background-color: blue;
          }
  
        #btn {
              width: 100px;
              display: block;
              margin: 10px auto;
          }
  </style>
      
  <div id="div0"></div>
  <button id="btn">启动</button>
  ```

  

- ### JavaScript代码：

  ```javascript
      /*
         用 js 实现一个平移动画：
       */
  
      let btn = document.querySelector("#btn");
      let div0 = document.querySelector("#div0");
  
      let isRun = false; //动画是否启动
  
      let interval= null;
  
      btn.addEventListener("click", function () {
          //取反
          isRun =!isRun;
          if (isRun) {
              //启动平移动画
              interval = translateX(div0,400);
              btn.innerText = "暂停";
          } else {
              //暂停
              clearInterval(interval);
              btn.innerText = "启动";
          }
          
      });
  
      /**
       *
       * @param ele
       *        需要执行的标签
       * @param distance
       *        移动的距离
       * @returns
       *         执行器
       */
      function translateX(ele,distance) {
          let totalStep = 0;//总步长
          let part = distance/100.0 ; //单位步长
          let interval = setInterval(function () {
               //分为 100 次
               totalStep = totalStep + part;//
               ele.style.transform = "translateX("+totalStep+"px)";
               // Math.abs() 求绝对值。
               if(totalStep >= Math.abs(distance)){
                   //当走到的总步数大于等于目标距离，关掉移动动画
                   clearInterval(interval);
                   //还原
                   ele.style.transform = "translateX(0px)";
                   btn.innerText = "启动";
                   isRun = false;
               }
          },16);
          //将执行器返回出去方便控制暂停。
          return interval;
      }
  ```

- ### 自练习：

  - JavaScript的逻辑性比CSS的要抽象一些，所以先把逻辑看懂再去模仿写。一旦熟练，就去模拟一下360°旋转的动画（这个时候你差不多就可以试试写旋转抽奖的代码了）。
  - 想一下用CSS实现动画和JavaScript实现各自的好处在于哪里？