# JavaScript—入门—分支

[示例详细代码49](代码相关/demo49-JavaScript-branch.html)

- ### if(){} else{}

  ```javascript
      /*
       1、if else 模式
       */
      let isHungry = false;
      if (isHungry) {
          alert("该吃东西了~~~~");
      } else {
          alert("就去散散步~~~~");
      }
  ```

- ### if(){} else if(){} ... else{}

  ```javascript
      /*
        以上只表达了2种分支情况，多种分支如何处理？
        使用如下形式：
  
        2、 if(){} else if(){} else if(){} .....else{}
  
        判断符号:
         相等：===
         不等：!==
         大于：>
         小于：<
      大于等于：>=
      小于等于：<=
  
       */
  
       let score = 70 ;
  
       if(score>=0 && score<60){
  
           alert("不及格~~~~");
  
       }else if(score===60){
  
           alert("刚好及格~~~~");
  
       }else if(score>60 && score<90){
  
           alert("一般~~~~");
  
       }else if(score>=90 && score<100){
  
           alert("优秀~~~~");
  
       }else if(score===100){
  
           alert("满分~~~~");
  
       }else{
  
           alert("分数有误~~~~");
       }
  ```

  

- ### 自练习：

  - 熟悉多分支的用法，注意{}不要括错了。你可以先写好模版，再去补充{}内的逻辑。一旦{}多起来了，很多人容易犯错。
  - 自学**三目运算符**以及**switch case**分支写法。

  