# CSS 动画知识点

1. ### 常规动画分类：

   [示例详细代码35](代码相关/demo35-animation.html)

   - 平移

     ```css
             div {
     
                 width: 100px;
                 height: 100px;
                 background-color: #0000FF;
                 margin: 100px auto;
                 color: #FF0000;
                 /*
                   设置过渡效果和时间
                   这个属性没有的话，动画就会很生硬,瞬间就执行完毕——自己试试看
                   all:所有属性都有过渡效果；（一般设为 all）
                   2s :动画执行2秒
                   不能在 hover 里设置这个。是否过度应该是还没有hover就确定了。
                 */
                 transition: all 2s;
             }
     
             /*  平移动画 */
             .div00:hover{
                  /* X 轴移动 400px */
                  transform: translateX(400px);
                  /* Y 轴移动 400px */
                 /*transform: translateY(400px);*/
                 /* X、Y 轴同时移动 400px */
                 /*transform: translate(400px,400px);*/
             }
     ```
   - 缩放

     ```css
             /* 缩放动画 */
             .div01:hover{
                 /* 整个放大 2 倍 */
                 transform: scale(2);
                 /* X 轴方向放大 2 倍 */
                 /*transform: scaleX(2);*/
                 /* Y 轴方向放大 2 倍 */
                 /*transform: scaleY(2);*/
             }
     ```
   - 旋转

     ```css
            /* 旋转动画 */
             .div02:hover{
                 /* 顺时针旋转 90 度 */
                 transform: rotate(90deg);
                 /* 围绕 X 轴旋转 90 度 （应该是一条水平直线了——恰好界面看不到了）*/
                 /*transform: rotateX(90deg);*/
                 /* 围绕 Y 轴旋转 90 度 */
                 /*transform: rotateY(90deg);*/
             }
     
     ```
   - 复合

     ```css
            /* 复合动画 */
             .div03:hover{
                 /*多个动画一起执行，每个动画之间空格 */
                 transform: translate(400px,400px)  scale(2) rotate(90deg) ;
             }
     ```
   - 一切皆可动画

     ```css
             /* 一切皆可动画 */
             .div04:hover{
                 /* 宽度变化 */
                 width: 500px;
                 /* 颜色变化 */
                 /*background-color: #00FF00;*/
             }
     
     ```
   - 动画延时

     ```css
             /* 动画延时 */
             .div05{
                 /* 延时2秒执行 */
                 transition-delay: 2s;
             }
             .div05:hover{
                 transform: translateX(100px);
             }
     
     ```
   - 指定动画原点

     ```css
            /* 指定动画原点 */
             .div06{
                 /* 默认是中心点即：50% 50% 或者 center*/
                 /* 值可以是：具体数值，百分比，方位（center\top\left等） */
                 transform-origin: 0% 0%;
             }
             .div06:hover{
                 transform: rotate(90deg);
             }
     ```

2. ### 自练习：

   - 熟练运用动画相关属性





