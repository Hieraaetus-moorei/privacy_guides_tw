# deMeta - 替換臉書 (和小紅書)

> 按讚粉絲團、標兩個朋友，就有小禮物喔！

老派行銷很愛這招，但你的資訊也會因此暴露
Meta 可推知你當時位置、有興趣的東西、在參加的活動...
有位朋友曾說：
> 我這輩子最討厭的事，就是別人叫我用臉書打卡
 
 看完 Meta 的黑歷史，或許你會心有戚戚焉

### 先上圖，再來細數罪狀
[deMeta Macroblog](image link)
^FOSS^ ^指免費開源軟體^ ^(^^Free^ ^and^ ^Open^ ^Source^ ^Software^^)^
^non-profit^ ^指「不以營利為目的」^
^End-to-end^ ^encrypted^ ^chat^ ^指私訊有端對端加密^

### 非換不可
#### 非死不可 (臉書 aka FB = Facebook)
Facebook 經公司重整，母集團變成 Meta
不過重整前後，都有許多**惡質**操作
_# 沒錯就是惡質，看下去就知道_
最知名的莫過於[劍橋分析](https://www.wired.com/gallery/cambridge-analytica-explainer/)案：
    2015 年開始，[劍橋分析](https://www.theguardian.com/news/2018/mar/17/cambridge-analytica-facebook-influence-us-election)和 Facebook 合作
    在用戶「不知情」的情況下蒐集個資，並用於政治廣告投放
    至 2018 年被吹哨者踢爆時，約有 8700 萬人受害
    且該事件被認為，可能影響 2016 美國大選、英國脫歐結果
    想當然爾[被罰](https://www.bbc.com/news/technology-45976300)了，但付出[巨額代價](https://www.bbc.com/news/technology-64075067)下，官方態度如何呢？
    Facebook 可[不認錯](https://www.bbc.com/news/technology-64075067)，還[宣稱](https://www.reuters.com/legal/government/facebook-must-face-dc-attorney-generals-lawsuit-tied-cambridge-analytica-scandal-2025-07-31/)已明確讓用戶知情
    跟創辦人祖克柏[不同調](https://www.brennancenter.org/our-work/analysis-opinion/facebooks-data-mishap-and-case-regulation)，顯然投資人比道德和用戶重要

再來就是個資掌握
Facebook 的[資料](https://proton.me/blog/facebook-data-privacy-revelation)，除了用戶自行提供外，還有第三方來源
例如許多網站使用 [Pixel Inspector](https://themarkup.org/show-your-work/2022/04/28/how-we-built-a-meta-pixel-inspector)，或其他 Meta 追蹤器
你可能想：「好吧！頂多是 Meta、美國政府拿到我的個資，很糟嗎？」
別傻了，**Meta 拿到就是全世界都知道**
Meta 的工程師[說](https://www.documentcloud.org/documents/21716382-facebook-data-lineage-internal-document/)，連他們也無法掌握所有資料流向
其中有段覆水難收的[比喻](https://www.vice.com/en/article/facebook-doesnt-know-what-it-does-with-your-data-or-where-it-goes/)：
> 想像你拿一罐墨水，裡面有第一方、第三方、機敏資料...。你把墨水倒進湖中，它會四處流竄...。你如何能收回傾覆的墨色？如何能確保，它只會流到被允許的位置？

鞭辟入裏，不愧是 Facebook 內部員工，很清楚公司搞了什麼勾當
你提供給 Facebook 的資料，可能被官方、廣告合作商、大概還有美國政府取用
至於第三方怎麼用、是否散佈、有無多重轉售，恐怕無人知曉

不介意個人化廣告，就沒關係了對吧？

不是喔，不是這樣的喔！
前陣子 Meta 被[踢爆](https://proton.me/blog/meta-scam-ads)，高達 10% 的收入來自詐騙、不法事業或違禁品廣告
_# 直接詐騙、無牌網路博弈、色情、違禁醫療用品都有_
不只臉書，[旗下產品](https://www.bnext.com.tw/article/85542/meta-china-ads-anti-fraud-cut)都沒能倖免
來看看路透社的[報導](https://www.reuters.com/investigations/meta-is-earning-fortune-deluge-fraudulent-ads-documents-show-2025-11-06/) (各方幾乎都引用該文)：
* 2024 年的收益，超過 10% 來自詐騙、違法業務的廣告
    10% 是什麼概念呢？ 
    那可是 160 億美元，足夠全資買下華航 30 幾次
* 系統判斷 95% 以上機率可能是詐騙、不法的內容，照樣給刊
    是的，他們**有發現**問題
    但比起趕走金主，他們決定大削一筆：向灰色廣告投放者收更多錢
    Meta 號稱此為「金融懲罰」，用以降低不法廣告投放率
    結果變成「有錢就能刊」，何況詐騙所得之高，多付點錢登廣告不成阻礙
* 即使多名用戶檢舉，不處理還是不處理
    Meta 內部統計，每週有十萬個「有效回報」指出問題
    但公司不是忽略、就是拒絕，96% 的回報都石沉大海
    還有用戶帳號被盜，且冒名者開始向他親友行騙，不斷回報都被 Meta 擱置
    直到巨額損失出現後，替身帳號才被處置

路透報導來自 Meta 內部文件、後續採訪，足以反映公司長期態度
_# 還有內部人員說，在 Meta 刊詐騙廣告比登到 Google 容易多了_
用戶不重要，錢才是關鍵，不論合法與否
甚至把處理劣質廣告的部門裁光了，顯然對 Meta 來說這不太重要
還相信 Meta 是良心企業的，不如相信我是外星人 (？)

再來就是帳號安全性問題
你的帳號不是你的帳號，是 Meta 的帳號
和 [Threads](https://www.dcard.tw/f/talk/p/259668996) 一樣，Facebook 三不五時刪文、[禁言](https://vocus.cc/article/614c8f37fd897800018bbf57)、封帳
社團大規模[滅絕](https://www.nownews.com/news/6699567)，連[企業帳號](https://www.ireland-live.ie/news/carlow-live/1943078/we-lost-business-carlow-woman-hits-out-at-meta-for-disabling-business-accounts.html)也沒能倖免
[理由](https://www.dcard.tw/f/talk/p/257537402)千奇百怪，最常見的莫過於「[性化兒童](https://www.cbc.ca/news/canada/funktasy-meta-ban-9.6932525)」
但當事人什麼也沒做，甚至是公開的營銷、[慈善](https://www.bbc.com/news/articles/cz6nyzvge79o)帳號
常見的救濟手段，是拍身分證、臉照驗證你是真實用戶
_# 那可是超敏感的個資，尤其 Meta 善於外洩，誰敢交付？_
重點是送出機敏個資後，**不見得會有回應、解封**
想找客服，除非你是商業帳號 i.e. 付錢，不然求神拜佛比較實際

帳號被祖，再辦一個不就行了？

如果你只潛水，確實另創新帳、加回朋友即可
但許多人存放家族遊玩影像，互動文章、影片也都在上面
珍貴的記憶，沒備份就再也回不來了
何況商家帳號，短暫下架即可能錯過生意
還有個大問題：
若你在其他網站，曾按下「以 Facebook 連動登入」
則臉書被祖，代表失去一堆下游帳號

夠慘了嗎？
好戲還在後頭

從前美國國安局的 [PRISM 監聽醜聞](https://www.theguardian.com/world/2013/jun/06/us-tech-giants-nsa-data)，Facebook 也沒缺席
和 [Google](https://www.theguardian.com/world/2013/jun/07/google-facebook-prism-surveillance-program)、[蘋果](https://www.theguardian.com/world/2013/jun/07/prism-tech-giants-shock-nsa-data-mining)一樣，[祖克柏否認](https://www.cnet.com/tech/services-and-software/facebook-ceo-denies-knowledge-of-nsas-prism-program/)捲入稜鏡監聽計劃
結果只是[玩文字遊戲](https://www.theatlantic.com/technology/2013/06/how-google-and-facebook-cooperated-nsa-and-prism/314459/)，每個都樂於[配合政府](https://www.infosecurity-magazine.com/news/operation-prism-nsa-and-fbi-monitoring-activity/)，用戶才不是他們在乎的事

壞處寫太多，快變成一篇文了，總之不換對不起自己

#### ~~毛語錄~~小紅書 (RedNote)
小紅書 (RedNote)，是中國行吟信息科技旗下的軟體
_# 人家中國公司所以叫「信息」，有意見去找它_
結合影音、相片和文章，是多功能社群平台
中國、台灣、馬來西亞華人，月活躍用戶約三億
美國則有[一億七千多萬](https://proton.me/blog/tiktok-ban-rednote-privacy-concerns)用戶，不少來自抖音難民
使用者以[**年輕女性**](https://apnews.com/article/china-xiaohongshu-tiktok-ban-refugees-c7f440803128ef50f0ade44d16068f01)居多，常拿來查日用品、旅遊、美妝等相關資訊

看起來很正常，有問題嗎？
問題可大了！

* 多倫多大學公民實驗室[發現](https://citizenlab.ca/research/network-security-issues-in-rednote/)，小紅書上的影音、圖文等內容，用 **http 明文傳遞**
    代表共用網路者、電信商、政府等，都能自由取得你傳輸的資訊
    _# 你用學校或咖啡廳免費 Wi-Fi，就會有其他人共用網路_
    門戶洞開的程度，已不是「漏洞」等級了
    「洞」代表結構有缺陷，這連結構都沒有
    形同住宅沒牆壁，誰想看都行
    使用 http 實作，不太可能是無心之過
    現代網站已預設 https，經加密才傳輸內容
    看看瀏覽器網址列，有個鎖頭標誌代表 https
    若不慎進到 http 網站，瀏覽器還會跳警告
    小紅書捨棄現代標準，跑去用舊時代的做法，動機不明
* 中國線上服務，要求全網實名制
    這是中國法規，至少國內有要求 (其他線上服務亦同)
    外國人有機會被抽到實名[驗證](https://www.reddit.com/r/rednote/comments/1oh2jme/why_did_rednote_make_itself_so_accessible_to/)，沒驗證可能無法使用特定功能
    _# 和台灣社群平台 Dcard 有異曲同工之妙_
    牆內用戶要求臉照 + 身分證，外國人則給護照號碼
    對國外的政策似乎常常改，時緊時鬆所以你也許遇不到
    海外新戶註冊相對容易，門號驗證即可
    也能綁定 Apple、微信註冊
    _# 上述代表小紅書、[中國政府](./chinese-service-risk.md)會有你的門號，甚至身分證、護照等個資_
    就算無視對岸掌握情資的風險，任何機構蒐集過多個資，就有機會外洩
    2025 中國就發生，世上最大的單一來源[個資外洩](https://spycloud.com/blog/inside-the-chinese-data-leak/)
    40 **億**筆外洩紀錄，包含身分證號、信用卡資訊、住址、門號、出生年月日...
    你能想到的機敏資訊幾乎都有，涵蓋銀行、微信、就業單位等各種來源
    集中化的資料庫，很可能是用於管控、[監聽](https://cybernews.com/security/chinese-data-leak-billiones-records-exposed/)人民，只是剛好出意外
    老話一句，不該蒐集的個資，就不要蒐集
    沒蒐集就不會外洩，被威脅也沒東西可交
* 電子前鋒基金會 (EFF)[調查](https://www.eff.org/deeplinks/2025/02/crimson-memo-analyzing-privacy-impact-xiaohongshu-aka-red-note)，同樣指出諸多缺陷：
    * 小紅書確實用 http 傳資料，獨立驗證公民實驗室結果
    * 索取過多權限，尤其「背景執行時的手機位置」
        意思是就算沒在滑，小紅書仍會回傳你的地點 (連 Meta 都沒那麼誇張)
        其他如月曆、聯絡人、手機檔案同樣都[要求](https://reports.exodus-privacy.eu.org/en/reports/560194/)讀寫權限
    * 除了背後的行吟、中國政府，小紅書還會和：
        * 字節跳動 (抖音母公司)
        * 騰訊
        * Facebook
        * Google
            等多家公司共享用戶個資，別以為選中資就能脫離美國巨頭
    * 沒上膛的槍
        Android 版用 [APK patch](https://github.com/sisong/ApkDiffPatch)，可繞過 Google Play 安全掃描直接更新程式碼
        意思是少了把關者，官方能偷偷注入惡意程式碼、追蹤器 
        當然，他們不一定會那麼做，但誰能保證不被濫用呢？
        APK patch 原本用意是更新，卻可用於注入攻擊 (injection attack)
        就像一把沒上膛的槍，何時擊發無從得知
* 我國[資安檢測](https://www.cna.com.tw/news/ahel/202512030203.aspx)，15 項指標全數未過，比抖音還危險
    包含蒐集位置、剪貼簿、截圖、過度[要求權限](https://apps.apple.com/us/app/rednote/id741292507)、蒐集生物 (臉部)資訊...

~~看來名字有個「書」字的社群平台，都是大地雷~~

### 替代品來啦！
臉書、小紅書可發長文，也可放多媒體，算全功能部落格 (Macroblog)
替代品就以類似性質者為主，定位比較接近
#### [Friendica](https://friendi.ca/)
語意類似「朋友們的國度」，是聯邦宇宙 (Fediverse)的臉書替代品
本身為[開源](https://github.com/friendica/friendica)、非營利專案，由社群維運
_# Fediverse 介紹請見[這篇](./deMeta-microblog.md#Mastodon)_
簡言之就是路人都能自架服務，且可和相容的社群媒體互動
有點像你可以用臉書帳號，到別人的[推特](./deMeta-microblog.md#Mastodon)、甚至 [Youtube](./deGoogle-video-platform.md) 留言
_# Fediverse 的平台都互通，而 Friendica 和 Hubzilla、Diaspora* 也能通_
Friendica 最初由網景 (Netscape)工程師 [Macgirvin](https://github.com/macgirvin) 發起，後由社群接手推動
_# 網景是 Mozilla 前身，[Firefox](./deGoogle-browser.md#Firefox)、[Thunderbird](./deGoogle-email.md#Thunderbird) 為該機構代表作_
介面和功能與臉書相似，算最直接的開源替代品
用戶可細緻調整身份權限，讓家人、朋友、特定人士、公開訪客看到不同內容
_# 同檔案、連結，但不同人造訪會看到不同東西，~~避免你不堪的家庭秘辛曝光~~_
缺點：
* 有些別人架好的 instance 版本過舊，可能有體驗不佳、漏洞尚存的問題
    找人多、版本有跟上的伺服器註冊，就比較不用擔心
* 私訊「無」端對端加密
    所以私人對話小心點，伺服器擁有者技術上能解碼 (自己架站就不怕)

自由、免費軟體的好處，就是沒商業模式
不會出現廣告、或任何官方推銷

#### [Diaspora*](https://diasporafoundation.org/)
名字意思是人口大外移，劍指 Facebook
[開源](https://github.com/diaspora/diaspora)、非營利，伺服器可自架 (i.e. 去中心化)
從前有四位紐約大學學生，不滿主流社群平台對隱私的侵害
發動目標一萬美元的群眾募資，想開發尊重隱私的替代品
結果募得 20 萬，顯示隱私的價值實為可觀
_# 諷刺的是，有部分還是祖克柏捐的_
Diaspora* 於焉誕生，基本上就是介面不同的 Friendica
但不支援 Fediverse 的 ActivityPub，協議稍嫌封閉
_# 只能通 Friendica 和 [Hubzilla](https://hubzilla.org/page/info/home)，不支援 Mastodon 或其他專案_
功能取名比較特別：
* Pod：公開實例，即其他人架的服務點
    一般稱為 Instance，Diaspora* 比較特立獨行
* Aspects：身份別，即 profile
    和 Friendica 類似，可選讓朋友、家人、外人看到不同身份

因為強調「用戶才是資料擁有者」，所以上傳的影音都能再下載
而且不要求真實身份，你愛用化名就用
缺點：
* 相較其他 Fediverse 專案，生態系較封閉
    但還是比臉書那類「中心化」者，要開放、民主得多
* 私訊**無**端對端加密

發文可用 Markdown，創作很方便
開發由 Diaspora* 基金會負責，沒商業模式 (硬要說就是群眾捐助)

#### [Movim](https://movim.eu/)
在上一篇[換 Threads](./deMeta-microblog.md) 提過
因為有長文、短文模式，同時滿足 macro- 和 micro- blog，就再提一次
是[開源](https://github.com/movim/movim)、免費、社群驅動的專案，在歐洲較活躍
可自架服務，但使用 XMPP 而非 ActivityPub，所以要橋接器才能進入聯邦宇宙
_# 你也可以不進聯邦宇宙，在不同 Movim 伺服器互動不受影響_
最大優點是私訊「有」端對端加密，細節可見[前文](./deMeta-microblog.md)
缺點：
* 旗艦伺服器在歐洲，選它可能會有點延遲
    _# 你也可以選其他伺服器，享受「分散式」的好處_
* XMPP 和 Fediverse 未直接互通

不過 XMPP 也有一票粉絲，可算偏門生態系

#### [GoToSocial](https://gotosocial.org/)
上次也[介紹過](./deMeta-microblog.md)，就是欠自架的 Fediverse 開源專案
架站所需資源甚少，是設計給朋友圈自己玩沙用的
不過因為是聯邦宇宙，你也可以從此出發到~~更遙遠的彼方~~其他服務，例如 Mastodon
缺點：
* 需自行架設服務
* 仍在 beta 測試，可能遇到功能不穩
* 只有後端
    不過可和第三方前端互通，意思是別人幫你把 app 寫好了
* mp4 的 metadata 尚無法自動清除 (其他圖像都可)
* 私訊**無**端對端加密

有長短文模式，符合臉書 macroblog 性質

#### [Minds](https://www.minds.com/)
美國人創立的去中心化平台，[開源](https://github.com/minds)、演算法透明、且無個人化廣告
建構在以太坊區塊鏈上，[起初](https://wefunder.com/minds)用 Nostr 協議，後來也支援 ActivityPub
_# 就是能通 Fediverse 啦！_
演算法基本上就是時序倒排，越新的能見度越高
伺服器可自架、容許匿名註冊、承諾[不賣](https://thinkbiganalytics.com/minds)用戶個資
私訊端對端加密，隱私保障相對完整
相較其他區塊鏈的「絕對自由」機制，Minds 有輕度內容審查
若內容被舉報，系統會隨機挑 12 位用戶評選，75% 以上反對才會推翻原決定
不過恐怖主義、造假內容、惡意攻擊等， Minds 管理員有權直接 ban 用戶、內容
雖然可善盡管理，但也存在極權隱憂
_# 只要有極權後門，哪天就能亂祖人_
最特別之處，莫過於商業模式：
* 互動即可賺取虛擬貨幣
    有點像之前介紹過的[奧德視](./deGoogle-video-platform.md#odysee)，算一種鼓勵內容創作、用戶參與的機制
* 對等 (peer-to-peer)廣告
    此非個人化廣告、也不是傳統行銷，而是用戶能花代幣增加貼文聲量
    「花錢 (虛擬貨幣)增加曝光量」，有點廣告的意味
* 訂閱費
    用戶可訂閱 Minds plus、Pro，享有更多[特權](https://www.minds.com/about/plus)
    E.g. 築付費牆、出金 (換代幣成法幣)、宣傳粉絲頁等
    Pro 有點貴，每月 50 美金或每年 480 美金
* 付費牆的收益抽成

畢竟 Minds 是「營利事業」，所以有商業模式

缺點：
* 美國企業，受制美國法律
    有金流、管理員特權，就容易被政府操弄
    若遇到稜鏡計畫或類似監聽法案，結果恐怕和 Facebook 相去不遠
* 免費戶最長上傳 20 分鐘影片，且儲存期限 30 天
* 加密機制安全性問題
    Minds 加密強度[低於](https://www.vice.com/en/article/that-social-network-app-backed-by-anonymous-uses-weak-encryption/)業界標準，雖非直接代表漏洞，但防護較薄弱
    且用戶端程式會盲目接收金鑰，若伺服器被掌控 / 惡意操作，用戶端風險較高
    I.e. 你得信任伺服器，但上面提過站方有很高權限，設計上不太安全
    開源本該是「做好詳盡防護，並讓大家抓漏」
    但 Minds 比較像「設計亂糟糟，直接端出來給駭客鑽」

雖然漏洞補了不少，但是否要進場最好審慎評估

原本還想介紹 Steemit，但起初是美企、後來被中國裔幣圈巨頭收購
fork 又有資安問題，不太值得推薦

<br/>

---

<br/>

### 懶人包
* 一般用戶，只想平行移轉：
    * 喜歡 Fediverse → [Friendica](https://friendi.ca/)
    * 接受隔牆加入 Fediverse → [Diaspora*](https://diasporafoundation.org/)
    * 不介意美企、有商業模式 → [Minds](https://www.minds.com/)
    * 想要端對端加密私訊 → [Movim](https://movim.eu/)
* 開發者，想自行架站：
    * 只想跟小圈圈玩沙 → [GoToSocial](https://gotosocial.org/)
    * 想架完整站點：
        * 喜歡 Fediverse → [Friendica](https://friendi.ca/)  / [Minds](https://www.minds.com/)
        * 搭橋加 Fediverse → [Diaspora*](https://diasporafoundation.org/)
        * 想要端對端加密私訊 → [Movim](https://movim.eu/) / [Minds](https://www.minds.com/)

<br/>

---

<br/>

本篇多以社群為主，對於想專心寫文的人來說，或許不那麼切合
_# 不過若你接受在臉書上撰文，那些絕對夠用_



