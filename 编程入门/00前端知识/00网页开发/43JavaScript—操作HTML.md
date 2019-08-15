# JavaScript—操作 HTML

[示例详细代码53](代码相关/demo53-JavaScript-dom.html)

- ### HTML代码：

  ```html
  <p id="p0">KingSwim0</p>
  
  <p id="p1">KingSwim1</p>
  
  <p class="p2">KingSwim2</p>
  <p class="p2">KingSwim3</p>
  <p class="p2">KingSwim4</p>
  ```

  

- ### 如何修改标签上面的文本：

  ```javascript
      //获取一个id标签：
      // document 代表整个页面。通过id找到对应的元素。
      let p0 = document.getElementById("p0");
      //修改 p0 的文本
      p0.innerText = "修改之后~~";
  ```

  

- ### 如何在标签上面新增其他标签：

  ```javascript
      //在p1标签内部新增标签
      let p1 = document.getElementById("p1");
      //注意：字符串用""包裹。字符串里面还有字符串，就得使用''包裹。
      p1.innerHTML = "<a href='http://www.kingswim.xyz' >XYZ<a/>";
      //结果：<p id="p1"><a href='http://www.kingswim.xyz' >XYZ<a/></p>
  ```

  

- ### 其他获取标签的方式：

  ```javascript
      // 获取一个class标签：
      // 获取文本为KingSwim3的标签。
      /*
        请注意： getElementById
                getElementsByClassName
  
         第一个其中有个单词是：Element (单数)
         第二个的为：Elements （复数）
         getElementById  ： 获得的是一个标签
         getElementsByClassName ： 获得的是一个标签数组。
  
         还记得之前说过：id 一个页面只能有一个。现在能明白么？
       */
  
      let p2s = document.getElementsByClassName("p2");
  
      let ks3 = p2s[1];
  
          ks3.innerText = "KingSwim03";
  
  
      /*
        另外一种CSS选择器写法：
       */
  
       let cP0 = document.querySelector("#p0");
       //类似 document.getElementById("p0");
  
  
       let cP2 = document.querySelector(".p2");
       /*
        类似:document.getElementsByClassName("p2")[0];
            永远取得符合CSS选择器里面的第一个
        */
  
       let cP2s = document.querySelectorAll(".p2");
        /*
         类似:document.getElementsByClassName("p2");
             获得的是所有符合条件的标签
         */    
  
       /*
        以上选择是否正确自己测试一下。
       */
  ```

- ### 自练习：

  - 测试一下querySelector、querySelectorAll 是否符合上面的说的。