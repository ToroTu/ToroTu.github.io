# Vue的菜鳥開發學習歷程
# [Day01] ~~菜鳥裝Ｂ之路~~...序章
---
## 前情提要
#### Vue.js，三大前端框架之一，在沈迷於javascript的美妙之下，前進前端開發之路...
查找網路上資料，大都是以引用CDN方式的教學說明，專案開發的教學說明等等文件，看得愈來愈是烏煞煞...坎坷啊
但身為菜鳥想要裝Ｂ下，這點挑戰還是要有的![/images/emoticon/emoticon38.gif](/images/emoticon/emoticon38.gif)![/images/emoticon/emoticon38.gif](/images/emoticon/emoticon38.gif)![/images/emoticon/emoticon38.gif](/images/emoticon/emoticon38.gif)...著裝！祈禱！前進吧...
- 裝B之路：
    - 1. vue component
    - 2. vue-router
    - 3. vuex
- 裝B裝備：
    - 1. scss
    - 2. typescript
    - ...買得起的話

## 初體驗...序章![](https://torotu.github.io/ITKeepSharing200806/img/hand.gif?v=3)

首先~~為了湊合湊合字數~~，還是先來提提Vue.js這frontend framework，根據官方說法：

> ### Vue.js 是什么
> Vue (读音 /vjuː/，类似于 view) 是一套用于构建用户界面的渐进式框架。与其它大型框架不同的是，Vue 被设计为可以自底向上逐层应用。Vue 的核心库只关注视图层，不仅易于上手，还便于与第三方库或既有项目整合。另一方面，当与现代化的工具链以及各种支持类库结合使用时，Vue 也完全能够为复杂的单页应用提供驱动。
> 
> *[vue.js.org](https://cn.vuejs.org/v2/guide/index.html)*

如此文言，~~看來我該去補補文科了(笑)~~，需要再更直白解釋的請再問問google大神吧！Rookie的我，一番腦內小劇場後，得到的翻譯：
用傳統的做法對html做處理，如要對parent element加入數個children element，像是div、li之類的，需要使用javascript或者jquery，執行類似以下做法：
```javascript
   // --- parent element ---
   // Version javascript
   // var $pe = document.querySelector('#parent-element');
   // Version jquery
   var $pe = $('#parent-element');
   
   // --- add children element ---
   // Version javascript
   // var $ce = document.createElement('div');
   // $ce.className = 'child-element';
   // $pe.append($ce);
   // Version jquery
   var $ce = $('<div class="child-element"></div>');
   $pe.append($ce);
```

...所以，為了養精蓄銳，明天再續...![](https://torotu.github.io/ITKeepSharing200806/img/hand.gif?v=3)



