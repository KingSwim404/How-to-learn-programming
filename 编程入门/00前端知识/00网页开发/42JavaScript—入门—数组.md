# JavaScript—入门—数组

[示例详细代码52](代码相关/demo52-JavaScript-array.html)

- ### 数组的定义与操作：

  ```javascript
      /*
  
       如何管理多个数据？
       使用数组
  
       */
  
      // 数组：编程语言里面运用最多的数据结构。
      let array = [9, 2, 13, 43, 65, 32, 71, 98, 19];
      // let arr = []; //定义一个空数组
  
      // 数组的长度 = 数组的元素个数
      let len = array.length;
      console.log("数组长度=" + len); // 9
  
      // 获取数组的第3个元素。
      let thirdEle = array[2]; //取值要使用:n-1;规定：从0开始
      console.log("第三个元素=" + thirdEle);
  
      // 获取数组的最后一个元素。
      let lastEle = array[array.length - 1];
      console.log("最后一个元素=" + lastEle);
  
      //打印数组所有元素
      console.log(array);
  
      //新增一个元素：
      array.push(10086);
      console.log(array);
  
      //修改第一个元素为：10000
      array[0] = 10000;
      console.log(array);
  
      //循环迭代数组
      for (let i = 0; i < array.length; i++) {
          let ele = array[i] ;
          console.log("第" + (i + 1) + "个元素=" + ele);
      }
  ```

- ### 自练习：

  - 熟练掌握数组的以上操作
  - 试一试如何找出数组中最大的值