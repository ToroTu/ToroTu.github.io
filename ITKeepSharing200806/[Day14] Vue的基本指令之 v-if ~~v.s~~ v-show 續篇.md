# Vue的菜鳥開發學習歷程
# [Day14] Vue的基本指令之 v-if ~~v.s~~ v-show 續篇
---
## Vue的基本指令之 v-if ~~v.s~~ v-show (續)

好的
因為昨晚熬夜不小心昏睡去勒

~~百般不願意 但還是~~
哈 丟給今天續篇

再承昨日的 **條件式渲染**
今天一定來一個跟他很像但不同品種
「 ***v-show*** 」

老樣子，再快速回顧劇情：
--- 
- Vue的基本語法1： **Interpolations(插值)**
    &emsp;&emsp;最常見用法：「 **{{ }}** 」、「 **v-bind:&lt;attributes&gt;** 」

- Vue的基本語法2： **if(判斷式)**
    「 **v-if** 」： **條件式渲染**
    &emsp;&emsp;如果條件成立，則「插入」元素；如果不成立，則「移除」元素
    &emsp;&emsp;對DOM做「 ***append*** 或 ***remove*** 」
    延伸：
    &emsp;&emsp;搭配「 **v-else** 」或「 **v-if-else** 」

&emsp;
很好! 快速回顧
然後
快速進正題!!

- Vue的基本語法3： **show(顯不顯示)**
    「 **v-show** 」： **條件式渲染**
    &emsp;
    蛤!?!? 條件式渲染... PART 2!?
    &emsp;
    &emsp;
    聽講完話啊 孩子
    &emsp;
    來人! 上例!
    ```html
        <p v-show="isShow">聽講完話啊 孩子</p>
    ```
    ```javascript
        var isShow = true;
    ```
    ![step 1](https://torotu.github.io/ITKeepSharing200806/img/day14/step_1.jpg)
    ![step 2](https://torotu.github.io/ITKeepSharing200806/img/day14/step_2.jpg)
    來來來
    我 v-show 一個綁「isShow」，一個綁「!isShow」
    所以對 v-show 而言
    一個顯示(true)
    一個不顯示(false)
    
    &emsp;
    現在! 來品味一下
    重點「 不顯示(false) 」那個，也就是「 **v-show="!isShow"** 」
    他雖然畫面上看不到
    但在DOM上
    **他是存在的**
    
    **他．是．存．在．的**
    
    ~~哎唷，我的媽呀~~
    他用了「 **CSS** 」的「 **display屬性** 」
    遮你的雙眼啊!! 哎唷威呀
    
    &emsp;
    沒感覺?
    反一個!
    ![step 3](https://torotu.github.io/ITKeepSharing200806/img/day14/step_3.jpg)
    ![step 4](https://torotu.github.io/ITKeepSharing200806/img/day14/step_4.jpg)
    看吧～
    認清現實吧! 對CSS不了解的請稍稍google一下吧
    
    好的，附個官方語錄：
    > Another option for conditionally displaying an element is the v-show directive. The usage is largely the same:
    >  ```html
    >    <h1 v-show="ok">Hello!</h1>
    >  ```
    > The difference is that an element with v-show will always be rendered and remain in the DOM; v-show only toggles the display CSS property of the element.
    > 
    > ***[v-show](https://vuejs.org/v2/guide/conditional.html#v-show)***
    
    &emsp;
    好! 初始化!
    「 **v-show** 」： **條件式渲染**
    &emsp;&emsp;如果條件成立，則對元素「移除」style「 **display: none;**」；如果不成立，則對元素「插入」style「 **display: none;**」
    
    &emsp;
    看出端倪了嗎??
    來來，在上一個官方語錄：
    > v-if is “real” conditional rendering because it ensures that event listeners and child components inside the conditional block are properly destroyed and re-created during toggles.
    > 
    > v-if is also lazy: if the condition is false on initial render, it will not do anything - the conditional block won’t be rendered until the condition becomes true for the first time.
    > 
    > In comparison, v-show is much simpler - the element is always rendered regardless of initial condition, with CSS-based toggling.
    > Generally speaking, v-if has higher toggle costs while v-show has higher initial render costs. So prefer v-show if you need to toggle something very often, and prefer v-if if the condition is unlikely to change at runtime.
    > 
    > ***[v-if vs v-show](https://vuejs.org/v2/guide/conditional.html#v-if-vs-v-show)***

    &emsp;
    「 v-if 」： 是真正的 **條件式渲染** ，因為會確實的做「重建」和「銷毀」
    「 v-show 」： 是擬似的 **條件式渲染** ，一直存在畫面，利用「CSS」做「遮不遮你眼」
    
    所以
    一般來說
    有著~~音速般的~~ **頻繁** 切換，使用「 v-show 」會比較好
    有著~~關鍵十個~~ **條件少變化** ，使用「 v-if 」會比較好
    
    雖然應該還是視狀況決定啦～
    哈
    好的～
    補回昨天面子了
    明天再續吧～掰&emsp;![/images/emoticon/emoticon29.gif](/images/emoticon/emoticon29.gif)
