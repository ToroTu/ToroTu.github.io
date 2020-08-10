# Vue的菜鳥開發學習歷程
# [Day04] 來建一下~Vue的開發專案&emsp;唄~
---
## 菜鳥建Vue開發專案

哼哼，先來附上幾個專業的連結
- ***[Vue-cli 基礎教學](https://medium.com/%E4%BC%81%E9%B5%9D%E4%B9%9F%E6%87%82%E7%A8%8B%E5%BC%8F%E8%A8%AD%E8%A8%88/vue-cli-%E5%9F%BA%E7%A4%8E%E6%95%99%E5%AD%B8-836e397bc432)***
- ***[Vue CLI3 安裝與建立 vue 專案](https://ithelp.ithome.com.tw/articles/10216606)***
- ***[Vue-CLI 官網 创建一个项目](https://cli.vuejs.org/zh/guide/creating-a-project.html#vue-create)***

今天來看&#8593;&#8593;&#8593;大神們的文章裝Ｂ一下![/images/emoticon/emoticon74.gif](/images/emoticon/emoticon74.gif)
- Step 1： 再次打開我完美的虛擬環境＋打開我完美的terminal(終端機)
    ![step 1](https://torotu.github.io/ITKeepSharing200806/img/day4/step_1.jpg)
    &#9650; 再次瞧瞧我完美的虛擬環境＋打開我完美的terminal(終端機)
- Step 2： 打上建立專案命令，來起一個專案名吧，按下你的Enter然後...敬請期待
    ```
        vue create plan-b
    ```
    ![step 2.1](https://torotu.github.io/ITKeepSharing200806/img/day4/step_2_1.jpg)
    
    !!等等!!
    
    專案不要隨便建
    等等找不到
    建之前先跳到你想要的資料夾下唄
    為了方便，菜鳥的我就建在桌面下吧 哈哈哈
    ```
        cd Desktop
    ```
    ![step 2.2](https://torotu.github.io/ITKeepSharing200806/img/day4/step_2_2.jpg)
- Step 3： 我們跟著大神們的腳步，手動自己想要的設定吧：
    - (1) 選擇 Manually select feactures (手動選擇設定，以下操作 空白鍵：選擇、Enter：確定、上下鍵)
    ![step 3.1](https://torotu.github.io/ITKeepSharing200806/img/day4/step_3_1.jpg)
    ![step 3.2](https://torotu.github.io/ITKeepSharing200806/img/day4/step_3_2.jpg)
    - (2) 選擇安裝工具，這裡我選擇大神選的：
        - (a) Babel： 翻譯ES6語法，因為有些瀏覽器版本尚未支援ES6
        - (b) Router： vue-router 路由器，設定前端路由，幫像我這樣的菜鳥操作window.history(笑)
        - (c) Vuex： 狀態管理秘密武器(笑)
        - (d) CSS Pre-processors： CSS預處理器，如果你想「不要，我就要純寫CSS!!!」拜託，別裝～ Rookie的我要來寫寫SCSS勒～
        - (e) Linter/Formatter： 幫你檢查代碼正確的擾人工具...
        p.s： 
            TypeScript以後有時間再建一個專案吧 現在先用Javascript就好～
            剩下幾個選項以後再看看吧
    ![step 3.3](https://torotu.github.io/ITKeepSharing200806/img/day4/step_3_3.jpg)
    ![step 3.4](https://torotu.github.io/ITKeepSharing200806/img/day4/step_3_4.jpg)
    - (3) 哎唷，接下來是Router模式
            模式有兩種： history模式、hash模式(默認) *[附個連結吧](https://router.vuejs.org/guide/essentials/history-mode.html)*
          這裡我們跟著大神的腳步
    ![step 3.5](https://torotu.github.io/ITKeepSharing200806/img/day4/step_3_5.jpg)
    - (4) CSS pre-processer： 我們也選擇Sass/SCSS(with dart-sass)吧(笑)
    ![step 3.6](https://torotu.github.io/ITKeepSharing200806/img/day4/step_3_6.jpg)
    - (5) ESLint： 哼哼，我們要來個統一、再來個嚴謹(笑...之後很刺激噠)
    ![step 3.7](https://torotu.github.io/ITKeepSharing200806/img/day4/step_3_7.jpg)
    - (6) ESLint檢查時機： 保存時就檢查
    ![step 3.8](https://torotu.github.io/ITKeepSharing200806/img/day4/step_3_8.jpg)
    - (7) 你想在哪配置各個工具配置：分開分開，我視力不好，一起好雜啊
    ![step 3.9](https://torotu.github.io/ITKeepSharing200806/img/day4/step_3_9.jpg)
    - (8) 最後了最後了，是否保存剛剛點的那些東西，不要存啦! 下次再玩點一次吧!!
    ![step 3.10](https://torotu.github.io/ITKeepSharing200806/img/day4/step_3_10.jpg)
    - (9) 哈哈，終於開始建了! 等他吧
    ![step 3.11](https://torotu.github.io/ITKeepSharing200806/img/day4/step_3_11.jpg)
    ![step 3.12](https://torotu.github.io/ITKeepSharing200806/img/day4/step_3_12.jpg)
    ![step 3.13](https://torotu.github.io/ITKeepSharing200806/img/day4/step_3_13.jpg)
    - (10) 哎唷威呀，終於建完了，快吧(!?) 想看看專案是否可以用，再打打指令吧
        ```
            cd plan-b
        ```
        ```
            npm run serve
        ```
    ![step 3.14](https://torotu.github.io/ITKeepSharing200806/img/day4/step_3_14.jpg)
    ![step 3.15](https://torotu.github.io/ITKeepSharing200806/img/day4/step_3_15.jpg)
    - (11) 然後複製下，去瀏覽器打開那網址，出現下面畫面代表成功囉！
    ![step 3.16](https://torotu.github.io/ITKeepSharing200806/img/day4/step_3_16.jpg)
    ![step 3.17](https://torotu.github.io/ITKeepSharing200806/img/day4/step_3_17.jpg)
    - (12) 好啦，等這麼多都快睡著了，我們用VSCode開開專案養眼下吧，但我完美的虛擬機暫時功成身退啦～所以我用回我MacOS環境開開～
           啊啊～順便耍Ｂ一下，如果你專案要給人家，記得先把" *node_modules* "這資料夾砍了再給，不然讓你等到天荒地老～
    ![step 3.18](https://torotu.github.io/ITKeepSharing200806/img/day4/step_3_18.jpg)
           

好瘩～今天也糊裡糊塗蒙混過關啦 明天再續!! ![/images/emoticon/emoticon48.gif](/images/emoticon/emoticon48.gif)

