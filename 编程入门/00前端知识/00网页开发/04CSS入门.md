# CSS入门（实践课）

1. 学习必要的CSS属性：
   [示例详细代码02](代码相关/demo02.html)
   
   ```html
   <style rel="stylesheet" type="text/css">
           /* 代表控制p标签的CSS */
           p {
               /*css 的注释写法*/
               /*宽*/
               width: 200px;
               /*高*/
               height: 50px;
               /*文本大小*/
               font-size: 26px;
               /*文本颜色*/
               color: blue;
               /*背景颜色*/
               background: black;
           }
            /*
               其实以上代码代表控制所有p标签的，你会发现所有的p标签都应用了以上CSS。
               显然这样不好。有的时候我需要:
               1、"KingSwim1"的文本是红色，怎么办？
               2、"KingSwim3"、"KingSwim4"的文本是绿色，怎么办？
               这个时候就引出了另一个知识点：CSS选择器。
   
               注意：如果你的代码没有出效果。请看你是不是少了"："或者";"或者“{}”
                    CSS比HTML要严格一些。
           */
       </style>
   ```
   
2. CSS的规范
   
   CSS相对HTML来说要严谨的多。如果，写错了，页面上就不会有效果。

   请记住下面的规范即可：
   
   - 一般格式如下：
   
     ```
     xxx0{ 
          yyyy0 : zzzz0;
          yyyy1 : zzzz1;
         }
         
     注意：刚刚开始学习CSS，会经常出错，丢失符号。所以大家一定要小心，不要求快。
          花括号括错是一个初学容易犯的错误，而且还不容易发现，代码格千万要规范。    
     ```
   
     
   
3. 学习必要的[CSS 选择器](http://www.w3school.com.cn/cssref/css_selectors.asp) ：
   
 [示例详细代码03](代码相关/demo03.html)
   
- 标签选择器：指定某种标签；
   
     格式：标签名 {    }
     
     ```html
     <p>KingSwim0</p>
     p{color: orange;}
     ```
     
- id选择器：指定某一个标签；
   
  注意：id整个HTML页面要唯一。当然，你可以不遵守，但是一定要遵守。先记住这个，后续会知道理由。
   
     格式：#+id名 {    }
   
     ```html
     <p id="red_text">KingSwim1</p>
    #red_text{ color: red;}
  ```
   
   - class选择器：指定某一些标签
   
     格式：. + class名 {  } 
     
     ```html
     <p class="green_text" >KingSwim3</p>
     <p class="green_text" >KingSwim4</p>
     .green_text{color: green;}	
     ```
     
   - 父子选择器：（这个很重要，后续会经常用到——很方便）
   
     先说几个概念：
     
     父元素、子元素、直接父元素、直接子元素。
     怎么分辨这几个概念：请看[示例详细代码04](代码相关/demo04.html)
     父子选择器代码详细示例：[示例详细代码05](代码相关/demo05.html)
   
       ```html
       <div id="div0">
           <p id="p0">p0</p>
           <p id="p1">p1</p>
           <div id="div1">
             <p id="p2">p2</p>
           </div>
       </div>
       ```
   
     - 子选择器
   
       格式： 父+空格+子{  }
   
       代码示例：
   
       ```html
       <style>
            #div0 p{
                 color: blue;
             }
       </style>
       ```
   
     - 直接子选择器
     
       格式： 父+>+子{   }
     
       代码示例：
   
       ```html
       <style>
            #div0>p{
                 color: red;
             }
       </style>
       ```
   
4. 自练习

   - 尝试一下此种格式的CSS选择器 xxx yyy zzz和xxx>yyy>zzz是否符合你的预期。
   - 预习一下RGB代表哪几种颜色。
