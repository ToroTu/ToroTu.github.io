# Vue的菜鳥開發學習歷程
# [Day05] 來看看下Vue的開發專案&emsp;唄~
---
## 菜鳥看Vue開發專案

好的，糊裡糊塗的第05天啦
終於麻煩之一的建專案部分在昨天已經建完啦！！！開勳～
先來附上昨天最後的圖唄
![step 1](https://torotu.github.io/ITKeepSharing200806/img/day5/step_1.jpg)
不錯不錯
好的
首先來講講昨天最後留了一個massage....（ ~~痾 命案現場似的...~~ )
「如果你專案要給人家，記得先把" *node_modules* "這資料夾砍了再給，不然讓你等到天荒地老～」
對對 沒錯
丟西基咕！！！
這洗勒公啥毀？？？
![圖/翻攝自Youtube《Thru The Lens: (DAY IN THE LIFE): Episode 04 - Day in the life of Nick Young》](https://onepage.nownews.com/sites/default/files/styles/crop_thematic_content_img/public/2020-05/02_6.jpg?h=bd907a81&itok=3bFxrfhe)

(笑) 首先
我們先來看看下：
" *node_modules* "： 這個資料夾幹什麼的勒，他囤放了專案使用的套件工具，攏底加！來看看他的大小
![step 3](https://torotu.github.io/ITKeepSharing200806/img/day5/step_3.jpg)
![step 2](https://torotu.github.io/ITKeepSharing200806/img/day5/step_2.jpg)
痾...
還好還好，就
**一百多MB** ，然後 **八百多個** 檔案而已啦![/images/emoticon/emoticon10.gif](/images/emoticon/emoticon10.gif)
如果你想也把這包丟給別人，通常應該會先壓縮，然後等啊等 等啊等 再等啊等之類
然後再把這壓縮傳過去，然後等啊等 等啊等 再等啊等之類
掌聲鼓勵鼓勵&emsp; ![](https://torotu.github.io/ITKeepSharing200806/img/hand.gif?v=3)

年輕人啊

好的，像Rookie這種年幼的
當然要想方設法一下啦
不錯
好在有個棒棒的檔案，幫我們記錄這些套件碗糕的東東
將將～
#### " ***package.json*** "

WHY??為什麼這樣說勒
百聞不如一見
![step 4](https://torotu.github.io/ITKeepSharing200806/img/day5/step_4.jpg)

來來來～望向 這 "dependencies" 和這 "devDependencies" 兩個部分物件
key了你用用的套件名稱，和value了你用用的套件的版本號

將將～
只這要這秘密武器檔沒不見
來勇氣吧 砍了 " *node_modules* " 這資料夾吧
再壓縮一下剛剛專案，咻的一聲，壓完了 哈
雖然因為剛建的專案沒啥東東

好啦～
然後把這丟給對方
通常 他理應會解壓...
![/images/emoticon/emoticon38.gif](/images/emoticon/emoticon38.gif)
到了這一步，專案雖然開起來了～但不會動 哈！！
因為 套件資料夾 被你砍了啊
![/images/emoticon/emoticon38.gif](/images/emoticon/emoticon38.gif)![/images/emoticon/emoticon38.gif](/images/emoticon/emoticon38.gif)

(笑)
我們用用VSCode打開這不能動的專案
注意！是不能動不是不能用
為什麼說用VSCode打開勒
按按快捷鍵吧
***"control + `"***
咦!?
藍藍框的部分跳了出來
![step 5](https://torotu.github.io/ITKeepSharing200806/img/day5/step_5.jpg)
矮額～ 這就是連著你的 Terminal(終端機) 啦
還很ㄅㄧㄤˋㄅㄧㄤˋ的是 他一打開就是你的專案路徑耶

要是你不信，敲個pwd命令吧
```
    pwd
```
![step 6](https://torotu.github.io/ITKeepSharing200806/img/day5/step_6.jpg)
看吧～

好的
或許有人按了快捷鍵沒東西
來啦來啦
誇家誇家～
![step 7](https://torotu.github.io/ITKeepSharing200806/img/day5/step_7.jpg)
![step 8](https://torotu.github.io/ITKeepSharing200806/img/day5/step_8.jpg)
![step 9](https://torotu.github.io/ITKeepSharing200806/img/day5/step_9.jpg)
看到沒有 如果想知道快捷鍵在哪裡
切去那吧
所有的快鍵 都在那裡！

好勒好勒
回來話題～
現在該是把 **你故意** 砍～掉的東西娶(!?)回來的時候了
打下命令：
```
    npm install
```
![step 10](https://torotu.github.io/ITKeepSharing200806/img/day5/step_10.jpg)
咦!? 就這樣!?
對! 就這樣!
等吧
![step 11](https://torotu.github.io/ITKeepSharing200806/img/day5/step_11.jpg)
![step 12](https://torotu.github.io/ITKeepSharing200806/img/day5/step_12.jpg)
阿勒 裝完了!
如果裝完了 你卻和我的電腦一樣
左邊那專案結構沒有顯示出" *node_modules* "的話...
哼哼 恭喜你

和我一樣重開VSCode吧&emsp; ![](https://torotu.github.io/ITKeepSharing200806/img/hand.gif?v=3)
![step 13](https://torotu.github.io/ITKeepSharing200806/img/day5/step_13.jpg)

將將
正常了吧
試試專案能不能Run
```
    npm run serve
```
![step 14](https://torotu.github.io/ITKeepSharing200806/img/day5/step_14.jpg)
![step 15](https://torotu.github.io/ITKeepSharing200806/img/day5/step_15.jpg)
![step 16](https://torotu.github.io/ITKeepSharing200806/img/day5/step_16.jpg)

理應要開起來瘩～
哈 今天也糊裡糊塗蒙混過關啦 明天再續!! ![/images/emoticon/emoticon48.gif](/images/emoticon/emoticon48.gif)

唉唷唉唷
最後再附個大神的文章～
***[NPM Install 到底做了些什麼？node_modules 檔案結構 + 特性入門](https://ithelp.ithome.com.tw/articles/10191783)***

