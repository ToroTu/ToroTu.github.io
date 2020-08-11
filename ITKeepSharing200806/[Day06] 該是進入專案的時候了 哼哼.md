# Vue的菜鳥開發學習歷程
# [Day06] 該是進入專案的時候了 哼哼
---
## 菜鳥進入Vue開發專案

看來該是進入專案的時候了
不然被斷頭就糟了(!?)

來來來 先附個專案開啟圖唄
![step 1](https://torotu.github.io/ITKeepSharing200806/img/day6/step_1.jpg?v=34)
不錯不錯

再來做一下前置作業吧(!?又來!?)
不急不急
幫你好開發咩
望向VSCode的左邊Sidebar(側邊欄)
按下倒數第二個那個icon，那是Extensions(擴充套件)
擴展你的VSCode工具

好的
我啦 我在寫Vue前會來裝裝下「 *Vetur* 」這個套件
幫助你快速開發不好嗎
![step 2](https://torotu.github.io/ITKeepSharing200806/img/day6/step_2.jpg?v=34)

下一個我是沒裝啦，我Rookie咩～
不過有的大神推薦
「 *Vue 2 Snippets* 」
快快速開發你的專案(!?)
![step 3](https://torotu.github.io/ITKeepSharing200806/img/day6/step_3.jpg?v=34)

來來 再下一個想裝的裝唄～
它可以讓你的專案結構美美的
「 *vscode-icons* 」
![step 4](https://torotu.github.io/ITKeepSharing200806/img/day6/step_4.jpg?v=34)
其他想聞想試的 去找找google大神吧～開開你的瀏覽器

好的 回來專案吧
廢話少說
展開那個「 ***src*** 」的資料夾
這個資料夾是我們現在最要關注的，因為我們的code攏底加
![step 5](https://torotu.github.io/ITKeepSharing200806/img/day6/step_5.jpg?v=34)

快速介紹～
- assets： 
    資源檔，現階段就在底下建個「 ***img*** 」的資料夾吧
    放你的圖片 ( ~不是D槽~ )
![step 6](https://torotu.github.io/ITKeepSharing200806/img/day6/step_6.jpg?v=34)
- components：
    Vue Component(元件)，我們之後切的component都放在這
- router：
    我們第04天不是建專案嗎，不是有個預裝工具選項
    這就是當你選那個 *Router* 選項他就幫你建出這資料夾來
- store：
    一樣的～～
    我們第04天選的 *Vuex* ～
- views：
    頁面的主檔，我們的 *router(路由)* 會導向這資料夾裡的檔案
    然後這裡面的檔案會再去 import(導入) 他想要的 component
- App.vue：
    這檔案...簡單來說
    你的 *main component(主元件)*
- main.js：
    承上選項
    這main.js是你的主進入點!!
    src同層的資料夾不是有個叫「public」的傢伙嗎
    裡面的「index.html」打～開來
    會看到有個「 id="app" 」的 "&lt;div&gt;"tag
![step 7](https://torotu.github.io/ITKeepSharing200806/img/day6/step_7.jpg?v=34)
    main.js會把你的 *main component(主元件)*
    注入取代他
![step 8](https://torotu.github.io/ITKeepSharing200806/img/day6/step_8.jpg?v=324)
    你的Vue～專案從此刻開啟啦～

好的～
看來今天可以收工啦![/images/emoticon/emoticon39.gif](/images/emoticon/emoticon39.gif)
哀...打到一半 手殘滑到重整...
又重打一次...
明天再認真點好了～![/images/emoticon/emoticon69.gif](/images/emoticon/emoticon69.gif)