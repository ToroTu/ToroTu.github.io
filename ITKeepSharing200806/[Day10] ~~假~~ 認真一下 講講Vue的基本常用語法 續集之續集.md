# Vue的菜鳥開發學習歷程
# [Day10] ~~假~~ 認真一下 講講Vue的基本常用語法 續集之續集
---
## 菜鳥認真講講Vue的基本常用語法 (續中續集)

好的
因為前天要加班一下
掰完“Mustache”语法
又掰太久，留剩下的到昨天
但昨天又手賤又加班了一下
只掰完"v-html"語法
好的
今天得努力下繼續生後面的兩個...

---

再補最後一次，一個component，基本上包含三個部分：
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
        Mustache標籤，也就是「{{ }}」會將包起來的區塊渲染成msg的值
    
  - 2. Raw HTML (原始HTML)
        “v-html”语法 的使用，插入Raw Html
        ```html
            <p>Using v-html directive: <span v-html="rawHtml"></span></p>
        ```
        ```javascript
            rawHtml = '<span style="color: #f00;">原始HTML</div>';
        ```
        
        將將～
        簡單吧～(笑)![/images/emoticon/emoticon38.gif](/images/emoticon/emoticon38.gif)
    
    好的～
    再繼續剩下兩個
    
  - 3. Attributes (屬性綁定、單向綁定)
        「 **v-bind** 」這方法跟 “Mustache”语法 一樣，是最常見常用的方式
        因為 “Mustache”语法 不能作用在Html的attribute上，所以 將將～ 就靠它了
        直接來個例子吧
        ```html
            <p v-bind:id="myId"></p>
        ```
        ```javascript
            myId = 'myParagraph';
        ```
        融合～～～&darr;
        ```html
            <p id="myParagraph"></p>
        ```
        簡單吧～
        來附附個畫面
        ![step 1](https://torotu.github.io/ITKeepSharing200806/img/day10/step_1.jpg)
        ![step 2](https://torotu.github.io/ITKeepSharing200806/img/day10/step_2.jpg)
        ![step 3](https://torotu.github.io/ITKeepSharing200806/img/day10/step_3.jpg)
        !!
        哎唷 有沒有看到又紅又橘的框框
        寫法不同
        但效果一樣![/images/emoticon/emoticon64.gif](/images/emoticon/emoticon64.gif)
        沒錯!!!!
        「 **v-bind:id** 」跟「 **:id** 」都是一樣做屬性綁定(單向綁定)的，
        所以「 **v-bind:&lt;attributes&gt;** 」的縮寫為「 **:&lt;attributes&gt;** 」
        
        ***!!兄台留步!!***
        以為這樣就沒了!?
        別急，魔鬼藏在細節裡
        官方文件說了
        > In the case of ***boolean attributes***, where their mere existence implies true, v-bind works a little differently. In this example:
        > ```html
        >    <button v-bind:disabled="isButtonDisabled">Button</button>
        > ```
        > If isButtonDisabled has the value of null, undefined, or false, the disabled attribute will not even be included in the rendered <button> element.
        >  
        > ***[Attributes](https://vuejs.org/v2/guide/syntax.html#Attributes)***
        
        直接上個畫面吧
        ![step 4](https://torotu.github.io/ITKeepSharing200806/img/day10/step_4.jpg)
        
  - 4. Using JavaScript Expressions (JavaScript表達式)
        來吧～
        這最後的插法，簡單來說
        Javascript的加減法，就是一種表達式
        ...!?(蛤)
        ```javascript
            var sum = 1 + 2;
        ```
        老師：「來～同學，sum是多少～」
        同學們心不甘情不願：「 3 」~~
        老師：「...」
        老師：「好棒唷 答對了～」
        對! 就是這樣
        咦!? 但我這值想在畫面顯示而已，還用一個sum變數存起來??
        將將～
        vue支援這樣的寫法，直～～接寫在「 **所有數據的綁定** 」都支持
        來個官方例子
        ```html
            {{ number + 1 }}

            {{ ok ? 'YES' : 'NO' }}

            {{ message.split('').reverse().join('') }}

            <div v-bind:id="'list-' + id"></div>
        ```
        厲害吧～
        ![step 5](https://torotu.github.io/ITKeepSharing200806/img/day10/step_5.jpg)
        ![step 6](https://torotu.github.io/ITKeepSharing200806/img/day10/step_6.jpg)
        ***!!兄台再留步!!***
        魔鬼又藏在細節裡
        官方文件又說了
        > These expressions will be evaluated as JavaScript in the data scope of the owner Vue instance. One restriction is that each binding can only contain one single expression, so the following will ***NOT work***:
        > ```html
        >    <!-- this is a statement, not an expression: -->
        >    {{ var a = 1 }}
        >
        >    <!-- flow control won't work either, use ternary expressions -->
        >    {{ if (ok) { return message } }}
        > ```

        > Template expressions are sandboxed and only have access to a whitelist of globals such as Math and Date. You should not attempt to access user defined globals in template expressions.
        > 
        > ***[Using JavaScript Expressions](https://vuejs.org/v2/guide/syntax.html#Using-JavaScript-Expressions)***
        
        上...算了
        各位自己試吧～哈
        
將將～快了時光總是過得特別快
明天再續吧～

明天續續～![/images/emoticon/emoticon69.gif](/images/emoticon/emoticon69.gif)
