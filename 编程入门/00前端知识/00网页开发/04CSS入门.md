# CSS入门（实践课）

1. 学习必要的CSS属性：
   [示例详细代码02](代码相关/demo02.html)
   ```html
   <style rel="stylesheet" type="text/css">
           /* 代表控制p标签的CSS */
           p {
               /*css 的注释写法*/
               /*宽*/
               width: 100px;
               /*高*/
               height: 50px;
               /*文本大小*/
               font-size: 26px;
               /*文本颜色*/
               color: blue;
           }
           /*
               其实以上代码代表控制所有p标签的，你会发现所有的p标签都应用了以上CSS。
               显然这样不好。有的时候我需要《KingSwim1》的文本是红色，怎么办？
               这个时候就引出了另一个知识点：CSS选择器。
           */
       </style>
   ```
   
2. 学习必要的[CSS 选择器](http://www.w3school.com.cn/cssref/css_selectors.asp) ：
   [示例详细代码03](代码相关/demo03.html)
   - 标签选择器

     格式：标签名 {    }
     
     
     
   - id选择器
   
     格式：# + id名 {  } 
   
     注意：id整个 HTML页面要唯一。当然，你可以不遵守，但是一定要遵守。后续你会知道理由。
   
     
   
   - class选择器
   
     格式：. + class名 {  } 