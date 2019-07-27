# 练习09—腾讯大学—Content-right（实践课）

1. ### HTML：

   ```html
           <aside id="content-right">
               <h3><span></span>排行榜</h3>
               <div class="hottest">
                   <div class="hottest-list">
                       <h3>
                           <a>最热排行</a><a>新课上线</a>
                       </h3>
                       <ul class="pic-text">
                           <li>
                               <img src="imgs/img-daxue/1510631401811.jpg"/>
                               <p><a href="#">1</a><a href="#">腾讯8分钟产品课|第二集：定位</a></p>
                           </li>
                           <li>
                               <img src="imgs/img-daxue/1452663224623.jpg"/>
                               <p><a href="#">2</a><a href="#">张小龙：微信四大价值观</a></p>
                           </li>
                           <li>
                               <img src="imgs/img-daxue/1510631401811.jpg"/>
                               <p><a href="#">3</a><a href="#">腾讯8分钟产品课|第二集：定位</a></p>
                           </li>
                           <li>
                               <img src="imgs/img-daxue/1510631401811.jpg"/>
                               <p><a href="#">4</a><a href="#">腾讯8分钟产品课|第二集：定位</a></p>
                           </li>
                           <li>
                               <img src="imgs/img-daxue/1510631401811.jpg"/>
                               <p><a href="#">5</a><a href="#">腾讯8分钟产品课|第二集：定位</a></p>
                           </li>
   
                       </ul>
   
                       <ul class="index-text">
                           <li>
                               <p>
                                   <span>6</span>
                                   <a class="singleline-omit" href="#">马化腾：“互联网+”时代，腾讯只做连接器和内容</a>
                               </p>
                           </li>
                           <li>
                               <p>
                                   <span>7</span>
                                   <a class="singleline-omit" href="#">腾讯8分钟产品课|第一集：用户</a>
                               </p>
                           </li>
                           <li>
                               <p>
                                   <span>8</span>
                                   <a class="singleline-omit" href="#">何凌南：谣言在想什么</a>
                               </p>
                           </li>
                           <li>
                               <p>
                                   <span>9</span>
                                   <a class="singleline-omit" href="#">张小龙：4小时演讲，全面总结微信8年</a>
                               </p>
                           </li>
                           <li>
                               <p>
                                   <span>10</span>
                                   <a class="singleline-omit" href="#">腾大直播间|红海中寻生路，化被动为主动的产品思考</a>
                               </p>
                           </li>
                       </ul>
                   </div>
               </div>
               <div class="gray-split-line">
               </div>
   
               <div class="communication">
                   <div class="pic-mark">
                       <img src="imgs/img-daxue/1437012075279.png" />
                       <img class="mark" src="imgs/img-daxue/icon-mark.png" alt="mark"/>
                   </div>
                   <p>腾讯大学</p>
                   <p>腾讯大学作为腾讯特色的学习交流平台，服务于腾讯合作伙伴及用户，面向互联网产业链，传播腾讯经验，分享行业知识及优秀实践，助力合作伙伴成长，推动开放共赢的互联网生态圈的建立。</p>
               </div>
   
               <div class="gray-split-line">
               </div>
               <div class="contact">
                   <h3><span></span><span>联系我们</span></h3>
                   <p>合作：university@tencent.com <br/> QQ&nbsp;：2813343187</p>
                   <div class="exam">
                       <span>在线考试</span>
                       <a href="#">ENTER入口</a>
                   </div>
               </div>
           </aside>
   ```

   

