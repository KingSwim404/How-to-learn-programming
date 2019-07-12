# HTML、CSS增补知识点01(实践课)

1. ### HTML 标签增补知识点

   - [实体字符](http://www.w3school.com.cn/html/html_entities.asp)

     ```
     HTML多个空格会被识别成一个。
     示例：
     <p>King    Swim</p>   ====>  界面：King Swim
     如果，要表示多个空格你需要用：&nbsp;代替" "
     示例：
     <p>King&nbsp;&nbsp;&nbsp;&nbsp;Swim</p>   ====>  界面：King    Swim
     &nbsp; 就是实体字符。
     比较重要的几个实体字符：
     <   &lt;  
     >   &gt;
     ®   &reg;
     < 、 >会被浏览器解析成标签，所以一定要用实体字符，其他字符自行点击上面的链接学习。
     ```

   - 新标签

     - span

       文本标签——和 p 标签不同的是，它属于行内元素，界面显示排成一行。

       ```html
       <span>我也是一个文本标签0</span>
       <span>我也是一个文本标签1</span>
       
        显示如下：
        我也是一个文本标签0我也是一个文本标签1
       ```

     - br

       换行标签——行内元素默认都在一行，需要换行就使用它。

       ```html
       <span>我也是一个文本标签0</span>
       <br/>
       <span>我也是一个文本标签1</span>
       
       显示如下：
       我也是一个文本标签0
       我也是一个文本标签1
       ```

     - ol、li

       有序列表标签——默认竖排,默认序号数字 1 开始。

       ```html
       <ol >
           <li>KingSwim0</li>
           <li>KingSwim1</li>
           <li>KingSwim2</li>
           <li>KingSwim3</li>
           <li>KingSwim4</li>
       </ol>
       
       <!-- type：序号类型   ；start ：从哪个位置开始 -->
       <!-- 意思是 ：字母为序号，从字母 C 开始-->
       <ol id="ol01" type="A"  start="3" >
           <li>KingSwim0</li>
           <li>KingSwim1</li>
           <li>KingSwim2</li>
           <li>KingSwim3</li>
           <li>KingSwim4</li>
       </ol>
       ```

     - ul、li

       无序列表标签——默认竖排

       ```html
       <ul>
           <li>KingSwim0</li>
           <li>KingSwim1</li>
           <li>KingSwim2</li>
           <li>KingSwim3</li>
           <li>KingSwim4</li>
       </ul>
       ```

     - input

       输入框

       ```html
       <!-- 一般的输入框  type：决定类型 -->
       <input type="text"   />
       
       <!-- 一般的输入框 value ：默认值，输入不消失。 -->
       <input type="text"  value="KingSwim" />
       
       <!-- placeholder ：设置提示语 ，输入就消失-->
       <input type="text"  placeholder="请输入密码" />
       
       <!--密码框-->
       <input type="password"   />
       
       <!--只能输入数值-->
       <input type="number"   />
       
       <!--按钮，  value：按钮上面的文案-->
       <input type="button"  value="按钮" />
       <!--下面也是按钮，一般建议用下面的。-->
       <button>按钮</button>
       ```

   ##### 	[示例详细代码20](代码相关/demo20.html)，自行联系一下。

2. ### CSS 增补知识点

   - 内边距——padding

     控制标签内部的区域范围和 margin（外边距，恰恰相反）

     ```css
     #outer{
           width: 400px;
           height: 400px;
           background: #0000FF;
           /*
             自己的左边50px的区域无法放置任意标签
             效果和：在inner上面设置 margin-left: 50px;一样。（自己尝试一下。）
            */
           padding-left:50px ;
          }
     
       #inner{
           width: 50px;
           height: 50px;
           background: red;
          }
     
     <div id="outer">
         <div id="inner"></div>
     </div>
     
     ```

     

   - 背景图片设置

   - 文本居中

   - 边框

   - 浮动

   - hover

   - 隐藏显示

   - overflow hidden

   

3. ### 盒模型

   

4. ### 总结：

   大部分标签都可以当做文本以及图片标签使用。但是，一般请不要这么做。每个标签都有其自身的含义，尽量别乱用。

   后续，很少单独列增补知识点。直接就会在后续的小项目中：边做边学——做中学。以上的知识点都是基础知识点，基本上学完了就可以开始做简单的静态页面了。下面的教程就开始做一些小东西了。