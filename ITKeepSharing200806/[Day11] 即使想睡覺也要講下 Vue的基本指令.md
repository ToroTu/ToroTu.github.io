# Vue的菜鳥開發學習歷程
# [Day11] 即使想睡覺也要講下 Vue的基本指令
---
## 菜鳥想睡中也要講下 Vue的基本指令

好的
因為昨天和前幾天
掰完Vue的插(值)法和效果
來回顧下吧：

--- 
- Vue的基本語法1： **Interpolations(插值)**
  - 1. Text (文本)
        “Mustache”语法 (双大括号) ，「 **{{ }}** 」，最常見簡單的作法
  - 2. Raw HTML (原始HTML)
        “v-html”语法 的使用，「 **v-html** 」，插入Raw Html
  - 3. Attributes (屬性綁定、單向綁定)
        「 **v-bind** 」這方法跟 “Mustache”语法 一樣，是最常見常用的方式
        「 **v-bind:&lt;attributes&gt;** 」的縮寫為「 **:&lt;attributes&gt;** 」
  - 4. Using JavaScript Expressions (JavaScript表達式)
        使用Javascript的表達式，支持「 **所有數據的綁定** 」
--- 

好的，因為愛睏中
快速講講
- Vue的基本語法2： **if(判斷式)**
    再講判斷之前，有個疑問?
    有沒有覺得，阿勒「 v-html 」、「 v-bind 」，為啥前面要有個「 **v** 」?我是要裝Ｂ又不是要演超人
    哼哼
    ~~賊哩丟Ｕ縮噗低啦～~~
    「 **v-** 」這是一種 ~~口令~~，阿不是...是 指令(Directives)!
    來看看下官方解釋：
    > Directives are special attributes with the v- prefix. Directive attribute values are expected to be a single JavaScript expression (with the exception of v-for, which will be discussed later). A directive’s job is to reactively apply side effects to the DOM when the value of its expression changes. Let’s review the example we saw in the introduction:
    > ```html
    >    <p v-if="seen">Now you see me</p>
    > ```
    > Here, the v-if directive would remove/insert the <p> element based on the truthiness of the value of the expression seen.
    > 
    > **[Directives](https://vuejs.org/v2/guide/syntax.html#Directives)**
            
將將～快了時光總是過得特別快
明天再續吧～

明天續續～![/images/emoticon/emoticon69.gif](/images/emoticon/emoticon69.gif)
