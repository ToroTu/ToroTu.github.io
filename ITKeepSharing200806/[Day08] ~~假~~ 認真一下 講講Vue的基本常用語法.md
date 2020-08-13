# Vue的菜鳥開發學習歷程
# [Day08] ~~假~~ 認真一下 講講Vue的基本常用語法
---
## 菜鳥認真講講Vue的基本常用語法

好的
來花個兩天假認真講講常用的Vue的語法吧
不過可能先來講講Vue的Component唄
好的
我們的專案開啟路由是 **http:&frasl;&frasl;localhost:8080&frasl;**
![step 1](https://torotu.github.io/ITKeepSharing200806/img/day8/step_1.jpg)
「 localhost 」是我們的ip位置，本機開發相當於127.0.0.1
「 :8080 」是ip位置開放出來的port，這個我們每次 npm run serve 可能會變不一樣
有興趣的自行去了解了解吧
我們著重的是後面的「 / 」
「 / 」這是我們路由設置要注意的部分，依不同的路由配置去取不同的component
路由部分後續再講講～
今天先直接跳這「 / 」路由對應的component，位在「 **/src/views/** 」下的「 **Home.vue** 」
打開來～
![step 2](https://torotu.github.io/ITKeepSharing200806/img/day8/step_2.jpg)
我們看看下結構
```
<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Home',
  components: {
    HelloWorld
  }
}
</script>
```
一個component，基本上包含三個部分：
- &lt;template&gt;： Html樣板
- &lt;script&gt;： JavaScript的部分，Vue的程式碼
- &lt;style&gt;： CSS樣式的部分
好的～
這個Home.vue component偷懶沒style(笑) 我們先不理吧～
我們用用這template和script寫點基本語法 ~~佔佔版面~~

先拿template開刀
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
    Mustache標籤，也就是「{{ }}」會將包起來的區塊渲染成msg的值，也就是「我是Rookie」
    ![step 3](https://torotu.github.io/ITKeepSharing200806/img/day8/step_3.jpg)
    然後這時候你只要更改msg的值... 他就渲染成那個新的值耶!!!! 你看 你完全不用理會他怎麼渲染到DOM上面的
    ![step 4](https://torotu.github.io/ITKeepSharing200806/img/day8/step_4.jpg)
    如果是傳統javascript的寫法
    可能會變成
    ```html
        <span>Message: </span>
    ```
    ```javascript
        var span = document.querySelector('span');
        var text = span.innerText;
        span.innerText = text + msg;
    ```
    還得留意如果多個span的話，還得加class或id之類做區分
    他既有的內容又要暫存起來...等等
    事情多吧

    再看看Vue的兩個括括...簡單明瞭
  - 2. Raw HTML (原始HTML)
  - 3. Attributes (屬性綁定、單向綁定)
  - 4. Using JavaScript Expressions (JavaScript表達式)

恩～～～依時間關係，2、3、4點明天再續吧
要先去加班了(暈..)

明天續續～![/images/emoticon/emoticon69.gif](/images/emoticon/emoticon69.gif)