2. ### CSS：

   ```css
           /*========================中间右边区域*/
   
           #content-right {
               width: 270px;
               height: 100%;
               padding: 22px;
               float: right;
               /* 防止内边距把区域变大 */
               box-sizing: border-box;
               background: white;
           }
   
   
           /*=================排行榜*/
           #content-right .hottest {
               width: 228px;
               height: 1120px;
               /*border: 1px solid blue;*/
               position: relative;
           }
   
           #content-right>h3>span {
               display: inline-block;
               width: 20px;
               height: 20px;
               background: url("imgs/img-daxue/icon-rank.png");
               margin-right: 13px;
           }
   
           #content-right>h3 {
               font-weight: 100;
               font-size: 22px;
               margin-bottom: 20px;
           }
   
           .hottest .hottest-list{
               width: 228px;
               height: 1105px;
               position: absolute;
               top: 0;
               left: 0;
           }
   
           .hottest .hottest-list>h3 {
               width: 226px;
               height: 34px;
               background: url("imgs/img-daxue/rank-tab-gray-bg.png") no-repeat center;
               padding-left: 2px;
               /*如果pading没有效果。
                * 一般是因为设置了怪异的盒模型的同时，子元素又比较大，所以移不动。*/
               padding-bottom: 2px;
               margin-bottom: 20px;
               box-sizing: border-box;
           }
   
           .hottest .hottest-list>h3>a {
               text-decoration: none;
               display: inline-block;
               color: black;
               font-size: 13px;
               width: 110px;
               height: 32px;
               text-align: center;
               line-height: 34px;
               box-sizing: border-box;
               border-left: 1px solid gainsboro;
           }
   
           .hottest .hottest-list>h3>a:nth-child(1) {
               border-top: 1px solid gainsboro;
           }
   
           .hottest .hottest-list>h3>a:nth-child(2) {
               border-bottom: 1px solid gainsboro;
           }
   
   
           /*==============图文混排列表*/
           .hottest .pic-text>li {
               width: 228px;
               height: 162px;
               margin-bottom: 20px;
               position: relative;
           }
   
           .hottest .pic-text>li>img {
               width: 228px;
               height: 162px;
           }
   
           .hottest .pic-text>li>p {
               position: absolute;
               left: 0;
               bottom: 0;
               background-color: rgba(0, 0, 0, 0.5);
               font-size: 13px;
               width: 228px;
               height: 27px;
           }
   
           .hottest .pic-text>li>p>a {
               display: inline-block;
               width: 20px;
               height: 27px;
               text-decoration: none;
               text-align: center;
               line-height: 27px;
               color: white;
           }
   
           .hottest .pic-text>li>p>a:nth-child(1) {
               background-color: blueviolet;
           }
   
           .hottest .pic-text>li>p>a:nth-child(2) {
               width: 208px;
           }
   
           .hottest .pic-text>li:nth-child(2)>p>a:nth-child(1) {
               background-color: sandybrown;
           }
   
           .hottest .pic-text>li:nth-child(3)>p>a:nth-child(1) {
               background-color: cadetblue;
           }
   
           .hottest .pic-text>li:nth-child(4)>p>a:nth-child(1) {
               background-color: brown;
           }
   
           .hottest .pic-text>li:nth-child(5)>p>a:nth-child(1) {
               background-color: lightgreen;
           }
           /*==============纯文本列表*/
   
           .hottest .index-text>li{
               width: 228px;
               height: 22px;
               margin-bottom: 12px;
           }
   
           .hottest .index-text>li:last-child {
               margin-bottom: 0px;
           }
   
           .hottest .index-text>li>p>span {
               width: 22px;
               height: 22px;
               background: url("imgs/img-daxue/icon-rank-item.png") no-repeat center;
               text-align: center;
               font-size: 14px;
               color: white;
               float: left;
               margin-right: 6px;
           }
   
           .hottest .index-text>li>p>a {
               width: 200px;
               height: 22px;
               float: left;
               text-decoration: none;
               color: black;
               font-size: 15px;
           }
   
   
           /*==================排行榜列表底部区域*/
   
           .gray-split-line {
               background-color: gainsboro;
               width: 228px;
               height: 1px;
               margin: 20px 0px;
           }
   
           /*==================交流*/
           .communication {
               margin-top: 28px;
           }
   
           .pic-mark{
              position: relative;
           }
   
           .pic-mark .mark{
               position: absolute;
               top: 0;
               left: 50%;
               /* 自己要移出自身的一半 */
               transform: translate(-50%,-50%);
           }
   
           .communication>p {
               margin: 10px 0px;
               font-size: 20px;
           }
   
           .communication>p:nth-of-type(2) {
               font-size: 15px;
           }
           /*==================考试联系*/
   
           .contact>h3>span:nth-child(1) {
               background: url("imgs/img-daxue/icon-phone.png");
               display: inline-block;
               width: 20px;
               height: 20px;
               margin-right: 10px;
           }
   
           .contact>h3>span:nth-child(2) {
               font-weight: 200;
               font-size: 20px;
           }
   
           .contact>p {
               font-size: 15px;
               margin: 3px 0px;
           }
   
           .contact .exam {
               width: 200px;
               height: 120px;
               background-color: gainsboro;
               margin: 26px 12px;
           }
   
           .contact .exam>span {
               width: 160px;
               height: 50px;
               display: block;
               font-size: 40px;
               margin: 0px  auto 5px auto;
   
           }
   
           .contact .exam>a {
               width: 160px;
               height: 40px;
               display: block;
               background-color: black;
               color: white;
               text-decoration: none;
               text-align: center;
               line-height: 40px;
               font-size: 24px;
               margin: 0 auto;
           }
   
   ```

   

3. ### 完整代码：

   [示例详细代码32](代码相关/demo32-dx-content-right.html)

4. ### 自练习：

   - 练习以上代码直到可以独立完成