# JavaScript—延时器

[示例详细代码56](代码相关/demo56-JavaScript-timer.html)

- ### 间隔一段时间后，再做一件事情——做且只做一次

  ```javascript
      /*
       1、间隔一段时间后，再做一件事情——做且只做一次
  
        setTimeout( 需要执行的方法 , 时间-单位毫秒 );
       */
      console.log("开始~~~");
      let time = setTimeout(function () {
          console.log("3秒后~~~");
      }, 3000);
  
      // 取消延时器如下：
      // clearTimeout(time);
  ```

  

- ### 每隔一段时间后，做同一件事情——不断重复

  ```javascript
      /*
       2、 每隔一段时间后，做同一件事情——不断重复
           setInterval( 需要执行的方法 , 时间-单位毫秒 );
       */
  
       let interval = setInterval(function () {
                
           console.log("interval~~");
  
       },3000);
  
      //  这是一个死循环，取消循环如下：
      //  clearInterval(interval);
  ```

- ### 自练习：

  - 思考一下这两个功能可以用来做什么？

