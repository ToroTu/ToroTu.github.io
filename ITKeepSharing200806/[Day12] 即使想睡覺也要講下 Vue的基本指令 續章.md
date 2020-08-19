# Vue的菜鳥開發學習歷程
# [Day12] 即使想睡覺也要講下 Vue的基本指令 續章
---
## 菜鳥想睡中也要講下 Vue的基本指令 Part.2

好的
因為昨天熬夜太晚 雖然現在也在熬夜寫這續篇...
接昨天和這幾天講

--- 
- Vue的基本語法1： **Interpolations(插值)**
      最常見用法：
      - 1. “Mustache”语法 (双大括号) ，「 **{{ }}** 」
      - 2. 屬性綁定、單向綁定，「 **v-bind:&lt;attributes&gt;** 」

- Vue的基本語法2： **if(判斷式)**
    
    --- 
    P.S:
    「 **v-** 」是一種指令(Directives)
    > Directive attribute values are expected to be a single JavaScript expression (with the exception of v-for, which will be discussed later).
    指令職責：
    - 1. 單一javascript表達式
    - 2. 當表達式的值改變時，響應式地作用於DOM
    --- 
    
    「 **v-if** 」：
        **條件式渲染**
        如果條件成立，則「插入」元素；如果不成立，則「移除」元素
        !? !?
        對! 發現沒有
        他是對DOM做「 ***append*** 或 ***remove*** 」
    好的，久違的畫面來下
    ```html
        <p v-if="seen">笑 還笑</p>
        <p v-if="!seen">消失給你看看</p>
    ```
    ```javascript
        seen = true;
    ```
    ***[Conditional Rendering](https://vuejs.org/v2/guide/conditional.html)***
    因為之前喇太多廢話，佔版，所以之前的我先移除
    ![step 1]()
    ![step 2]()
    ![step 3]()
    ![step 4]()
    好的～我們發現了一件事
    上圖，「 v-if 」移除元素的位置，他會用「 **&lt;!----&gt;** 」做標記

    好的～
    延伸延伸～
    我想要「 **v-if** 」單一判斷成立與否
    若否，則顯示
    恩～這功能不錯!
    當然有呀
    「 **v-else** 」!!
    來來～之接上畫面囉
    ![step 5]()
    ![step 6]()
    
       
將將～累了...
明天再續吧～

明天續續～![/images/emoticon/emoticon69.gif](/images/emoticon/emoticon69.gif)
