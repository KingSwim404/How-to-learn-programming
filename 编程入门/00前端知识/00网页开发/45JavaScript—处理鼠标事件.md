# JavaScript—处理鼠标事件

[示例详细代码55](代码相关/demo55-JavaScript-event.html)

- ### HTML代码：

  ```html
  <style>
      
          #div0{
              width: 200px;
              height: 200px;
              background-color: #0000FF;
          }
  
          #div1{
              width: 200px;
              height: 200px;
              background-color: red;
          }
  </style>
  
  <div id="div0"></div>
  <div id="div1"></div>
  ```

  

- ### 监听鼠标点击事件：

  ```javascript
      //1、监听鼠标点击事件
      let div0 = document.querySelector("#div0");
      div0.addEventListener("click",function (event) {
           alert("我被点击了~~~");
      });
  ```

  

- ### 监听鼠标滑过事件（模拟CSS :hover ）：

  ```javascript
      //2、监听鼠标滑过事件：模拟CSS的hover。
  
      let div1 = document.querySelector("#div1");
  
      //鼠标滑入
      div1.addEventListener("mouseenter",function (event) {
          div1.style.backgroundColor = "yellow";
      });
  
      //鼠标滑出
      div1.addEventListener("mouseleave",function (event) {
          div1.style.backgroundColor = "blue";
      });
  ```

  

- ### 自练习：

  - JavaScript里面还有很多其他事件监听，想要继续深入学习的可以通过搜索自学一下。

