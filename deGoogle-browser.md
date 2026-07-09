# deGoogle - 替換瀏覽器  

### 前言  
本篇將鉅細彌遺介紹，瀏覽器相關的知識背景  
**看倌不必全部讀完，挑對自己有幫助的部分即可**  
當然，欲全面瞭解瀏覽器生態的，也歡迎全文詳讀  

---
  
> Chrome 吃太多記憶體了，而且跑超慢  

Google Chrome 作為主流瀏覽器，雖已由 Google 優化驅動引擎，但為了各種目的 (例如廣告、追蹤器)，犧牲了不少效能  
就算不論隱私，差勁體驗早已令人厭倦  
噁心的是，Google 把 Chrome 塞入 Android，綑綁銷售  
預設為 Andoird 瀏覽器外，想換還刪不掉它 (只能停止)  
預設瀏覽器對市占率影響很大，因為不論是懶得換、或根本不知道有其他選擇的人，就很可能固著在預設瀏覽器上  
微軟當初把 IE 瀏覽器隨 Windows 強迫推銷，靠 OS 壟斷優勢搞垮 Mozilla Firefox 的前身 Netscape Navigator，因而被美國[反壟斷法制裁](https://www.justice.gov/atr/us-v-microsoft-proposed-findings-fact-0)  
不正當的競爭手段，往往能讓「一無是處的產品」擠進主流  
多數人用 Google Chrome (市占逾六成)，不代表它就是好東西  
_# 小提醒：主流瀏覽器中，只有 Chrome 對跨站 cookies 網開一面，方便別人追蹤你_  

---
  
### 瀏覽器 (Browser)  
替換產品前，得先簡介一下要換的東西  
瀏覽器是進入網路世界的主要途徑，Windows 內建 Edge、Android 內建 Chrome、MacOS 內建 Safari  
那些預設瀏覽器，都是該廠商推出的閉源產品，藉由綑綁行銷，強行增加市占率  
瀏覽器引擎主要分三類：  
* Blink (Chrome / Chromium)  
* Gecko (Firefox)  
* WebKit (Safari)  

Chromium 是 Chrome 的核心，驅動引擎是 Blink，而 Chromium 本身開源  
因此許多知名瀏覽器建構在 Chromium 上，例如 Brave、Vivaldi、Edge 和 Opera  
_# 注意：開源的是 Chromium，不是 Chrome  
且 Chromium 仍由 Google 開發維護，不完全獨立於科技巨頭_  
Gecko 是 Mozilla 開發的開源引擎，Firefox 以此驅動，是 Chromium 的重要競品  
_# Gecko 是守宮 (一類壁虎)，Mozilla 很愛用動物命名產品_  
WebKit 由蘋果開發、開源，是 Safari 的核心  
_# 有趣的是，Blink 是 Google 從 WebKit 改來的，現在卻反超成為主流引擎_  

講這些幹嘛？  

因為之後要介紹的瀏覽器，多半基於 Gecko (Firefox)，所以先提一下它們的愛恨情仇  
為何是 Gecko？  
因為除了 Chrome，Chromium 系列瀏覽器也受制於 Google  
WebKit 系列則受制於 Apple，且發展很少、使用平台受限  
身為唯一有效、獨立競爭者，選 Firefox 系列對市場競爭很重要，尤其就隱私保護而言  
很多開發者也意識到這點，所以高隱私、安全的瀏覽器，多半建構在 Firefox 之上  

上述乍看像陰謀論，但事實便是如此  

讓營利企業壟斷，就會發生各種惡霸行徑，譬如 Youtube [廣告劣化](https://www.mirrormedia.mg/story/20250109edi025)、[延長化](https://www.reddit.com/r/youtube/comments/1i89wj8/60_minute_unskipable_ad/)、[取消背景播放](https://support.google.com/youtube/answer/7437614?hl=zh-Hant&co=GENIE.Platform%3DAndroid) (勒索大家買 Premium)  
Chrome 強制升級 Manifest V3，[不再支援](https://superuser.com/questions/1884201/these-extensions-are-no-longer-supported-chrome-recommends-that-you-remove-them)特定廣告 / [追蹤器攔截外掛](https://ublockorigin.com/) (此非未來式，是完成式)  
Android 機種綁死 Google 生態系，甚至在更新中偷渡 Gemini app  
光六成市占率，Chrome 就可以亂搞了 (除非另行開發，否則其他 chromium 基底的瀏覽器，也得被迫配合)  
如果世上只剩 Chromium 基底的瀏覽器，甚至只剩 Chrome，你我要碼交出大量個資、觀看鋪天蓋地的廣告，要碼付錢給 Google  
所以 Firefox 的市場競爭很重要，確保大眾還有選擇  
至於近年出現的第三勢力，[Ladybird browser](https://ladybird.org/)，因尚處開發、測試階段，沒程式背景的人應該玩不了，就不在此贅述 (甚至沒下載按鈕)  

終於來到懶人圖了：  
[deGoogle Chrome](image link)  
<sup>圖源：我本人</sup>  
有些瀏覽器只有桌面版、有些則只有行動版  
至於 Telemetry (遙測)、fingerprint、Tor、uBlock Origin 是什麼，稍後會解說  
該換的除了 [Chrome](https://www.forbes.com/sites/zakdoffman/2021/03/20/stop-using-google-chrome-on-apple-iphone-12-pro-max-ipad-and-macbook-pro/) ([醜聞](https://www.forbes.com/sites/zacharyfolk/2024/04/01/google-will-destroy-incognito-mode-browsing-data-heres-what-that-means-for-users/)超多)、[Edge](https://www.zdnet.com/article/a-professor-says-edge-is-the-worst-for-privacy-microsoft-isnt-happy/)、[Safari](https://www.theregister.com/2024/04/30/apple_safari_europe_tracking/) (比前二者好「一點」，但閉源、廣告追蹤無法擋、隱私外掛不支援、綑綁生態系...)，還有 Opera  
Opera 粉絲可能很震驚：「Opera 不是保障隱私的挪威公司嗎？」  
首先，Opera 建構在 Chromium 上、閉源，且[出過資安問題](https://www.darkreading.com/vulnerabilities-threats/crossbarking-attack-secret-apis-expose-opera-browser-users)  
再者，2016 年奇虎 360、昆侖萬維等的中國集團，收購了 Opera  
閉源又中資，當然換掉  

---
  
### 背景知識  
想無腦選瀏覽器可略過本段  
#### [Tor](https://www.torproject.org/) 是什麼？  
圖例中的那顆洋蔥，指「是否支援洋蔥路由」  
洋蔥路由的做法是，每個連線都經三層加密，傳到一個節點解密一層，所以單一伺服器無法解析請求來源、連線到哪 (造訪什麼網站)  
節點就是伺服器，是分散式的架構，由許多志願者、機構維運，無特定人士能掌控 (你高興的話，也可以架一台進 Tor network)  
_# 題外話，柯南《零的執行人》劇中的「Nor」網路，本尊就是 Tor 喔！  
Tor 比 VPN 更安全，許多人權倡議者、獨裁政權下的記者，都藉此匿蹤連網  
_# 注意：Tor 並非絕對安全，使用者不當操作仍可能導致曝光，稍後會再提_  
缺點是速度很慢，畢竟要多層加、解密，不適合日常瀏覽 (你能接受電動每 10 秒更新一次畫面？)  
需靠洋蔥路由才能造訪的網站，就稱為「暗網」  
很多人受電影影響，以為「暗網」充斥醜惡的東西  
原因是暗網不受監管，所以人性黑暗面可能會在其中展現  
但許多主流服務為突破特定政權封鎖，也會架設 xxx.onion 的暗網版頁面，例如 Facebook (你喜歡的話，也可以自架暗網頁面喔！)  
> 科技無罪，人的選擇才決定善惡 - 移幣  

#### 瀏覽網路，會留下指紋 (Fingerprint)？  
此處 fingerprint 指瀏覽器指紋，是「可辨識特定用戶的特徵」總稱，非單一項目  
例如 IP、時區、瀏覽器種類、預設語言、背景主題 (暗色或亮色)、裝哪些外掛、用什麼平台 (Mac、Windows 或 Linux 等)、行動裝置還是電腦、螢幕寬度、硬體配置...  

看起來和瀏覽器無關？  

不，只要非高隱私瀏覽器，網站都很容易能取得那些資訊  
有些無良網站，甚至會傳一個透明的圖、沒聲音的音訊，藉此探知你瀏覽器渲染所需時間，鎖定你用哪種硬體  
就算沒登入，仍可能被抓出身份
想像一下，假設你沒翻 VPN、沒做任何防護，如同一般使用者  
你開 Chrome 無痕模式逛購物網，爾後關閉瀏覽器，再度開啟以用「乾淨之身」造訪遊戲網站  

以為很安全了，對吧？  

若網站維運者為同個集團、或有交流客戶資訊，甚至更常見的情況是，使用相同第三方服務 (e.g. 廣告投放，像 Google ad)  
他們就能靠你的「網路指紋」知道你有玩 ooo 遊戲、喜歡買 xxx 物品，以及你所逛過~~見不得光~~的網站  
怎麼做呢？  
首先，IP 位址相同、瀏覽器相同 (Chrome 無痕)、裝置相同 (都是你的手機)、OS 都是 Android、瀏覽器都裝暗色外掛...  
光第一點，就幾乎可確定你是誰了  
搭配其他特徵，你在無痕的活動，並不如想像中私密  
好奇你的瀏覽器多脆弱，可透過此[線上測試](https://coveryourtracks.eff.org/)玩玩  
_# 放心，那是非營利機構「電子前鋒基金會 (Electron Frontier Foundation, EFF)」的網站_  
或參考 Proton 的[測試報告](https://proton.me/blog/best-browser-for-privacy)  
#### [uBlock Origin](https://ublockorigin.com/) (uBO) 關瀏覽器選擇什麼事？  
關係可大了！  
很多人聽過 Adblock 這類「廣告攔截器」，也常尋找各式的擋廣告外掛  
而 uBlock Origin 可謂「地表最強廣告攔截器」，但其本質是個「[廣泛內容攔截器](https://github.com/gorhill/uBlock/wiki/Blocking-mode)」  
有礙隱私者，如廣告、追蹤器、惡意網域與資源濫用都擋  
_# 第三方廣告多伴隨追蹤器，也會浪費資源載入  
有時第一方廣告仍可顯示，例如劍橋辭典側邊欄  
所以許多保障隱私的瀏覽器，都預設安裝 uBlock Origin  
廣告過濾在你的瀏覽器發生，沒所謂「官方」會偷窺你  
授予權限不怕洩露隱私，反而能保護隱私  
廣告載入前就被擋、uBO 本身又很輕量，啟用後上網會更快、更省電  
_# 如果你喜歡環保，uBO 還能減少跑廣告所需的電能，更該支持_  
強到什麼程度呢？  
* 常見廣告都不會出現，包括 Gmail 推銷、方格子廣告 ~~(方格子別 ban 我)~~  
* Youtube 形同 Premium，看不到廣告  
* 高度可客製化，哪些網站擋、哪些不擋，都能用 GUI 調整  
* 網站、網址的追蹤器，也能擋掉  
* 效能很高，且廣告載入前就會被屏蔽，所以甚至能「加速」瀏覽體驗  
* Safari 外的瀏覽器都支援，直到 Google 打不贏只好改到 Manifest V3  
* 不用帳號不用錢，[獨立社群開發者](https://github.com/gorhill/uBlock)所創、維護，**不接受贊助** (不為錢而來)  

uBlock Origin 最初叫 μBlock (後改名 uBlock)，[Raymond Hill](https://github.com/gorhill) 覺得處理用戶需求像「乏味的工作」，而非嗜好  
故將 uBlock 專案轉交給 Chris Aljoudi，分家出 uBlock Origin、把 uMatrix 專案的概念融入，使其日趨完備  
而另一頭，uBlock 專案漸漸卡住，終至停止開發  
後來 Adblock 公司買下 uBlock.org，經一番波折成為耳熟能詳的 Adblock 外掛  
但效能、擋攔截器有效性，都輸 uBlock Origin 一大截，畢竟他們希望用戶買 Adblock plus (營利公司的缺點)  
Google 把 Chromium 推上 Manifest V3 後，Chromium 基底的瀏覽器，便不再相容於 uBlock Origin 了 (有些後門仍可通行，但不排除將來 Google 出手關門)  
開發者也說，不會再支援 Chromium 系列  
粉絲有兩個選項：  
* 改用 Firefox 基底的瀏覽器  
    因為 Firefox 雖然升級，但仍保留對 Manifest V2 的支援，尤其 WebRequest API  
    _# 那個 API 就是廣告攔截器高效過濾的關鍵_  
* 用 uBlock Origin Lite (輕量版)，保護效果、功能都少很多  
    _# uBO Lite 也支援 Safari 唷！_  

其實還有第三個選擇，就是瀏覽器發行商自行調整，讓產品兼容 uBlock Origin (Manifest V2)  
至於 Firefox 會不會放棄向後相容性，應該不必太擔心  
因為 Firefox CTO 自己說很愛 uBO，沒意外會繼續支援下去  

#### Telemetry 遙測又是什麼？  
此處的遙測，指內建在瀏覽器中、回傳給發行商的資訊  
例如不正常關閉、使用紀錄、異常行為等  
你可曾有不慎踩到電源，強制關閉電腦的經驗？  
重開機後，可能會跳出「瀏覽器不正常關閉」，並有個問題回報選項  
按下回報，就會把斷線資訊傳給瀏覽器發行者 (e.g. Google)  
內建的遙測更可怕，你沒按下任何按鈕，仍會傳出資訊  
何時開、關，每個 session 多久，都可能被傳出，算很侵入式的資訊獲取  
但瀏覽器本質是上網，不太可能斷網防止遙測，不然你要瀏覽器幹嘛？  
圖中的 Telemetry-free 指無遙測，**你的瀏覽器就真的是你的瀏覽器**  

---

### 正題：替代瀏覽器介紹  
**本篇介紹的替代品，「以開源、免費，且和 uBlock Origin 相容」為原則**  

#### [Brave Browser](https://brave.com/)  
對習慣 Chrome 的人來說，Brave 瀏覽器算轉換成本最小的  
因為 Brave 是本篇「唯一」基於 Chromium 的隱私瀏覽器  
它容許 Youtube 背景播放、內建 Brave Shield (廣告/追蹤器攔截器)、Leo (隱私 AI 對話功能，預計另行撰文介紹)、Brave Talk (視訊功能，以後的文章會提)、預設用 Brave 搜尋引擎 ([之前介紹過](https://vocus.cc/article/68921a5efd89780001926c42#data-h3-4-68921a5efd89780001926c42))...  
官方也做出調整，讓 Brave 雖身為 Chromium 系列，卻**仍可使用 uBlock Origin**  
只想用 Brave Shield 也行，體驗很類似 uBlock Origin，只是功能不那麼細緻  
_# 好處是內建在瀏覽器裡，所以不受外掛平台影響_  
Brave 還有個特點：支援 Tor 連線！  
你可以用 Brave 瀏覽器，進入先前提過的暗網  
不用高深的技術，按鈕點一點就行  
**注意：Brave [官方說過](https://brave.com/blog/tor-bridges/)，須高度隱私的行為，仍應使用 [Tor 瀏覽器](https://www.torproject.org/download/)進行** (稍後會介紹)  
不提不行的是，Brave 有獨特**抗網路指紋**功能  
每次造訪網站，哪怕是同個網頁，Brave 都會隨機化可辨認特徵  
只要你不登入，就難以被網路指紋鎖定，有興趣者可至 [EFF](https://coveryourtracks.eff.org/) 測試 (Brave 表現十分優異)  
_# 請記得，一旦你「登入」某服務，等同交出高度可辨識特徵，不論是 Tor 還是網路指紋防護，都沒辦法阻止網站知道你是誰 (就像穿著隱形斗篷，卻拿身分證給人看)_  
有興趣者還可開啟 Brave rewards，會看到 Brave 容許的廣告，但能賺虛擬貨幣 (就算被擋掉，仍有機會計入獎勵)  
_# 該功能預設關閉，看不爽[把它隱藏](https://www.youtube.com/watch?v=W6cKFliWW6Q)即可_  
Windows 用戶可能有聽說，微軟近期加入的 Microsoft Recall 會 20 秒截圖一次你的畫面，號稱為了 AI 功能而設  
大量反彈聲浪下，微軟允許關閉該功能，而 Brave 在此之前，就加入「瀏覽器畫面不受擷取」的保護，以用戶隱私為優先考量  
喜歡 Brave 的人，不必擔心平台問題  
所有主流平台如 Mac、Windows、Linux、iOS 和 Android，都能下載 Brave 瀏覽器！  
缺點：  
* 遙測需手動關閉，選擇有限  
* 臃腫，不必要的功能、介面很多  
* 美國公司，若坐大難保不會變成下一個 Google  

後來推出 [Brave Origin](https://brave.com/origin/download-nightly/)，基本上就是乾淨版的 Brave (把臃腫功能拔光)  
不過要價幾千台幣，建議有錢的再去玩 (好消息，Linux 版免費！)  


#### [Mullvad Browser](https://mullvad.net/en/browser)  
噹啷，[又是](https://vocus.cc/article/68921a5efd89780001926c42)瑞典公司 Mullvad！  
身為 VPN 公司，最知名的產品卻是瀏覽器，很~~諷刺~~棒吧？  
Mullvad 瀏覽器改自 Firefox，移除所有遙測、整合 Mullvad VPN (可不使用)、預設搜尋引擎為 Mullvad Leta ([這篇](https://vocus.cc/article/68921a5efd89780001926c42)提過)  
_# Mullvad Leta 已不再維運 QQ_  
和 Tor 計畫結盟，號稱「只差洋蔥路由的 Tor 瀏覽器」  
_# Mullvad 對抗網路指紋的原理和 Tor 一樣，稍後再仔細解說_  
不儲存個人資訊如帳密、瀏覽記錄等 (關掉即刪光，預設就像無痕模式)。可能不方便，但很安全  
_# 因此可選為預設瀏覽器，點擊連結時用它開啟，關掉就刪乾淨_  
甚至連 uBlock Origin 都幫你裝好了  
上述配置是為了「開箱即用」，意思是不需額外調整  
想像你開公用電腦，查詢某些資料、登入特定帳號  
如果直接用 Chrome、Edge，得擔心帳密、瀏覽記錄是否被儲存，以及會不會被追蹤  
但有了 Mullvad，你要做的是「查詢 Mullvad Browser」，並下載、安裝  
之後一切從 Mullvad 出發，Google、公用電腦取得的資訊，只有你查了 Mullvad  
哪怕未刪除 Mullvad，關閉瀏覽器後，下一個人再開也只會看到全新頁面，什麼資料都沒留  
缺點：  
* 目前只有桌面版，手機不支援  
* 設定像無痕，有些人可能不習慣 (但我超愛)  

Mullvad 在改進瀏覽器方面，非常有效率  
[評比網站](https://privacytests.org/)上，Mullvad 從前和 Firefox 差不多，現在卻變成數一數二保護隱私的選擇  

#### [Tor Browser](https://www.torproject.org/download/)
最安全、隱密的瀏覽器，沒有之一  
Tor 是 [Tor project](https://www.torproject.org/) 官方基於 Firefox 魔改來的，拔光遙測、所有設定都調成隱私保障款  
預設支持洋蔥路由 (The Onion Routing, Tor)，可直接進入暗網  

---

講古：  
洋蔥路由是美國海軍實驗室草創，研究匿蹤通訊科技  
初創者退役後改為民間單位，MIT 電腦科學家加入團隊  
後續轉向對抗流量監聽、網路活動審查、保障隱私等，並成立 [Tor project](https://www.torproject.org/) 非營利組織，早期主要靠電子前鋒基金會 ([EFF](https://www.eff.org/))贊助  
洋蔥路由連線皆經三層加密，沒有單一伺服器能解析使用者 IP、網路活動  
伺服器群是志願者、機構架設，分佈於全球各地，不受特定政府管轄  
Tor 瀏覽器除了洋蔥路由，也抗指紋追蹤  
原理是混合「所有使用者資訊」，讓每個人看起來都一樣 (和 Brave 正好相反，但都很有效)  

---

同樣開箱即用，不需額外調整  
但使用者才是關鍵，不當使用仍會破壞 Tor 匿名性  
譬如登入某些帳號，你的登入資訊仍會被抓到  
或造訪 http 而非 https 網站，又做各種資料、訊息傳輸，則第三方仍有機會竊聽  
官方未加裝 uBlock Origin，也**強烈不建議安裝任何外掛、改任何設定**  
否則可能破壞匿名性、增加受敵面積 (因為外掛程式可被網路指紋追蹤，你會在拌勻的資訊裡鶴立雞群)  
**Tor 保障的是網路安全，至於軟硬體、電腦被埋側錄程式等問題，不在守備範疇內**  
缺點：  
* 除非是高風險人士，否則不建議日常活動使用 Tor  
   不然你只會覺得，網路變很慢很難用  
* 沒 iOS 版，iPhone 可改用 Onion Browser (下文會介紹)  

#### [LibreWolf](https://librewolf.net/)
Libre- 是拉丁文「自由」之意，Wolf 就是狼，所以是自由的狼  
這個專案非常酷，由社群人士自發投入，將 Firefox 改得更隱私友善  

---

講古：  
2020 LibreWolf 會創立，是因為 Mozilla 諸多作為惹惱不少隱私愛好者  
* Firefox 發行者 Mozilla 不斷追加遙測功能，還越來越侵入式  
* 除了增加遙測，又把「贊助 Mozilla」、「Mozilla VPN」等各種功能，擺到更顯眼處  
    白話文就是，偷你資料又推銷產品  
* Mozilla 更新使用條款，把「永遠不會使用用戶資料」刪掉，又移除「漸進式網頁應用程式 (Progressive Web App, PWA)」支援  
* 另一個受歡迎的 Firefox 分支，Waterfox，在 2020 年初被廣告公司 System1 收購 (沒錯，就是我[搜尋引擎那篇](https://vocus.cc/article/68921a5efd89780001926c42)提過的廣告公司)  
社群覺得自由、獨立的本質消失了，需要有替代品  

這時候，開源的優點就很耀眼啦！  

開發者創建新的 Firefox 分支 (fork)，並大肆修改，命名為 LibreWolf 象徵重新取回自由  

---

LibreWolf 適合偏執用戶 (例如我)，因為以下出廠設定，或許不適合一般人：  
* 關閉程式即刪除 cookie、瀏覽記錄 (形同無痕，和 Mullvad 一樣)  
* 反網路指紋設定，預設開啟  
* 拔光所有遙測，也拆除 Mozilla 置入性行銷，非常乾淨  
* 預設安裝 uBlock Origin  
* 螢幕寬度設死、背景設為亮色系、時區是 UTC + 0、不允許硬體圖像渲染...  
    這些設定是用來保護網路指紋，降低個體獨特性  
* 更新十分快速，只要 Firefox 推出更新，他們多半會在 1 天內跟上  
    若有任何漏洞修補，LibreWolf 也能立刻跟進  
* 預設搜尋引擎為 DuckDuckGo (請參見我的[搜尋引擎比較](./deGoogle-search-engine.md))，不綁 Google  

LibreWolf 超棒的，因為是社群專案，有任何意見都能直接向開發者反映  
往往也會迅速得到回覆，且不受制任何公司  
缺點：  
* 只有桌面版  
* Mac 用戶安裝不便  
   開發者拒付蘋果稅，得手動下載、安裝  
   Windows 則可[無腦裝](https://librewolf.net/installation/windows/)  
* 無自動更新，需手動處理  
   若用指令安裝，可仰仗套件管理器的自動更新功能  
* 阻擋硬體渲染，有些網站載入圖片會稍慢  

總之，LibreWolf 比較像「面向開發者的瀏覽器」，日常用戶需適應一下  
LibreWolf 官網有[很多資源](https://librewolf.net/docs/testing/)，有興趣可參考  

#### [Zen Browser](https://zen-browser.app/)
Zen 可說是開源、Firefox 基底版的 Arc 瀏覽器 (也許有些老人聽過？)  
Zen 同樣是社群自發的專案，注重隱私但不像前幾個那麼極端  
撰文時仍在 beta 測試階段，會一直更新功能、介面  
有垂直標籤列、整合標籤等流行設計，且畫面偏極簡  
可客製化功能多，且有 Zen Mods (畫面風格外掛)能直接套用  
獨家功能是，可在瀏覽器畫面內分割多個視窗  
官方陸續拔除了遙測，新版已不會送資訊給 Mozilla  
相較於前幾個項目，Zen 比較像「尊重隱私」而非「守護隱私」  
簡言之，Zen 不拿你的個資，但也沒太多額外保護  
缺點：  
* 快速發展中，可能遇到 bug  
* 未預裝 uBlock Origin、保護較弱 (但還堪用)  
* 尚且只有桌面版，行動裝置無緣消受  
* 官方對[隱私](https://github.com/zen-browser/desktop/discussions/5907)、[漏洞](https://github.com/zen-browser/desktop/issues/5947)的應對方式，令人[生疑](https://news.ycombinator.com/item?id=43443494)  

#### [Floorp](https://floorp.app/)  
Floorp 是罕見的「日本製」瀏覽器，比壓縮機還稀少 (唯一亞洲貨)  
2021 年時由[日本學生](https://docs.floorp.app/docs/other/contributors/) aka 社群開發者，以「Firefox 界的 Vivaldi 瀏覽器」為定位創建  
Floorp 高度可自訂，雙側邊欄、標籤位置等功能都沒少  
摘除 Mozilla 遙測，還有嚴格模式能進一步防守  
嚴格模式封鎖特定 API、偽造 WebGL 資訊 (即前述硬體渲染)、也預設使用容器區隔分頁  
_# 封鎖的 API 主要是易洩漏資訊者；容器化可隔離個別分頁，避免跨站追蹤_  
Floorp 甚至提供「一鍵切換 user agent」，也就是從原本「xxx 平台的 Firefox 使用者」，喬裝成「ooo 平台的 Chrome 用戶」  
_# 平台指 OS，例如 Windows、Linux_  
不過 user agent switcher 在第 12 版後停止支援，需靠外掛達成  
缺點：  
* 僅有桌面版  
* 未先安裝 uBlock Origin，要自己記得補裝  
   某些版本似乎有預裝，但新版官方又移除了  
* 高保護的嚴格模式，需手動切換，並非「開箱即享有」  
* 文件更新較慢，需注意是否有過時描述  

#### [Waterfox](https://www.waterfox.net/)  
Waterfox 直翻「水狐」，因應火狐而取名  
從前也是社群專案，專為隱私打造 (LibreWolf 那段提過)  
不過曾被美國廣告公司 System1 收購、預設 Startpage 為搜尋引擎，令不少開發者惱怒  
_# 好消息是，2023 年水狐開發者 Alex Kontos [宣布](https://www.waterfox.net/blog/a-new-chapter-for-waterfox/)，Waterfox 重新獨立！_  
好處是 Waterfox 開源、有相對隱私的設定  
例如移除預測遙測、 阻擋追蹤器、一鍵清除資料，也脫去 Mozilla 置入的功能  
且支援 Chrome、Opera、及新舊版 Firefox 外掛 (但不保證完全相容)  
各大主流平台都可取得，包括電腦和手機 (除 iOS 外)  
缺點：  
* 之前能隨便出售，以後會不會再賣，難說  
* 沒預載 uBlock Origin，需手動安裝  
* 預設搜尋引擎 Startpage ，已被美國廣告公司 System1 收購  
   _# 開發者有做個 [Waterfox Private Search](https://www.waterfox.net/blog/waterfox-private-search/)，但截稿前仍在 Beta 測試階段_  
* 隱私保障中等，額外措施不多  

2026 年更成為除了 Brave，第一個使用其函式庫實作廣告攔截器的瀏覽器  
過濾引擎用 rust 寫成、無需外掛，效能高、攻擊面積較小  
還正在早期測試中，穩定度不保證，且預設會留文字廣告 (為了 startpage 廣告分潤)  
用戶得自行點選全擋，才能取回乾淨頁面  

#### [Onion Browser](https://onionbrowser.com/)  
前面提到 Tor 瀏覽器無 iOS 版，但社群開發者是很厲害的，沒有就做一個出來呀！  
[Mike Tigas](https://github.com/mtigas)，自稱駭客兼記者，開發了 Onion browser (直譯就是「洋蔥瀏覽器」，因 Tor 是「洋蔥路由」)  
[Guardian project](https://guardianproject.info/2019/10/08/onions-on-apples-a-new-release-of-onion-browser-for-ios/) 贊助下，開放免費下載  
後來 Tor 官方更[推薦](https://support.torproject.org/tbb/tbb-31/)洋蔥瀏覽器，稱其為 iOS 上最好的 Tor 替代品  
洋蔥瀏覽器內建 Tor 代理，白話文就是能直接連上 Tor，基本上就是「iOS 版的 Tor」  
_# 也可串接 [Orbot app](https://orbot.app/en/)，連線至 Tor 網路_  
同樣開源非營利，建構在 WebKit 核心上，有銅銀金三種防護程度可選 (預  設為銀)
缺點：  
* 建構在 WebKit 引擎而非 Firefox 上，安全性較低  
   WebKit 是蘋果推出的 Safari 核心，相較 Firefox Gecko，開發者能動的底層[設定](https://www.privacyguides.org/articles/2024/09/18/onion-browser-review/#other-settings)不多  
   更何況審視 WebKit 的開發者較少，所以安全性不如其他平台的 Tor  
   _# 別怪 Onion，去**怪蘋果**！他們規定「**上架 iOS 的瀏覽器，都必須用 WebKit 核心**」_  
   儘管歐盟反壟斷法，讓其他核心也能在「歐盟市場」上架，但尚無瀏覽器替換引擎  
   _# 首先，市場局限不符成本 (全球開放比較有動機)；再來，開發者幹嘛為了蘋果，從頭再做一次？_  
* iOS 系統限制，無法與 Tor 生態系完整相容，削弱安全性 (再買蘋果啊！)  
* 僅 iOS 可取得  

其餘優缺點大致和 Tor 相同，畢竟只是不同平台上的替代品  

#### [Cromite](https://github.com/uazo/cromite)  
基於 Chromium，但社群魔改成保障隱私的瀏覽器  
開源、拔除遙測、內建修改版 Adblock Plus，也和 uBlock Origin 相容  
有網路指紋防護，可說是除了 Brave 外少數能用的 Chromium 瀏覽器  
在 Windows、Android、Linux 系統都能用，蘋果系列請去怪 Apple  

缺點：  
* iOS、MacOS 不支援  
* 未上架 Google Play  
   不和 Google 生態系妥協，或許算優點  
   可從[官方釋出](https://github.com/uazo/cromite#releases)下載，Android 用戶可至[開源程式商店](./deGoogle-appStore.md) [F-droid](https://f-droid.org/) 下載  
* 沒預載 uBlock Origin，需手動安裝  

習慣 Chromium 生態系，一樣能取回隱私  

#### [Firefox Focus](https://www.firefox.com/en-US/browsers/mobile/focus/)  
專注版 Firefox 是 Moziila 推出、給行動裝置的瀏覽器  
沒預裝 uBlock Origin，但有內建較弱的追蹤器攔截器  
從前 Firefox Focus 有 Mozilla 遙測，2024 才移除了預設遙測 (但似乎沒特別[說明](https://www.techzine.eu/news/privacy-compliance/123726/mozilla-removes-telemetry-service-adjust-from-mobile-firefox-versions/))  
_# 不過 Mozilla 會不會又置入遙測，無法保證_  
預設就是無痕模式，關閉視窗即刪光歷程記錄、cookie  
也提供一鍵清除歷程、cookie 功能，不一定要靠關閉 app 達成  
有個其他競品缺少的特色 - 指紋解鎖瀏覽器  
且在 stealth mode 下，切換 app 時會屏蔽瀏覽器畫面  
~~避免不小心曝光你見不得人的秘密~~，可提供多一層保護  
有趣的是，Firefox focus 本身可作追蹤器攔截器，安裝到 Safari 當外掛  
_# 有點納悶此功能，直接用 Firefox focus 不就好了？_  
缺點：  
* 發行者為美國公司 Moziila，儘管開源，但說不定又會搞遙測或其他手段  
   Mozilla 是個基金會，但也成立了同名公司  
   每年近 9 成營收來自「預設 Google 為搜尋引擎」，獲得的廣告分潤 (參見 Mozilla 每年財報)  
   _# 受制於 Google，若哪天被以「不續約」要挾，Mozilla 是否挺得住呢？_  
* 續上，預設搜尋引擎為 Google (但可手動更換，替換選項參考[這篇](./deGoogle-search-engine.md))  
* 未預裝 uBlock Origin  
   _# 畢竟若廣告被擋光，就沒分潤啦！_  
* 只有手機版  
* [網路指紋防護](https://www.bitestring.com/posts/2023-03-19-web-fingerprinting-is-worse-than-I-thought.html)、隱私保障不若前幾者  

#### [Firefox](https://www.firefox.com/)  
想必很多人聽過，就是大名鼎鼎的[火狐](https://www.firefox.com/zh-TW/)瀏覽器嘍！  
Mozilla 直接維運，更新最快、都是第一手，還有 Firefox Labs 測試功能可玩  
_# 有個測試功能是，側邊欄 AI 聊天介面，串接主流 LLM 供應商  
~~從前還有開源的 HuggingChat~~，但那已無預警停止服務了，復活之後很不一樣  
復刻版對隱私不那麼保障，功能也差強人意_  

---

講古 (可略)：  
從前瀏覽器由微軟 Internet Explore (IE)，和 Netscape Navigator (網景領航員)二分天下  
網景領航員功能更完善、使用者體驗較好 (網景工程師很強，發明 JavaScript 甚至只花兩週)  
_# 順帶一提，JS 發明人曾任 Mozilla CEO，也是 Brave 創辦人_  
微軟眼見打不贏，就出[奧步](https://www.justice.gov/atr/file/705246/dl)把 IE 綁成 Windows 預設瀏覽器  
許多人沒花工夫查其他選擇，就固著於 IE，使其市占率大增、網景因此倒閉  
之後，在網景為首的企業[舉發](https://www.computerworld.com/article/1362658/update-netscape-sues-microsoft-over-browser.html)下，美國司法部協同 20 個州的檢察長，向微軟發起[反壟斷訴訟](https://www.theringer.com/2018/05/18/tech/microsoft-antitrust-lawsuit-netscape-internet-explorer-20-years)  
最後當然是微軟敗訴，需調整商業模式但逃過公司拆分  
網景的律師也很行，微軟最後支付鉅額達成和解 (付給網景母公司，AOL 時代華納)  

講這幹嘛呢？  

網景歷經收購、重組等波折，核心成員在捐助下，組成 Mozilla 基金會 (很眼熟吧！)  
_# Mozilla 是 Navigator 的內部代號_  
他們開源 Netscape Navigator，並著手改寫  
換 Gecko 引擎後，釋出 Phoenix/Firebird，之後改名 Firefox  
_# 他們也釋出 Minotaur，即後來的 Thunderbird_  
Firefox 從此就變社群導向的開源專案囉！  

---

火狐開源、高度可自訂、附帶截圖功能、支援各大平台  
且從前為人詬病的速度，也在幾次[引擎大改](https://blog.mozilla.org/en/mozilla/introducing-firefox-quantum/)後巨幅提升  
甚至因為沒 Google 那坨追蹤器、臃腫程式，有時還更快  
相較 Chrome，許多網站的廣告也會被攔阻 (但效果有限)  
相對省記憶體，純效能考量不再輸光  
Firefox 系列都內建「開源 PDF 編輯器」，超方便的  
缺點：  
* Mozilla 直營，有[恐怖遙測](https://discussion.fedoraproject.org/t/why-is-mozilla-firefox-built-with-telemetry-reporting-explicity-enabled/146466)、置入功能  
* 預設搜尋引擎是 Google  
* 沒擋網路指紋  
* 沒預裝 uBlock Origin  
* 想要無痕體驗，需自行開啟隱私瀏覽  

好處是，若有興趣鑽研，多數缺點都能手動排除  
關閉遙測、隱藏置入、開啟網路指紋防護、設定總是開無痕、其他安全措施...  
全都可透過[設定檔](https://support.mozilla.org/en-US/kb/about-config-editor-firefox)調整 (在網址列輸入 `about:config `即可進入修改)  
_# Firefox 系列，都能用 `about:config` 修改設定_  
uBlock Origin 也手動安裝即可  
若是自用電腦，可以魔改成喜歡的樣子  
但在外想「開箱即用」的話，就不是那麼方便  

---

#### 懶人包  
依需求推薦：  
* 想要所有平台體驗近似，且只要一個瀏覽器 → [Brave](https://brave.com/) / [Waterfox](https://www.waterfox.net/) / [Cromite](https://github.com/uazo/cromite)  
* 喜歡高度客製化  
   * 電腦版 → [Floorp](https://floorp.app/) / [Zen](https://zen-browser.app/)  
   * 手機 [Waterfox](https://www.waterfox.net/) / [Firefox](https://www.firefox.com/) ([focus](https://www.firefox.com/browsers/mobile/focus/))  
* 倡議者、人權記者 → 不用說，就是 [Tor](https://www.torproject.org/download/)  
* 偏激隱私仔 (例如我)：  
   各瀏覽器有不同優勢，沒規定只能選一個  
   **許多開發者會裝 4、5 個瀏覽器**，區隔不同用途  
   例如平時習慣 [Floorp](https://floorp.app/)、預設開啟網頁用 [LibreWolf](https://librewolf.net/) / [Mullvad](https://mullvad.net/en/browser)、裝 [Brave](https://brave.com/) 使用 Chromium 功能、為非作歹高隱私需求活動用 [Tor](https://www.torproject.org/download/)...  
   至於行動裝置，選擇較少更要精打細算 ([Brave](https://brave.com/) / [Waterfox](https://www.waterfox.net/) / [Tor](https://www.torproject.org/download/) / [Cromite](https://github.com/uazo/cromite))  

---

#### 漏網之魚 or 遺珠之憾？  
有些人可能好奇，不是有一堆「號稱」重隱私的瀏覽器，如 Vivaldi、Puffin、DuckDuckGo、Pale Moon、IceCat、SeaMonkey、Hyphanet 嗎？  
一個個來：  
* Vivaldi  
   * 建構在 Chromium 上，只有 Chromium 開源，其餘非開源  
   * 官方說[會跟進 Manifest V3](https://vivaldi.com/blog/manifest-v3-update-vivaldi-is-future-proofed-with-its-built-in-functionality/)，不再支援 uBlock Origin、推銷自家廣告攔截器  
      攔廣告只是順路，和最強追蹤器攔截器不相容便不予考慮  
   * 而且月曆、郵件、高度客製化功能，都會讓瀏覽器變臃腫、增加網路指紋識別度  
   * 雖然沒到侵犯隱私，但非開源、保護不那麼完善，就不特地推薦  
* Puffin  
   * 雖然是台灣人創立的公司 (CloudMosa)，但程式碼不開源，出局  
* DuckDuckGo  
* 美國公司**閉源**產品，慢走不送  
* 重點是 DuckDuckGo 瀏覽器曾[開後門給微軟](https://www.bleepingcomputer.com/news/security/duckduckgo-browser-allows-microsoft-trackers-due-to-search-agreement/)，隱私保障顯然[非第一順位](https://www.wired.com/story/duckduckgo-microsoft-twitter-ft-bush-assassination-whatsapp/)  
   用非開源的產品，就得盲目信任對方  
   若對方已踐踏過信任，更不值得考慮  
* [Pale Moon](https://www.palemoon.org/)  
   這值得細講  
   Pale Moon 是非 Firefox、非 Chromium，少數還活著的獨立瀏覽器  
   支援電腦版、有持續維護、開源，甚至有可攜版 (不必安裝)  
   但設計非常過時，也和 Firefox、Chromium 的外掛不相容  
   [有人實測](https://www.reddit.com/r/browsers/comments/18wj96a/i_tried_pale_moon_because_ugemmaugr_keeps/)過，有興趣可參考  
   該用戶指出，可找到「過時」版的 uBlock Origin，但點擊後會跳到程式碼倉庫，不會自動安裝  
   而官方提供的攔截器，又形同失能  
   若有舊電腦、喜歡懷舊風的，去玩玩無妨  
   但最後幾點對隱私保障不足，因此本篇不介紹  
* [IceCat](https://www.gnu.org/software/gnuzilla/)  
   一言難盡，IceCat 又稱 GNU IceCat，是 GNU 開源基金會從 Firefox 改來的  
   當年有做出許多保障隱私的調整，程式碼也全開源  
   支援各[電腦平台](https://icecatbrowser.org/download.html)，不過[更新速度](https://gitlab.trisquel.org/ruben/icecat/-/tree/102.5.0)是以年計  
   更新可以稍慢，但「年」有點夸張  
   漏洞修補一天都嫌久，何況是月、年？  
   一年中，瀏覽器總有許多漏洞被發現、修補，而沒修補的就很容易被利用  
   _# 資安界稱「零日漏洞」 (zero day vulnerability)_  
   安全性不理想，所以不列入  
* [SeaMonkey](https://www.seamonkey-project.org/)  
   別誤會，那是指豐年蝦，不是海裡的猴子  
   SeaMonkey 不只是瀏覽器，而是 all-in-one 的瀏覽器-email-HTML 編輯器-IRC 即時通訊-網頁開發工具組  
   是社群開發者將當初網景的統合工具組，撿回來再開發而成  
   不介紹是因為：  
   * uBlock Origin 相容性問題 (僅支援舊版)  
   * [研究](https://cseweb.ucsd.edu/~kmowery/papers/js-fingerprinting.pdf)說明，網路指紋 100% 可被辨識  
   * 更新慢，約莫半年一次  
   _# 莫忘零日漏洞_  
* [Hyphanet](https://www.hyphanet.org/index.html)  
   Hyphanet 是對等網路 (peer-to-peer, p2p)，使用者直接對使用者，不經第三方審查  
   由分散式節點構成、社群開發者自主維運，和 Tor 類似  

   聽起來很棒，為什麼沒介紹？  

   因為嚴格來說，它不是個瀏覽器，而是連結此網路的軟體  
   非瀏覽器，自然不在範疇內囉！  
   有興趣者仍可[下載](https://www.hyphanet.org/pages/download.html)，但有點技術門檻  
   _# 特別提它是因為，Tuta [介紹瀏覽器的文章](https://tuta.com/blog/best-private-browsers)有寫到_  

---

除了開箱即用者，許多瀏覽器都能手動硬化 (外國社群稱 hardening)，調成相對高隱私  
下載瀏覽器後，不妨進入設定逛逛，按自己喜好訂製專屬款！  
_# 圖形化設定介面，或 `about:config` (chromium 系列則是 `flags`)都可嘗試_  

