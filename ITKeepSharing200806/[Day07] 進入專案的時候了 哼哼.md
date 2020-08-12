# Vue的菜鳥開發學習歷程
# [Day06] 進入專案的時候了 哼哼
---
## 菜鳥進入Vue開發專案 (續)

先再附上專案結構圖
![step 1](https://torotu.github.io/ITKeepSharing200806/img/day7/step_1.jpg)
多看幾次，對專案的感覺度就愈來愈高
我是這樣啦(笑)

昨天提到「 ***main.js*** 」這隻程式碼會是你專案的起始點
根據官網敘述：
> ### vue serve
> *vue serve uses the same default setup (webpack, babel, postcss & eslint) as projects created by vue create. It automatically infers the entry file in the current directory - the entry can be one of main.js, index.js, App.vue or app.vue. You can also explicitly specify the entry file.*
> 
> *[Instant Prototyping](https://cli.vuejs.org/zh/guide/prototyping.html)

我們的專案進入口預設是叫main.js
你也可以改成index.js
但我不要～

首先我們先來看看main.js裡面做了什麼吧
main.js這邊我們看
他主要做了4件事情
- import： 引入所需的模組
  *[完全解析 JavaScript import、export](https://wcc723.github.io/development/2020/03/25/import-export/)*
  這裡我們引入了：
  - Vue： vue物件
  - App： App.vue這個component
  - router： vue-router物件
  - store： Vuex物件
- Vue.config： *[vue的全局配置](https://vuejs.org/v2/api/#productionTip)*
- new Vue()： 創建Vue的instance(實例)，渲染App component，並router、store注入進instance
  *[渲染函数 & JSX](https://vuejs.org/v2/guide/render-function.html)*
  *[插件](https://vuejs.org/v2/guide/plugins.html)*
  *[Vuex](https://vuex.vuejs.org/guide/)*
- $mount()： 如果在new Vue()創建instance的時候，沒有傳入el的參數，那這個instance就還尚未跟DOM綁定，處於「 ***unmounted (未挂载)*** 」的狀態
  哼哼～你以為沒機會掛載了嗎？ No No，我們可以用$mount()來手動式掛載他～
  *[vm.$mount( [elementOrSelector] )](https://vuejs.org/v2/api/#vm-mount)*
  > 秀一下官方示例：
  > ```
  >  var MyComponent = Vue.extend({
  >      template: '<div>Hello!</div>'
  >  })
  >
  >  // 创建并挂载到 #app (会替换 #app)
  >  new MyComponent().$mount('#app')
  >
  >  // 同上
  >  new MyComponent({ el: '#app' })
  >
  >  // 或者，在文档之外渲染并且随后挂载
  >  var component = new MyComponent().$mount()
  >  document.getElementById('app').appendChild(component.$el)
  > ```
  > 
  這裡我們是去掛載位於專案的public資料夾裡的index.html名為 ~~信念的旗幟下~~ ，啊不是 是id="app"的元素
![step 2](https://torotu.github.io/ITKeepSharing200806/img/day7/step_2.jpg)

好的 ~~看來今天可以先收工下了~~
如何來驗證$mount掛載在public資料夾裡的index.html的id="app"的元素勒
來幹嚇傻事
我們 npm run serve 起專案後
瀏覽器打開「開發者工具(option+command+i)」
![step 3](https://torotu.github.io/ITKeepSharing200806/img/day7/step_3.jpg)
我們看看Element的地方有個「&lt;div id="app"&gt;」的tag
將將～這就是對應我們public資料夾裡的index.html的id="app"的元素啦～
．
．
．
錯！ 正確來說是 public資料夾裡的index.html的id="app"的元素 **被** 渲染成 App.vue這個component了

我們做個傻事
將App.vue的template「id="app"」改成「id="app1"」
![step 4](https://torotu.github.io/ITKeepSharing200806/img/day7/step_4.jpg)
來來來 存檔!!!!
見見他的變化
![step 5](https://torotu.github.io/ITKeepSharing200806/img/day7/step_5.jpg)



看來今天可以收工啦![/images/emoticon/emoticon39.gif](/images/emoticon/emoticon39.gif)
明天再再認真好了～![/images/emoticon/emoticon69.gif](/images/emoticon/emoticon69.gif)