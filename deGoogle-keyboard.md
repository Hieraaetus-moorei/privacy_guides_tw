# deGoogle - 替換鍵盤  

> 我手機超方便的，可以直接用鍵盤搜尋  

不少人享受[方便性](https://support.google.com/gboard/answer/9058099?hl=zh-Hant&co=GENIE.Platform%3DAndroid)的同時，疏忽了隱私與資安的風險  

「手機鍵盤」接觸許多機敏資訊，說是「最貼身的程式」也不為過  
傳訊息給朋友、輸入銀行帳密、寫電郵給老闆...  
幾乎所有手機功能，都依賴鍵盤  
_# 別以為語音、手寫輸入就沒事，那些攻擊面積更大_  
若所有 app 都換了，卻用著預設鍵盤，形同資料裝進保險庫，但忘記關門  

---

### 從圖開始看吧！  
[deGoogle keyboard](image link)  
<sup>圖源：除了我還會有誰？</sup>  
<sup>FOSS 指「免費開源軟體 (Free and Open Source Software)」</sup>  
<sup>non-profit 指「不以營利為目的」</sup>  

### 欠換鍵盤  
#### Gboard  
Android 手機預設鍵盤，多半為 Gboard (Google keyboard)  
顧名思義來自 Google，有不少隱私問題：  
* Gboard 使用[聯邦學習](https://security.googleblog.com/2020/10/privacy-preserving-smart-input-with.html) (federated learning)，先將資料去識別化再傳給 Google  
    理論上 Google 不會看到輸入內容，但[特定情況](https://arxiv.org/abs/2306.14793)仍有機會回推  
* 語音輸入會[傳到雲端](https://www.wired.com/story/apple-googles-ai-wizardry-promises-privacy-cost/)，模型運算完再送回  
    部分 Pixel 機型支援地端運算，但多數機種、語言並非如此  
* Google 會儲存用戶和語音助理的互動內容，員工和承包商還會[抽樣聽取](https://www.wired.com/story/whos-listening-talk-google-assistant/)  
    據稱是用於改善服務，但問題是消費者並不知情  
* 拼音輸入法風險高，資料常會上傳雲端  
且加密多半[未落實](https://blog.lapcom.com.hk/2024/05/29/prevent-android-keylogging-and-ime-spying/)，變成[安全漏洞](https://citizenlab.ca/2024/04/vulnerabilities-across-keyboard-apps-reveal-keystrokes-to-network-eavesdroppers/)  
* 輸入語言、當下時間、在哪個應用程式打字、字串長度等 metadata，都會[被記錄](https://www.kaspersky.com/blog/prevent-android-keylogging-and-ime-spying/51281/)  
* 索求[過多權限](https://medium.com/startup-grind/smartphone-keyboards-the-achilles-heel-of-data-privacy-182a69047a7b)，包括網路、精確座標、硬碟、聯絡人、身份、麥克風、相機...  
    麥克風和網路權限，還能用語音輸入、優化服務當藉口  
    但請問鍵盤要你的座標 (你人在哪)、聯絡人、相機是想幹嘛？  

寫到這裡，只能說喜歡被偷窺的可以繼續用  

#### SwiftKey  
微軟的手機鍵盤，同樣有多項隱私爭議  

等等，微軟連手機市場都沒有，卻推出鍵盤！？  

想笑死誰呀！  
![patrick laughing meme](https://media.tenor.com/sD3x5P_M778AAAAC/spongebob-squarepants-patrick-star.gif)  
沒錯，他們就是出了鍵盤  
而且華為、三星多款手機，都拿 SwiftKey 當預設鍵盤  
先前 Gboard 的問題，SwiftKey 也不遑多讓：  
* 要求[過多權限](https://medium.com/startup-grind/smartphone-keyboards-the-achilles-heel-of-data-privacy-182a69047a7b)，包括網路、GPS 精確座標、儲存空間、身份  
* Google 拿的 [metadata](https://www.kaspersky.com/blog/prevent-android-keylogging-and-ime-spying/51281/)，微軟也都要  

該傳到雲端的，當然也沒少  
畢竟人家要練 AI，而你的資料剛好很可口  

---

### 替代品  
#### [HeliBoard](https://github.com/Helium314/HeliBoard?tab=readme-ov-file)  
社群開發者[氦 314](https://github.com/Helium314) 推動的專案，開源、完全離線  
是 [OpenBoard](https://github.com/openboard-team/openboard) 的分支 (fork)，也是繼任者  
_# OpenBoard 是廣受歡迎的開源鍵盤，但久未維護已被封存_  
HeliBoard 可自訂：  
* 個人字典 (包括 emoji、科學符號等)  
也可拿[現成的](https://codeberg.org/Helium314/aosp-dictionaries#dictionaries)  
* 鍵盤主題  
    風格、背景圖片、亮 / 暗色都行  
* 鍵盤佈局  
    按鍵位置、快捷鍵設定等  

支援單手模式、剪貼簿歷史紀錄、分拆鍵盤等  
拼寫檢查、用字建議也沒少，很受社群推崇  

缺點：  
* 滑動輸入使用**閉源**函式庫 (但至少透明揭露)  
* 注音輸入大有障礙，比較適合英語系使用者  
    東亞語言支援都較弱，尚在發展階段  

僅上架 [F-Droid](https://f-droid.org/packages/helium314.keyboard/)，要跑對地方才能下載唷！  
_# 不知道 F-Droid 的，可參閱[前篇文章](./deGoogle-appStore.md)_  

#### [FlorisBoard](https://florisboard.org/)  
同樣為社群驅動的[開源專案](https://github.com/florisboard/florisboard)，成立 FlorisBoard.org 管理開發流程  
[開發者](https://florisboard.org/legal/privacy/) [Lars Mühlbauer](https://github.com/lm41) 為德國人、[Patrick Goldinger](https://github.com/patrickgold) 是奧地利人  
主打高度客製化、離線使用，同樣尊重隱私  
同樣可自訂鍵盤排列、佈景主題、功能手勢、按鍵震動 / 聲響回饋...  
支援滑動輸入、剪貼簿歷史紀錄、單手模式等  

缺點：  
* 尚在 Beta 測試階段，有些功能不穩定  
* **還**沒有拼寫檢查  
    但列在計劃中，可參見[產品規劃](https://github.com/florisboard/florisboard/blob/main/ROADMAP.md)  
* 和 HeliBoard 一樣，不支援注音  
    畢竟開發者是歐洲人，對拉丁語系比較熟  
    其他語言，還有待社群開發者投入 (例如你我)  
上架在 [F-Droid](https://f-droid.org/packages/dev.patrickgold.florisboard/)，[Obtanium](https://apps.obtainium.imranr.dev/redirect.html?r=obtainium://app/%7B%22id%22%3A%22dev.patrickgold.florisboard%22%2C%22url%22%3A%22https%3A%2F%2Fgithub.com%2Fflorisboard%2Fflorisboard%22%2C%22author%22%3A%22florisboard%22%2C%22name%22%3A%22FlorisBoard%20Stable%22%2C%22additionalSettings%22%3A%22%7B%5C%22includePrereleases%5C%22%3Afalse%2C%5C%22fallbackToOlderReleases%5C%22%3Atrue%2C%5C%22apkFilterRegEx%5C%22%3A%5C%22stable%5C%22%7D%22%7D%0A) 亦可取得  
_# 應用程式商店請見[這篇](./deGoogle-appStore.md)_  

#### [Simple Keyboard](https://github.com/rkkr/simple-keyboard)  
直翻簡易鍵盤，超輕量、社群發起的開源鍵盤  
_# 開發者是立陶宛人_  
主打純粹、輕量、極簡主義  

多輕量呢？  

大小不到 1MB，非常省空間  
_# 參考值：一般應用程式動輒幾十、上百 MB_  
也因此僅具基本功能，花俏的東西都沒有  
當然也可離線使用，因為它沒連網功能 XD  
[F-Droid](https://f-droid.org/packages/rkr.simplekeyboard.inputmethod/) 和 Google Play 都能取得  

缺點：  
* 非常陽春，無滑動輸入、拼寫檢查、表情符號等  
    官方自己[說](https://github.com/rkkr/simple-keyboard#about)，可能永遠不會加入那些功能  
* 不支援中文  

極簡主義者或許會喜歡  

#### [AnySoftKeyboard](https://anysoftkeyboard.github.io/)  
社群發起的離線、[開源](https://github.com/AnySoftKeyboard/AnySoftKeyboard)鍵盤，支援[多種語言](https://github.com/AnySoftKeyboard/AnySoftKeyboard/blob/main/addons/languages/PACKS.md)  
_# 抱歉，**不**包括中文_  
可自訂鍵盤佈局，預設就有不少選擇  
甚至有終端機佈局，或許開發者會喜歡 (？)  
支援拼寫檢查、暗色模式、建議選字、語音輸入等  
平時能開按鍵震動、音效，亦可啟動省電模式 (震動音效都取消)  
還有「無痕鍵盤」，拼寫建議不會從此學習  
_# 做偷雞摸狗的事不影響正常選字_  
滑動輸入仍在測試，[社群反映](https://discuss.techlore.tech/t/i-tried-11-mobile-keyboards/10627)該功能尚不穩定  
最特別之處，莫過於可自訂手勢搭配執行的動作  
_# E.g. 左滑換語言_  

缺點：  
* 不支援中文  
* 滑動輸入測試中，功能不穩  
    _# I.e. 可能會失效_  

[F-Droid](https://f-droid.org/en/packages/com.menny.android.anysoftkeyboard/) 和 Google Play 都有  
_# Google Play 有，代表[其他](https://anysoftkeyboard.en.aptoide.com/app)[地方](https://auroraoss.com/https://anysoftkeyboard.en.aptoide.com/app)也能找到_  

#### [8vim](https://8vim.github.io/)  
8vim 是社群推動、受 8pen 啟發的開源專案  
名字很特殊，評價也頗兩極  
8vim 不像傳統鍵盤，採用特殊佈局  
向各種角度滑動，可產出不同字串、符號  
_# 畫面可參考 F-Droid 上的[官方展示](https://f-droid.org/en/packages/inc.flide.vi8/)_  
設計邏輯是熟悉輸入法後，能準確、高速打字  
可自訂功能鍵、配合游標移動、打出特殊字元 (e.g. emoji)  

缺點：  
* 想當然爾，學習曲線陡峭  
    弄熟後或許能高速輸入，但「弄熟」本身就很難哪！  
    困難到官方寫一堆[教學](https://8vim.github.io/docs/category/guides/)，幫助新手入坑  
* 據我所知，應該僅支援英文  

有些人盛讚此鍵盤，它又開源、重隱私  
就放這給各位參考，說不定你是萬中選一的超能使用者  

#### [Thumb-Key](https://github.com/dessalines/thumb-key)  
直翻拇指鍵盤，九宮格[佈局](https://raw.githubusercontent.com/dessalines/thumb-key/main/fastlane/metadata/android/en-US/images/phoneScreenshots/1.png)類似按鍵式手機鍵盤  
社群推出的開源專案，旨在「單手拇指即可操作」  
支援離線使用、emoji、滑動和語音輸入、自訂功能鍵...  
開發者[號稱](https://github.com/dessalines/thumb-key?tab=readme-ov-file#about-thumb-key)「變成肌肉記憶後，字可以打得像物理鍵盤一樣快」  
> As the key positions get ingrained into your muscle memory, eventually you'll be able to approximate the fast speeds of [touch-typing](https://en.m.wikipedia.org/wiki/Touch_typing), your eyes never having to leave the text edit area.  

似曾相識？  
是的，8vim 也採類似哲學  
Thumb-Key 比 8vim 易學一點，但仍有上手難度  

缺點：  
* 得花點工夫學習  
* 似乎不支援中文  

[多數商店](https://f-droid.org/packages/com.dessalines.thumbkey/)都能找到，免費使用  
_# 要錢的我才不會推薦哩！_  

#### [Futo Keyboard](https://keyboard.futo.org/)  
本篇唯一「盈利導向」機構的產品，是家美企  
創辦人 Eron Wolf 曾製作 Yahoo Games、種子輪投資並開發 What's App  
現在全資挹注 Futo，使其不受矽谷投資人左右  
_# 矽谷投資人的金錢遊戲，常會毀掉美妙產品_  
Futo [使命](https://futo.org/about/what-is-futo/)是「取回數位主導權」，擺脫控制狂企業寡頭  
> We used to control our computers. Now our computers are used to control us.  

欸欸別急著走，Futo 鍵盤**免費**、公開原始碼，沒那麼可怕  
之所以沒 FOSS 標籤，是因為它「公開原始碼，但不開源」  

講什麼鬼話？  

請稍安勿躁，**公開原始碼「不等於」開源**  
開源定義更廣，必須能「自由取用、重新分發、可產出衍生作品」等  
_# 詳見[開源簡介](./open-source-intro.md)_  
Futo Keyboard [公開原始碼](https://gitlab.futo.org/keyboard/latinime)，但對重置、分發有諸多[限制](https://gitlab.futo.org/keyboard/latinime/-/raw/master/LICENSE.md)  
畢竟人家要賺錢，怕其他公司整碗端走  
看看該產品好在哪，為何怕別人偷：  
* 離線使用，包含語音功能  
    官方口號：你的鍵盤不應連網  
* 支援滑動、語音輸入  
    語音模型架在本地，也就是你的手機裡  
    中文語音也行，但請選[專用模型](https://keyboard.futo.org/voice-input-models)  
* 拼寫檢查、預測選字都沒少  
* 預載少量佈景主題，可輕鬆個人化  

語音輸入、預測選字功能強大，社群好評聲浪不斷  
這就是為什麼明明一堆開源選擇、Futo 身為盈利美企、僅公開原始碼  
卻仍被選入推薦榜，因為實在值得一試  
_# 重點是離線使用，個資不怕被偷_  

缺點：  
* 還在 Alpha 測試階段，功能不太穩定  
有些人回報自動選字、滑動輸入失靈  
偶爾也會出現詭異的 bug，不過官方修復迅速  
_# Alpha 完才換 Beta，所以仍屬開發嬰兒期_  
* 尚無剪貼簿整合  
* 缺乏注音鍵盤  
* 美企  

可一次性付費購買授權，但不給錢也無任何影響 (免費仔鬆一口氣)  
類似捐助，確保 Futo 能存活下去  
   
#### [Guileless Bopomofo (樸實注音鍵盤)](https://github.com/hiroshiyui/GuilelessBopomofo)  
看完一堆美妙鍵盤，卻沒一個能打注音，很惱怒嗎？  
這不就來了 - 本篇第一個 (也是唯一)堪用的注音鍵盤  
由[台灣人](https://ghostsinthelab.org/)開發的[社群](https://bobtung.medium.com/)[專案](https://github.com/cataska)，開源、尊重隱私、可離線使用  
Guileless 指「誠實、老實的」，Bopomofo 就是ㄅㄆㄇㄈ啦！  
援引[新酷音](https://chewing.im/about.html)輸入法，即你熟悉的注音鍵盤  
一直有在更新，介面越變越好看 (維護錯重點？)  
上架在 [F-Droid](https://f-droid.org/zh_Hant/packages/org.ghostsinthelab.apps.guilelessbopomofo/)，永久免費、無廣告  

缺點：  
* 無自動選字功能，得老老實實拼寫  
* 偶爾會有 bug，畢竟開發者只有一人、也沒拿錢  
    _# 本文撰寫時，按下該鍵盤逗號都會變成「ㄝ」，後來已修正_  

能切換英文輸入，還算堪用  

#### [Unexpected Keyboard](https://github.com/Julow/Unexpected-Keyboard)  
社群推出的開源離線鍵盤，不蒐集個資、也完全免費 (但你可以贊助)  
配置乍看很普通，不過各按鍵四周都被標上小符號  
按住按鍵後，往哪個角落滑就能輸出該角落的符號  
免切換輸入法，就能打出各種文字  
_# 不易想像的話，可參見[官方示範](https://github.com/Julow/Unexpected-Keyboard#unexpected-keyboard-)_  
支援多語言，但不包括注音  
不需學習，裝完大概就會用  

缺點：  
* 沒注音輸入  
* 無拼寫檢查、建議詞彙  
* 社群批評有點醜，不過審美觀因人而異  
[F-Droid](https://f-droid.org/en/packages/juloo.keyboard2/)、[Google Play](https://unexpected-keyboard.en.aptoide.com/app) 都能取得  

---

#### iOS 鍵盤？  
前面只提 Android 替代品，那 iPhone 用戶呢？  
蘋果預設鍵盤 QuickType，難道不用換嗎？  

QuickType 隱私政策較理想：  
用[差分隱私](https://www.wired.com/2016/06/apples-differential-privacy-collecting-data/) (differential privacy)蒐集統計資料，去識別化才拿走  
平常拼寫檢查、自動選字，都在你手機離線完成  
不過若開啟 Siri 聽寫，資料同樣會[送到雲端](https://www.apple.com/legal/privacy/data/en/ask-siri-dictation/)，用以處理、優化服務  
雖然閉源，但未達隱私威脅，因此未呼籲替換  
更重要的是，iOS 生態系封閉，想換也沒多少選擇啊！  
唯一優質替代品 [kif - keyboard](https://apps.apple.com/us/app/qwerty-keyboard/id1434021039)，2021 年已停止維護  

---

背景故事：  
    開發者[表示](https://github.com/cemheren/akifkeyboard)，當初受夠第三方側錄，所以自己做鍵盤  
    推出一款開源、尊重隱私，且功能幾乎等同 QuickType (iOS 預設鍵盤)的軟體  
    支援多語言、滑動輸入、暗色背景、拼寫檢查等  
    但 2021 年時，他說受夠蘋果各種詭異要求，決定不再維護 (說不定蘋果稅也是一環)  
> I was sick of dealing with Apple's weird demands and focused on other projects  

---

能換當然換，但沒選擇也沒辦法  
買蘋果手機，就只好自認倒霉囉！  

---

### 懶人包~~青天~~  
~~抓到，偷懶仔，你是不是沒看文章就直接滑到這~~  
* 拉丁語系 (e.g. 英文)：  
    * 想要 AI 輔助、接受美企 → [Futo](https://keyboard.futo.org/)  
    * 喜歡滑動輸入、自訂佈局：  
        * 想要拼寫建議 → [HeliBoard](https://github.com/Helium314/HeliBoard?tab=readme-ov-file)  
        * 偏好高度客製化 → [FlorisBoard](https://github.com/florisboard/florisboard) / [HeliBoard](https://github.com/Helium314/HeliBoard?tab=readme-ov-file)  
    * 不需滑動輸入，但想要拼寫建議、自訂功能 → [AnySoftKeyboard](https://anysoftkeyboard.github.io/)  
    * 極簡主義者，只要最基礎、輕量的鍵盤 → [Simple Keyboard](https://github.com/rkkr/simple-keyboard)  
    * 不喜歡切輸入法，想全在同介面解決 → [Unexpected Keyboard](https://github.com/Julow/Unexpected-Keyboard)  
    * 嚮往單手打字：  
        * 願意花時間學、想特立獨行 → [8vim](https://github.com/8VIM/8VIM) (學不會不負責)  
        * 喜歡舊式手機九宮格排版 → [Thumb-Key](https://github.com/dessalines/thumb-key)  
        * 雙手打字時不想換軟體、想客製化 → [HeliBoard](https://github.com/Helium314/HeliBoard?tab=readme-ov-file) / [FlorisBoard](https://github.com/florisboard/florisboard) (單手模式)  
* 注音輸入法 → [Guileless Bopomofo](https://github.com/hiroshiyui/GuilelessBopomofo) ([樸實注音鍵盤](https://f-droid.org/en/packages/org.ghostsinthelab.apps.guilelessbopomofo/))  
* iOS 用戶 → ~~自生自滅~~ [kif - keyboard](https://github.com/cemheren/akifkeyboard)  
    _# 但專案已停止維護，能否下載、正常運作，全看你造化囉！_  

---

細心的讀者可能有發現，以往圖片常加皇冠、偷渡推薦次序  
_# 例如 [Searxng](./deGoogle-search-engine.md)、[Proton Mail](./deGoogle-email.md)、[F-Droid](./deGoogle-appStore.md)_  
但鍵盤使用因人而異，本篇沒納入這種考量  
[HeliBoard](https://f-droid.org/packages/helium314.keyboard/)、[FlorisBoard](https://f-droid.org/packages/dev.patrickgold.florisboard/) 很推薦給英文使用者  
[Futo](https://futo.org/) 若非美企，其實也很推薦  
[樸實](https://github.com/hiroshiyui/GuilelessBopomofo)是唯一堪用的注音鍵盤，台灣用戶可能需要  
也可以裝一個好用的外文鍵盤 (e.g. [HeliBoard](https://f-droid.org/packages/helium314.keyboard/))，搭配[樸實注音鍵盤](https://f-droid.org/zh_Hant/packages/org.ghostsinthelab.apps.guilelessbopomofo/)使用  
每個都玩玩，再做決定也無妨  



