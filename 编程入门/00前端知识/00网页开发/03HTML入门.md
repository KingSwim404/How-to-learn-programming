# HTML入门(实践课)

1. 学习必要的HTML标签：

   [示例详细代码01](代码相关/demo01.html)

   ```html
   <!-- 这个是注释,用于解释只用，不影响程序。 -->
   <!-- 1、显示一个文本段落 -->
   <p>KingSwim</p>
   <!-- 2、显示一张图片 -->
   <img src="https://www.kingswim.xyz/xyz/img/kingswim.png" alt="KingSwim的头像"/>
   <!-- 3、超链接 -->
   <a href="https://www.kingswim.xyz/">KingSwim的官网</a>
   <!-- 4、容器标签，用于划分区域 -->
   <div>KingSwim</div>
   <div>
       <p>KingSwim</p>
       <a href="https://www.kingswim.xyz/">KingSwim的官网</a>
       <a href="https://www.kingswim.xyz/">KingSwim的官网</a>
   </div>
   ```

2. 标签的规范

   HTML是一种极度不严谨的标签语言。它有规范，但是你不遵守，它也可以运行，甚至从界面上还看不出错误来。

   请记住下面几条规范即可：

   - 标签都需要闭合。

     ```html
     <p></p>   (正确)
     <p><p/>   (错误)
     <br/>     (正确)  自闭合标签  
     ```

   - 标签不可以交叉嵌套。

     ```html
     <div><p></p></div>   (正确)
     <div><p></div></p>   (错误)
     ```

   - 标签要语义化

     ```html
     <div><p>KingSwim</p></div>  (正确) 
     <div>KingSwim</div>         (错误)
     记住：
     代码是写给人看的，写给机器运行的。
     后面我会经常强调这一点，后续讲代码优化的时候还会反复强调。                      
     ```
     

3. 自练习：

   - 自行学习如何显示：视频、音频。
   - 自行学习如何链接到本地路径。