# Vue的菜鳥開發學習歷程
# [Day09] ~~假~~ 認真一下 講講Vue的基本常用語法 續集
---
## 菜鳥認真講講Vue的基本常用語法 (續集)

好的
昨天因為要加班一下
又打得不夠快速，所以停留在“Mustache”语法掰完
好的
今天來繼續後面的三個

再補一次，一個component，基本上包含三個部分：
- &lt;template&gt;： Html樣板
- &lt;script&gt;： JavaScript的部分，Vue的程式碼
- &lt;style&gt;： CSS樣式的部分
好的～

- Vue的基本語法1： **[Interpolations(插值)](https://vuejs.org/v2/guide/syntax.html#Interpolations)** ，作數據綁定
  不同的插法不同的效果(笑)：
  - 1. Text (文本)
    “Mustache”语法 (双大括号) ，「 **{{ }}** 」，最常見簡單的作法
    ```html
        <span>Message: {{ msg }}</span>
    ```
    以上述程式為例，如果我在 javascript 部分有一個 **msg** 的變數
    ```javascript
        msg = '我是Rookie';
    ```
    Mustache標籤，也就是「{{ }}」會將包起來的區塊渲染成msg的值，也就是「我是Rookie」...
    
好的～到這邊是昨天的份，再提一下
開始今天的份～

  - 2. Raw HTML (原始HTML)
    “Mustache”语法 (双大括号)的使用，會將數據視為單純的文本，我把他視意為傳統javascript的「 **innerText** 」，不知道的人自己去看看吧～ **[HTMLElement.innerText
](https://developer.mozilla.org/en-US/docs/Web/API/HTMLElement/innerText)**
    那...
    如果今天我就想要插一個Raw Html勒
    插一個
    ```html
        <div style="color: #f00;">我菜～</div>
    ```
    勒
    ![/images/emoticon/emoticon19.gif](/images/emoticon/emoticon19.gif)
    傳統的javascript只能插文本嗎? 哼 怎麼可能這麼簡單
    將將～「 **innerHTML** 」能辦到! 想嵌Raw Html，找他就對了 **[Element.innerHTML](https://developer.mozilla.org/en-US/docs/Web/API/Element/innerHTML)**
    既然傳統就有
    新一代當然要繼承意志了
    「 **v-html** 」直接來使用下吧
    ```html
        <p>Using v-html directive: <span v-html="rawHtml"></span></p>
    ```
    ```javascript
        rawHtml = '<span style="color: #f00;">原始HTML</div>';
    ```
    ![step 1](https://torotu.github.io/ITKeepSharing200806/img/day9/step_1.jpg)
    簡單吧～(笑)
    好啦 v-html 還有一些細節，請看看 ***[官網文件.vue](https://vuejs.org/v2/guide/syntax.html#Raw-HTML)***
    
    好的～今天時間上有點趕...
    哈明天再繼續下兩個
    
  - 3. Attributes (屬性綁定、單向綁定)
  - 4. Using JavaScript Expressions (JavaScript表達式)

恩～～～依時間關係，2、3、4點明天再續吧
要先去加班了(暈..)

明天續續～![/images/emoticon/emoticon69.gif](/images/emoticon/emoticon69.gif)
