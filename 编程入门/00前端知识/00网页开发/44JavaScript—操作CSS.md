# JavaScript—操作 CSS

[示例详细代码54](代码相关/demo54-JavaScript-css.html)

- ### HTML 代码

  ```html
  <style>
        #div1{
              width: 200px;
              height: 100px;
              background-color: #00FF00;
          }
   </style>
  
  <div id="div0"></div>
  
  <div id="div1"></div>
  
  <img id="img0"  />
  ```

  

- ### JavaScript 设置 CSS

  ```javascript
   let div0 = document.querySelector("#div0");
       div0.style.width = "100px";
       div0.style.height = "100px";
       //css里面的中划线都要传化成首字母大写
       //background-color 转化为：backgroundColor
       div0.style.backgroundColor = "blue";
  ```

  

- ### JavaScript 获取 CSS

  ```javascript
  let div1 = document.querySelector("#div1");
  let width =  getComputedStyle(div1).width ;
   //另一种写法：let width =  getComputedStyle(div1)["width"] ;
    alert(width);//200px
  
    //如何转化为可以计算的数值 200
  let wtNum = parseInt(width); //parseInt去掉所有非数值的字母。
     alert(wtNum);//200
  ```

  

- ### JavaScript 设置 图片

  ```javascript
  let img0 = document.querySelector("#img0");
      img0.src = "imgs/kingswim.png"; 
  ```

- ### 自练习：

  - 尝试改变一些其他的 CSS 属性看看。

    