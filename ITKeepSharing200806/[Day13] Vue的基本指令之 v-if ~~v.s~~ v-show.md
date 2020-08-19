# Vue的菜鳥開發學習歷程
# [Day13] Vue的基本指令之 v-if ~~v.s~~ v-show
---
## Vue的基本指令之 v-if ~~v.s~~ v-show

好的
因為加班熬夜加班熬夜 雖然現在也在熬夜...
承昨日的 **條件式渲染**
今天來一個跟他很像但不同品種
「 ***v-show*** 」

老樣子，回顧劇情：
--- 
- Vue的基本語法1： **Interpolations(插值)**
      最常見用法：
      - 1. “Mustache”语法 (双大括号) ，「 **{{ }}** 」
      - 2. 屬性綁定、單向綁定，「 **v-bind:&lt;attributes&gt;** 」

- Vue的基本語法2： **if(判斷式)**
    「 **v-if** 」： **條件式渲染**
    &emsp;&emsp;如果條件成立，則「插入」元素；如果不成立，則「移除」元素
    &emsp;&emsp;對DOM做「 ***append*** 或 ***remove*** 」
    
    &emsp;

    來來～
    「 **v-if** 」的延伸：搭配「 **v-else** 」
    好的~
    「 **v-if** 」還有一個延伸，那就是...將將
    「 **v-else-if** 」當如果有3種以上，可以用用

    不錯吧! 光一個判斷式就有這些玩法
    但...
    我因應我公司規則，
    盡量只用 「 **v-if** ]
    ![/images/emoticon/emoticon06.gif](/images/emoticon/emoticon06.gif)
    哼哼
    為什麼勒～

    &emsp;

    假設你有
    100行的內容放在「 v-if 」
    然後再一個100行內容放在 「 v-else 」
    ...
    ![/images/emoticon/emoticon04.gif](/images/emoticon/emoticon04.gif)
    我的螢幕不夠長啊!!!!!
    要滑啊滑才比較好找到 **v-if** 和 **v-else** 的分隔點在哪
    難找啊～
    所以～
    
    &emsp;

    &emsp;

    如果要用到 v-else 的時候
    我們可以改成「 **!&lt;veriable&gt;** 」
    如下～
    ```html
        <p v-if="isSeen">笑 還笑</p>
        <p v-if="!isSeen">消失給你看看</p>
    ```
    同理～!!
    「 **v-else-if** 」請舉一反三吧
    
好的～
快快進入正題
但...
~~因為眼皮要撐不住了~~

&emsp;

將將～累了...
明天再續吧～

明天續續～![/images/emoticon/emoticon69.gif](/images/emoticon/emoticon69.gif)
