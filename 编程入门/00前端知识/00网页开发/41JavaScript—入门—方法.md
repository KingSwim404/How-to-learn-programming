# JavaScript—入门—方法

[示例详细代码51](代码相关/demo51-JavaScript-function.html)

- ### 方法：

  将一部分逻辑封装起来重复使用。

  格式：

    function 方法名（参数1,参数2）{} 

  ```javascript
      /*
  
       方法：可以理解为数学里面的函数表达式。
       例如：
          数学表达 —— f(x) = x + 1;
          代码表达 —— function f(x){ let y = x+1; }
  
       */
      // 1、无返回值的方法：
      //定义一个叫：say 方法
      function say(text) {
          alert(text);
      }
  
      //调用say方法。
      say("Hello");
  
      //2、有返回值的方法
  
      function getJoinText(text) {
          let result = "前缀——" + text;
          // 将结果返回
          return result;
      }
  
      let text = getJoinText("Hello");
      //显示获得的结果。
      alert(text);
  
  
      /*
        方法最大的作用：复用逻辑
       */
  
      //定义一个可以计算 ：0-n之间和的方法。
  
      function getSum(n) {
          let sum = 0;
          for (let i = 0; i <= n; i++) {
              sum = sum + i;
          }
          return sum;
      }
  
      let sum = getSum(100);
      alert(sum);
  ```

- ### 自练习：

  - 自己把上一节的作业，偶数之和封装成一个方法。