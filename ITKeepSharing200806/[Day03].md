# Vue的菜鳥開發學習歷程
# [Day03] 將將~Vue的開發安裝
---
## 菜鳥的Vue安裝

將將～該來假認真一下了，不然被砍頭就不妙了哩![/images/emoticon/emoticon04.gif](/images/emoticon/emoticon04.gif)
好瘩！直接進入主題，今天來先安裝一下環境，本Rookie因為想裝Ｂ下，所以使用環境... **MacOS Catalina 10.15** ～
使用Windows環境的... 以後想到再放吧((笑

### Rookie環境：
- 1. 作業環境： MacOS Catalina 10.15
- 2. 編輯器： Visual Studio Code
- 3. 框架環境：
    - (1) nvm： 0.32.1，Node.js的版本管理器(version manager)
    - (2) npm： 6.13.7
    - (3) node： v13.10.1
        p.s： nvm、npm不多講了，網上很多安裝教學。哈，但還是附下參考連結好勒
        *[nvm：安裝、切換不同 Node.js 版本的管理器](https://titangene.github.io/article/nvm.html)*
        ![](https://torotu.github.io/ITKeepSharing200806/img/npm-ico.png) *[從零開始: 使用NPM套件](https://medium.com/html-test/%E5%BE%9E%E9%9B%B6%E9%96%8B%E5%A7%8B-%E4%BD%BF%E7%94%A8npm%E5%A5%97%E4%BB%B6-317beefdf182)*
    - (3) vue-cli： @vue/cli 4.2.3，基于Vue.js进行快速开发的標準開發工具 *[Vue CLI官網](https://cli.vuejs.org/)*

### 啟程囉
首先...沒裝npm的請自行先裝下吧(笑XD)
將將～ 來安裝vue-cli囉，打開terminal，輸入安裝命令：
```
    npm install -g @vue/cli
```
噗噗～在此之前，請容Rookie的我先生個新環境
將將～使用parallels desktop新一個Catalina 等待安裝完成中...
![/images/emoticon/emoticon28.gif](/images/emoticon/emoticon28.gif)
![/images/emoticon/emoticon28.gif](/images/emoticon/emoticon28.gif)
![/images/emoticon/emoticon28.gif](/images/emoticon/emoticon28.gif)
．
．
．
啊哈～生出來啦&emsp;![](https://torotu.github.io/ITKeepSharing200806/img/hand.gif?v=3)

Rookie的小劇場下集，得到的翻譯：
上集小劇場，用傳統的做法對html做處理，如要對parent element加入數個children element，像是div、li之類的，需要使用javascript或者jquery，沒錯～這類的做法需要動態對DOM做操作，當大量操作~~ＣＲＵＤ(!?)~~
的時候，效能影響就極為嚴重了勒，更何況還有事件綁定、樣式綁定等等之類的，用jquery來寫還算勉勉強強，javascript...歐～

將將～這時候想破頭腦不如來放鬆下試試framework，來View一下唄![/images/emoticon/emoticon37.gif](/images/emoticon/emoticon37.gif)

用Rookie的話語來說，Vue幫我們處理了畫面的所有事情
新增元件，自己來&emsp;不用！
綁定事件，自己來&emsp;不用！
刪除元件，自己來&emsp;不用！
...，自己來&emsp;不用！
![](https://torotu.github.io/ITKeepSharing200806/img/what.png)
那還要自己幹嘛？？

誒～當然還要咩
你總要給他資料吧，要給他畫面格局吧

所以我們事先定好 ***模板(Component)*** 後
只要跟他講好，給你什麼資料的時候，你去用什麼模板畫出來給我看看
將將～咻的一下畫面就出來了
你只要專心處理你的邏輯就好啦～

像是 ~~D槽下的秘...~~ 規則之類的

哼哼，好像差不多佔完版面了
看來明天得認真寫點專業裝Ｂ了

前進Vue吧！Rookie！

最後給個Vue官網最重要的圖裝Ｂ下![/images/emoticon/emoticon75.gif](/images/emoticon/emoticon75.gif)
![](https://cn.vuejs.org/images/lifecycle.png)