# 安全的通訊軟體 - 替換 Line、Discord

> 他們公司用 Line？這樣資安不會有問題嗎？

之前某助理曾言，諷刺的是他自己公司用 Telegram，另一個稱不上安全的東西

<br/>

這次結論先行

### 看圖最快
[deMeta WhatsApp](image link)
^FOSS^ ^指免費開源軟體^
^non-profit^ ^指「不以營利為目的」^
^最下排是^ ^Discord^ ^替代品^

該換的有：
* Facebook / IG Messenger
* Line
* 微信 (WeChat)
* WhatsApp
* Telegram (TG)
* Snapchat
* Discord
* QQ

### 懶人包
#### 安全替代品
* 想要跨裝置同步：
    * 需要網路匿名性 → [Session](https://getsession.org/)
    * 不接受閉源組件 → [Delta Chat](https://delta.chat/)
* 可為匿名、安全性犧牲部分功能 → [SimpleX Chat](https://simplex.chat/)
* 一般用戶，不想管技術、能接受中心化服務
    * 願意門號辦帳 → [Signal](https://signal.org/) / [Molly](https://molly.im/) (Android 用戶)
    * Email 辦帳號 → [Wire](https://wire.com/) (所有平台都支援，包括瀏覽器)
    * 人權記者、有人身安全疑慮、所在地可能無網路 → [Briar](https://briarproject.org/)
* 替代 Discord：
    * 安全性優先，功能其次
        * 大群聊天 → [Element](https://element.io/) / [Wire](https://wire.com/)
            想替代 Slack 的企業，也可以考慮 [Wire](https://wire.com/)
        * 私訊用途 → [FluffyChat](https://fluffychat.im/)

    _# [FluffyChat](https://fluffychat.im/)、[Element](https://element.io/) 可互換，只是介面和功能針對不同用途優化_
    * 看重功能，甘冒風險 → [Stoat](https://stoat.chat/)

<br/>

---

<br/>

### 為什麼該換
因為主流服務都很不尊重隱私，你極有可能也中標了
**挑自己「以為很尊重隱私」的看就行，求知若渴者再全部細讀**
_# 如果已決心要換，跳過本段落無妨_

#### Facebook (和 IG)Messenger
Facebook Messenger aka 臉書私訊，會[掃描](https://www.bloomberg.com/news/articles/2018-04-04/facebook-scans-what-you-send-to-other-people-on-messenger-app)用戶傳的每個連結、圖片
還會搜集：健康、經濟、聯絡人、地點、機敏個資... (官方自己說的)
[FB messenger 在 AppStore 宣稱會拿的個資](messenger-app-data-collection.png)
從前甚至[分享語音給第三方](https://www.phonearena.com/news/Facebook-voice-chats-transcribed-by-contractors_id118198)，靠人力聽取內容
這應該能解釋為何 2014 年起，手機上 FB 私訊只能從 app 使用
_# 因為應用程式能深入裝置、取得更多權限，以及機敏個資_
IG 私訊大同小異，且 2026 三月**停掉**端對端加密
_# FB 因太少人用端對端加密，故預設開啟；IG 同樣太少人用，所以拿掉；標準何在？_
官方重獲訊息內容監控權，直接掃描每則來往文字、多媒體
_# 不過 IG 端對端加密預設關閉、深藏在設定裡，多數人大概原本就沒開_
加上 Meta 過往不怎麼光彩，實在不值得信任：
* 縱容造假、詐騙猖獗 (e.g. 2024 收益，[超過一成](https://www.reuters.com/investigations/meta-is-earning-fortune-deluge-fraudulent-ads-documents-show-2025-11-06/)來自不法事業廣告)
    _# 而且官方已知那些內容，95% 以上是有問題的喔！_
* [偷開 app 相機](https://www.cnet.com/tech/mobile/lawsuit-accuses-instagram-of-peeping-with-iphone-camera/)
* 和第三方[分享](https://proton.me/blog/facebook-data-privacy-revelation)用戶個資
* 配合政府[監聽](https://www.theguardian.com/world/2013/jun/06/us-tech-giants-nsa-data)用戶
* [亂祖](https://www.nownews.com/news/6699567)帳號
* ...

爭議過多，有興趣可見[前文](./deMeta-macroblog.md)
Meta 每隔一陣子就會搞事，說不定你讀本篇時又有新黑料
多數人應該都知道，Meta 是偷窺狂
所以還選擇繼續用、甚至下載 app 的人，不是暴露癖、暴露慾就是暴露狂

### WhatsApp
WhatsApp 可說是歐美、印度的 Line，盛行率高、許多機構也用來創官方群
但 Facebook 在 2014 年就買下 WhatsApp 了，隱私也因此[成為妄想](https://proton.me/blog/whatsapp-new-privacy-policy)
來看看[官方說法](https://www.whatsapp.com/legal/privacy-policy)，拿的個資可多了
* 門號 (註冊要手機號碼)
* 和誰通聯、多頻繁互聊 (i.e. 訊息的 metadata)
* 何時用、用多久
* 你的所在地
* 裝置資訊，例如電池電量、訊號強度、IP、語言
* ...
    光前兩點，就夠鎖定你身份了

用途不外乎行銷、配合法規和政府
_# 小提醒，從前[稜鏡計畫](https://www.theverge.com/2013/7/17/4517480/nsa-spying-prism-surveillance-cheat-sheet)也是美國政府主導的喔！_
諷刺的是，Meta 很愛用「隱私」來行銷 WhatsApp，甚至[大言不慚](https://blog.whatsapp.com/setting-the-record-straight)：
> 「尊重你的隱私」刻在我們 DNA 裡，WhatsApp 的目標是「瞭解你越少越好」

![「Meta 尊重隱私」，有看過比這更好笑的笑話嗎？](https://media.tenor.com/eF3Jo97LytMAAAAC/ronald-laugh.gif)

笑話看完，繼續深入
WhatsApp 號稱使用 Signal protocol 做端對端加密
_# 「理論上」只有你和接收者能看到訊息內容，Signal 段落會細說_
如果落實，官方就無法竊聽

那不是很棒嗎？

問題來了，WhatsApp 程式碼不公開、Meta 劣跡又一堆
端對端加密是否有做，口說無憑
2026 年初，Meta 就因「未妥善實作 WhatsApp 端對端加密」，[被告](https://proton.me/blog/whatsapp-encryption-lawsuit)上加州法院
再者，訊息[備份](https://faq.whatsapp.com/481135090640375/?helpref=hc_fnav&cms_platform=android)**無**端對端加密，地端甚至**無加密**
雲端服務商高機率看到內容，若裝置遺失更是毫無保障
_# 雲端備份的端對端加密，得由用戶手動開啟_
壞消息，就算你不備份，資料也可能從他處流出
因為聊天軟體的特性，就是用戶「們」互相通聯
如果聊天對象有做備份，你傳的內容一樣會曝險

[資安](https://proton.me/blog/is-whatsapp-safe)方面更可怕，攻擊面積大、甚至**不修補漏洞**
* [惡意軟體](https://www.ibm.com/think/insights/pixpirate-brazilian-financial-malware)能運用 WhatsApp，傳送、截持機敏資訊
    還能自動下載，並將惡意連結傳給你的聯絡人
* 零點擊漏洞利用 (zero-click exploit)
    對方圖片傳來，就算你不點任何東西一樣會被駭
    [iOS](https://techcrunch.com/2025/08/29/whatsapp-fixes-zero-click-bug-used-to-hack-apple-users-with-spyware/)、[Mac](https://techcrunch.com/2025/08/29/whatsapp-fixes-zero-click-bug-used-to-hack-apple-users-with-spyware/)、和[三星 Android](https://ccb.belgium.be/advisories/warning-critical-vulnerability-samsung-galaxy-android-actively-exploited-install-spyware) 都有受災戶
* 資料可輕易盜取，沒基礎防護機制
    2025 年有[研究](https://arxiv.org/abs/2511.20252)指出，靠流水號暴力窮舉，就能洗出用戶門號
    頭貼、自介、裝置資訊、時間戳，甚至端對端加密公鑰都沒倖免
    研究期間，查詢頻率約每秒 7000 個門號，全程攻擊者 IP 都未遭封阻
    最後得手約 35 億個活躍帳號，幾乎等同全球 WhatsApp 用戶數
    任何一個正常網站，都會設高頻訪問阻擋機制，就算沒設也該有示警、監測異常用量
    這次實驗能成功，就是因為 Meta 沒安全機制
    直到研究員**主動聯繫**，官方才修補速率限制問題
    但遍歷門號這種事，早在 [2012 年](https://www.researchgate.net/publication/230035813_Guess_Who_Is_Texting_You_Evaluating_the_Security_of_Smartphone_Messaging_Applications)就有學者對 WhatsApp 試過了
    _# 2017 也有人[測試 Facebook](https://seclab.skku.edu/wp-content/uploads/2019/09/Kim2017_Chapter_HelloFacebookHereIsTheStalkers.pdf)，連生日、所在地、姓名都能挖到_
    結果十多年來 Meta 都視而不見，放任潛在駭客盜取用戶資訊
    拿到聯繫方式不只能網路釣魚、詐騙，甚至還會造成人身安全威脅
    中國、緬甸、伊朗等禁用 WhatsApp 的國家，官方同樣能洗出電話號碼清冊
    比對國內門號名單，就能抓出誰在偷用「境外反動勢力」的軟體，進而採取行動
    不是太懶、太鬆散，就是不重視用戶權益
    研究員事後會刪資料，但那麼多年來，有多少駭客、政府曾利用此漏洞呢？
    更意外的發現是，端對端加密公鑰和**一次性**事前金鑰 (one-time prekey)被**多次複用**
    one-time prekey 顧名思義，每個 session 都該重新生成
    _# 何況 WhatsApp 號稱用 Signal protocol，理論上**每則訊息**都該生成新的_
    Signal 協定本來會提供 perfect forward secrecy，但 Meta 糟糕的實作毀了它
    _# Perfect forward secrecy 在 Signal 段落會提_

號稱的安全，只是給用戶錯覺
相信 Meta，不如相信祖克柏[蜥蜴人](https://www.reddit.com/r/OutOfTheLoop/comments/8879c9/why_are_people_comparing_mark_zuckerberg_to_a/) (？)

#### Line
東亞地區盛行的通訊軟體，在台灣滲透率超過 90% (台灣用戶約 [2200 萬](https://www.informationsecurity.com.tw/article/article_detail.aspx?aid=12484))
但 Line 的問題可多了，用戶隱私、對資安的態度都令人不敢恭維
先看看 Line [蒐集](https://www.lycorp.co.jp/en/company/privacypolicy/)哪些資料：
* 創帳強制索取門號、email
    在台日港韓辦電話號碼，都需要政府 ID (e.g. 身分證號)
    所以光取得帳號，就已經確立 Line 非匿名、不隱私了
    2026 更因電信商的鬆散資安措施，發生[大規模盜用](https://tw.news.yahoo.com/line%E5%B8%B3%E8%99%9F%E9%9B%86%E9%AB%94%E8%92%B8%E7%99%BC-%E5%85%A8%E5%8F%B0%E9%A9%9A%E5%82%B3line%E5%A4%A7%E8%A6%8F%E6%A8%A1%E7%9B%9C%E7%94%A8%E6%BD%AE%E5%A7%8B%E6%9C%AB-%E6%AC%A1%E7%9C%8B-%E5%85%87%E6%89%8B%E7%AB%9F%E6%98%AF%E5%AE%83-025700640.html)
    你可能說：那是電信商的漏洞，又不是 Line
    沒錯，但不拿門號就沒有這攻擊面，何況 Line 也沒做額外防範
    _# 稍後會提的 Signal 同樣要求門號註冊，但有追加 PIN 保護_
* 通訊錄
* metadata，例如你何時上下線、何時在線
* App 內的一切活動，包括：
    * 你點擊或看了哪些廣告、內容
    * 購買與搜尋紀錄
    * 應用程式內的瀏覽行為
    I.e. 點連結用 Line 開啟網頁，在上面做什麼都會被側錄
    號稱用來改進服務，和**推送廣告**
    _# 想起聊天室頂端的侵入式廣告了嗎？_
* IP
* 裝置種類與名稱

隱私政策說會和第三方合作，蒐集、共享資料，用途卻寫得頗模糊
信任 Line 就算了，來歷不明的第三人也能存取，風險有點高
[[Line 蒐集的個資種類，直追 WhatsApp](https://apps.apple.com/us/app/line/id443904275)](line-app-data-collection.png)

接下來是資安
Line 的端對端加密並非業界標準，而是自行研發的 Letter Sealing protocol
閉源，安全性、加密有效性並不透明
2025 歐洲黑帽 (Black Hat Europe)活動，有學者[分析](https://blackhat.com/eu-25/briefings/schedule/#line-break-cryptanalysis-and-reverse-engineering-of-letter-sealing-49039) Letter Sealing 協議的漏洞：
* 重播攻擊 (replay attack)
    設計上沒紀錄狀態 (stateless)，伺服器能任意重送曾發過的訊息
    例如某次朋友問你：「要不要幫買南投蕉？」
    你說：「好，買啊」
    結果另一次問：「xx股票要買嗎？」，伺服器惡意重送：「好，買啊」
    一樣的話在不同情境說，結果會很不一樣
* 明文洩漏 (plaintext leakage)
    還記得打字時，Line 偶爾會推薦相關 emoji、貼圖嗎？
    問題就在這
    裝置端有字典會比對內容、自動推薦相應表情或圖片
    但當你沒那些貼圖時，Line 會自動向伺服器發送請求
    用**你打的字段**當關鍵字，尋找適當的貼圖推薦資訊

    等等，你打的字段！？

    沒錯，所以明文會被送到伺服器，端對端加密於焉瓦解
    不僅如此，「圖片、連結預覽」功能也是破口
    _# 在 Line 聊天室貼一段網址，會自動顯示網頁預覽_
    你以為預覽縮圖哪來的，當然是由伺服器渲染送回
    因此連結、或長得像連結的字段，都不受端對端加密保護
* 身份冒充攻擊 (impersonation attack)
    這才是最大問題
    在群組中，惡意人士能輕易冒充其他人傳訊給你，且接收者無從分辨發送方真偽
    _# 此處非指「改頭貼、ID」，而是透過伺服器從技術上進行仿冒_
    雖然此「中間人攻擊 (man-in-the-middle attack)」需被害者連到惡意伺服器
    但實務上並不困難，簡單的社交工程 (i.e. 教你操作)、惡意員工、政府操弄...
    有太多方法能達成，用戶根本無從分辨自己連上的伺服器是否良善
    尤其地緣政治因素、台灣的高盛行率，讓對岸更有動機投入伺服器滲透
    若 Line 官方有不肖員工 (insider threat)，一樣能對用戶出手
    何況如果政府要求，站方會為了你不配合政府嗎？
    「端對端加密」初衷就是降低營運者操弄、窺探的風險，Liine 卻與此背道而馳
    依然得無條件信任伺服器，端對端加密的優勢所剩無幾
    為了驗證可行性，學者甚至在 iOS 上成功展演中間人攻擊，並非紙上談兵

那麼，Line 修補漏洞了對吧？

**沒有**。
學者向 LY Corp. (Line 母公司)回報問題後，[官方說](https://www.darkreading.com/application-security/line-messaging-bugs-asian-cyber-espionage)：
> 那些攻擊假設伺服器被滲透... 發生機率很低，情境不切實際，所以**未對此採取行動**

還說這類漏洞是為了功能才「刻意為之」，不考慮升級、修補加密協議
漏洞都已經被利用，還說發生機率不高，出發點令人懷疑
而且既然已知「可能會發生」，難道不該設法防堵？
官方態度明顯不願降低風險，對政府找上門、內部威脅都門戶洞開
這種「假設不會出事」的心態，全然違背資安黃金準則「[零信任](https://vocus.cc/article/68dfe075fd89780001423718)」
不過也不太意外，畢竟會出事的是消費者，公司只管賺錢並不在乎用戶

綜觀過往，會發現 [2021](https://safety.rsf.org/line-a-messaging-app-to-use-with-caution/)、[2023](https://www.cpomagazine.com/cyber-security/data-breach-on-the-largest-japanese-messaging-app-line-leaks-440k-records/) 都發生過外洩事件，台灣 Line Pay 更因此[暫時下線](https://focustaiwan.tw/business/202112070008)
還曾有中國工程師[存取](https://www.reuters.com/article/us-japan-line-access-idUSKBN2B901E/)日本用戶資料的記錄，資安顯然非優先考量
有段時間，[仿冒網站](https://teamt5.org/tw/posts/line-malware-cybersecurity-incident/)甚至在搜尋結果排行更高，用戶因此下載到假 Line
惡意軟體裝進手機，通訊、付費、使用習慣全曝險
還沒完，LY corp. 也樂於配合政府**言論管制**
在[泰國](https://www.bangkokpost.com/life/tech/436370/red-buffalo-sticker-banned)、[印尼](https://www.abc.net.au/news/2016-02-12/indonesia-bans-gay-emojis-on-messaging-apps/7164674)、[中國](https://citizenlab.ca/research/asia-chats-investigating-regionally-based-keyword-censorship-line/)都有先例，儼然亞洲版 Meta
就算~~幻想~~假設公司良善，端對端加密一樣非滴水不漏
群組語音通話、視訊，及 50 人以上群組訊息都[沒](https://www.lycorp.co.jp/en/privacy-security/security/transparency/encryption-report/2024/)端對端加密
被檢舉的訊息，及使用者互動 (對訊息按表情)，同樣不在保護範圍

2026 年，Line 又掀起另一波[爭議](https://www.dcard.tw/f/talk/p/261127578) - 月費 165 台幣的付費版
把眾多[基本功能](https://today.line.me/tw/v3/article/NvGDP0Z)綁進方案，備份空間[少得可憐](https://tw.news.yahoo.com/line%E6%8E%A8%E8%A8%82%E9%96%B1%E5%88%B6%E6%AF%8F%E6%9C%88165%E5%85%83-%E5%9F%BA%E6%9C%AC%E5%8A%9F%E8%83%BD%E9%83%BD%E8%A6%81%E6%94%B6%E8%B2%BB-%E9%81%AD%E7%B6%B2%E5%AB%8C%E7%BF%BB-122906206.html)
別家有的跨裝置備份遲遲不出，其實只是為了收割
從前的訊息備份也很不尊重隱私，Android 綁定 Google drive、iOS 綁 icloud
iCloud 好歹能開進階資料保護 (ADP)，Google 雲端則是[被監控](https://vocus.cc/article/6898d4fafd89780001c44f98)出名的服務

賺錢，對 Line 來說比用戶權益和體驗更重要

#### Snapchat
Snapchat 在[前文](./deMeta-img-and-short.md)詳述過，在此不贅述，有興趣可自行參考

#### WeChat (微信)
我是不知道，重視隱私的人怎麼會選[中國軟體](./chinese-service-risk.md)
註冊微信需要電話號碼，app 又會[蒐集](https://www.mozillafoundation.org/privacynotincluded/wechat/)：
* **精確**位置
* 加速器資訊 (你的移動狀態、姿勢)
* 裝置資訊 (e.g. OS 種類、第幾代，螢幕長寬等)
* Email
* FaceID、付款資訊 (如果使用相關功能)
* IP
* 性別

WeChat 背後是騰訊，國外用戶[言論控制](https://citizenlab.ca/research/tracking-censorship-on-wechat-public-accounts-platform/)較鬆，國內相對嚴格
曾關閉多個平權倡議者帳號，很有中國風格
加拿大公民實驗室做了一系列分析，[發現](https://citizenlab.ca/research/privacy-in-the-wechat-ecosystem-full-report/)：
* WeChat 會索取裝置 IMEI (手機指紋)，及「檔案」、「多媒體」存取權
    那可是連 Google 都說「危險」的權限，能讀檔案幾乎形同剝去手機的內衣
* 用戶授予「微信插件 (mini programme)」權限時，微信本身往往也會同步取用
    **全數**插件 (i.e. 外掛程式)，都會對使用情況做精細的追蹤
    等同裝了一堆追蹤器，且不會告知用戶資料蒐集正在進行
* 微信與微信不同
    看不太懂？很正常
    多數功能，適用 WeChat 隱私政策
    但部分功能則受 Weixin 隱私政策規範
    WeChat 就是微信、微信音譯就是 Weixin，你不是你他不是他
    什麼鬼東西？
    白話說法：微信搞了兩套隱私政策
    通訊軟體 WeChat 一套，另一套則以 Weixin 名義頒布
    Weixin 被視為「第三方」，隱私政策較侵犯、會蒐集更多資訊
    可以「合規」掠奪個資，同時保持 WeChat 雙手乾淨
    _# WeChat 和 Weixin 甚至使用相同伺服器，基本上是同個實體_
    ![WeChat 和 Weixin 與微信的差別](https://media.tenor.com/9C-42Fsr6U8AAAAC/spidey.gif)

此外，WeChat **沒**端對端加密，所以騰訊能看到對話內容
中國政府，當然也行

#### QQ
同樣是騰訊的軟體，「乍看之下」比較隱私友善
[蒐集](https://apps.apple.com/sc/app/qq/id444934666)位置、聯絡人、財經資訊，可用門號或 email 註冊
但同樣**沒**端對端加密，且**有「主動惡意行為」**
電腦版 QQ 曾[被發現](https://www.privateinternetaccess.com/blog/tencent-has-been-caught-spying-on-your-web-browsing-history-with-qq-messenger/)，會偷爬瀏覽器歷程記錄
東窗事發官方才藉口「為了帳號安全性而做」，但兩者顯無關聯
平台管理也略顯鬆弛，QQ 的「小世界 (little world)」短片區
因放任色情訊息氾濫、性引誘與招募未成年者，違反《未成年人保護法》被罰
_# 中國官方開罰的，不管理的代價是 [100 萬人民幣](https://dig.watch/updates/china-fines-tencent-for-hosting-explicit-content-on-qqs-little-world-section)_

#### Telegram
簡稱 TG，是俄羅斯人創立的通訊軟體
創辦人提倡言論自由、秘密通訊，因而被當局封殺
支援端對端加密，也不太有言論管控

看起來不錯，也常被推薦當 Line 替代品，問題在哪？

或許比 Line 好一點，但絕對稱不上保護隱私
TG 客戶端開源、伺服器閉源，**註冊需要門號**
會[蒐集](https://apps.apple.com/us/app/telegram-messenger/id686449807)位置、通訊錄、財經資訊、購買相關個資 (如果訂閱)
端對端加密「預設關閉」，且多數使用者並未開啟
_# 人們以為有開，造成安全的錯覺，更危險_
你可能會說：「那我手動開不就好了？」
很遺憾，能獲得的保障有限
Telegram **唯一**有端對端加密之處，就是一對一秘密聊天 (Secret Chats)
其他群組、私訊、公開頻道，都是伺服器加密，i.e. 站方能解鎖、窺探內容
官方聲稱用於同步、備份，但訊息內容也會曝光
_# 再說「端對端加密」和「備份」、「同步」並非互斥，可以都做_
而不論是否端對端加密，訊息都會附帶許多 metadata，e.g. 
* auth_key_id，裝置識別碼 (TG 配發的指紋)
* IP
* 時間戳

重點是那些 metadata 是**明碼**，不受加密保護
[隱私政策](https://telegram.org/privacy)亦言明，會配合執法單位提供資訊
若俄羅斯動用監控法規 SORM，用戶個資很可能不保
何況後端基建由 Global Network Management (GNM)[管理](https://www.occrp.org/en/news/telegram-responds-to-investigation-that-links-its-infrastructure-to-russian-security-services)，GNM 的老闆又曾和俄羅斯聯邦安全局 (FSB)簽監控合約
哪怕 TG 經營者很有良心，難保 GNM 不會配合政府
_# 兩者關係類似「我提供服務，但網頁架在亞馬遜雲端 (AWS)」_
再說 metadata 都沒加密，外界可以自由取用
有了裝置識別碼，就能判定哪些訊息是誰傳的
有 IP，則幾乎可以鎖定身份
有時間戳，可以斷定何時活躍，推斷用戶時區
官方[宣稱](https://www.bbc.com/news/articles/cvglp0xny3eo)「不主動提供」，但有合法要求時，仍會配合交出資料

除了政權風險，隱私政策也說有許多第三方會拿到資料
* 語音訊息轉文字：Google
* 翻譯功能：Google 和微軟

TG 本身也有廣告 (即贊助訊息，Sponsored Messages)
即使官方說不會拿個資推廣告，但廣告商仍可透過頻道主題間接定向
隱私功能也未設成「開箱即用」，下載後得手動調整
否則陌生人能搜尋你、刷出你的門號、發送訊息給你
是否在打字、上線狀態都是公開
所以核心價值並非隱私保障，頂多是相對不侵犯的選擇

再來就是加密問題，這攸關安全性
Telegram 用自己發明的加密協議，[MTProto](https://core.telegram.org/techfaq)
但協議本身和[金鑰交換](https://kclpure.kcl.ac.uk/ws/portalfiles/portal/324396752/main.pdf)、管理、產生方式，[存在](https://eprint.iacr.org/2023/469.pdf)不少脆弱點
一般的傳輸層加密 (TLS)，都還比較安全
在加密領域，現有的協議夠好就不該亂換
因為容易踩前人踩爛的坑，何況既有做法經時間考驗，但新方法沒有
_# 當然，若現有協議存在重大缺失，另闢蹊徑就合理_
MTProto 曾面臨的[漏洞](https://mtpsym.github.io/)：
* 訊息重排攻擊 (message reordering attack)
    攻擊者可以調整訊息順序，例如
    友：要買巧克力嗎？
    你：好
    友：要買黃金嗎？
    你：不用，謝謝
    可以被操作成：「要買巧克力嗎？」→ 不用，謝謝
    「要買黃金嗎？」→ 好
    _# 和 Line 的漏洞有異曲同工之妙_
* 明文復原漏洞 (plaintext recovery)
    客戶端實作中，允許特定情況下恢復部分明文，Android、iOS、桌面平台都不例外
    不過若想達成，需發送百萬則以上訊息，實現難度較高
* 刺激的來啦，中間人攻擊 (attacker-in-the-middle)！
    在初始金鑰協商時，攻擊者有機會冒充伺服器，讓用戶連到惡意後端
    用假的伺服器和你對接，便可操弄、存取你送出的訊息，及你的資料
    不過這得在**分鐘**尺度下，撒數十億則訊息給伺服器，實現難度也很高
    _# 畢竟 TG 和 Meta 不一樣，至少有做基礎防護_
* 時序攻擊 (timing attack)
    明文才有完整性 (integrity)保障
    所以客戶端收到訊息後，必須先解碼才能驗證完整性
    不同長度的訊息，解碼所需時間不同，因此可藉解析時間推斷訊息長度

和 Line 不同的是，研究員告知後，官方就陸續修補漏洞
_# 還提供賞金給研究者，應對方式還算不錯_
但中間人攻擊僅「降低風險」，未完全防堵
這也顯示自研協議的弱點 - 用戶得信任伺服器，同樣違背零信任原則
此外，TG 加密協議、各環節雖然開源，但設計並不「乾淨」
第三方不易稽核，開源的優勢就降低不少
更可能因為過於複雜，修改、補洞時又引入其他漏洞
例如升級成 MTProto 2.0 後，雖然前述問題多已修補，但又冒出[其他風險](https://www.sciencedirect.com/science/article/abs/pii/S0167404822004643)

至少 Telegram 還算誠實，弱項基本上都有說明
「隱私錯覺」主要來自民眾吹捧、以訛傳訛造成誤導
只是加密保護較弱，國家級情報機構仍可能滲透

不過如果是簡單的漏洞利用，就不必勞煩國家機器
早在 2016 年，TG 就踩過和 WhatsApp [一樣的坑](https://www.huntress.com/threat-library/data-breach/telegram-data-breach)
惡意人士用大量門號，從 API 端點洗出存在的用戶與其公開頁面
官方事後做了防堵，但犯案者沒找到

#### Discord
簡稱 DC，[爭議](https://medium.com/tenable-techblog/lets-reverse-engineer-discord-1976773f4626)一直[很多](https://www.simpleanalytics.com/is-gdpr-compliant/discord)
曾發生員工[濫用職權](https://www.reddit.com/r/internetdrama/comments/dqb0m8/discord_trust_and_safety_employee_uses/)、違反歐盟 GDPR [被罰](https://www.complianceweek.com/regulatory-enforcement/discord-fined-830k-for-gdpr-lapses/32372.article)，早年也有[極端團體](https://www.forbes.com/sites/thomasbrewster/2019/01/29/discord-the-2-billion-gamers-paradise-coming-to-terms-with-data-thieves-child-groomers-and-fbi-investigators/)氾濫問題
同老闆更早創立的遊戲平台 OpenFeint，也有過偷偷蒐集、盜賣個資的[事跡](https://www.courthousenews.com/gamers-say-openfeint-sold-them-out/)
[隱私政策](https://discord.com/privacyinformation-we-collect-automatically)包山包海，前述軟體會拿的資訊， Discord 大概都沒漏掉
而且就算關閉追蹤、刪帳，活動紀錄也僅「[去識別化](https://discord.com/safety/privacy-preserving-products)」，不會自動刪光
_# 除非手動一一刪除_
若用自動化工具清資料，或選第三方加密前端，則可能被官方 [ban 帳](https://support.discord.com/hc/en-us/articles/115002192352-Automated-User-Accounts-Self-Bots)

</br>

---


Discord 我有親身經驗，沒興趣的可略過
尚未學成~~被害妄想症~~出師之前，為加入開源社群，我曾用過 Discord
某天帳號突然莫名被封，官方只說要門號驗證
_# 我只加入開源社群，未活躍使用_
對沒有門號，或不願個資被出售的人來說，此要求很侵犯
所以我寄信給客服，結果得到疑似 AI 的答非所問：
「
您好 ，
很遺憾的是，我們的應用程式目前不支援 __________ ，因此我們無法針對此事提供幫助。您可以查看以下這篇文章，進一步了解目前可以使用的作業系統有哪些： https://support.discordapp.com/hc/articles/213491697
如果您還需要其他任何幫助，或者有任何其他問題的話，請隨時告訴我！
謝謝，
」
上面是原文，那段 `____` 意義不明
傳的文章也和反映事件無關，很像在羞辱使用者
後來有真人出現，表示沒給電話就無法登入，該帳號生產的內容也無法取出
再三確認後，對方表示：
> 電話驗證要求的確是我們的安全措施。 目前無法省略

儼然個資勒索軟體，只好放棄該服務
_# 現在回想，好險當時體驗差，及時退場以免個資被貪光_

---

<br/>

看了作者經歷，不在乎門號的你可能無感
但近期的年齡驗證爭議，需要的可是政府 ID (i.e. 身分證)
> 你是該，擔心一下...

-- 灼熱沙丘 K'zrath

因應英、澳法令，Discord 在該地推動實驗性[年齡驗證](https://www.theverge.com/news/650493/discord-age-verification-face-id-scan-experiment)
_# 小知識：英國、澳洲禁青少年用社群，還實施全網年齡驗證，隱私蕩然無存_
做法是找第三方合作商，掃描身分證件、或直接拍臉照
號稱生物特徵不離裝置、上傳的 ID 則會「處理完即刪」
但如果系統誤判，就需要提供資料進一步審核

猜猜怎麼樣？
當然外洩了！

第三方年齡驗證服務商，在 2025 年 8 月[被偷](https://arstechnica.com/tech-policy/2026/02/discord-faces-backlash-over-age-checks-after-data-breach-exposed-70000-ids/)約七萬筆個資
_# 別忘記，此處個資是「政府 ID」，非常敏感_
主要受害者是英國、澳洲用戶，畢竟英澳政府用很愚蠢的方式「保護兒童」
結果兒少機敏資料反而外洩了，其他成年人也跟著受害
不僅如此，之後 Discord 還想把年齡驗證[推至全球](https://arstechnica.com/tech-policy/2026/03/after-discord-fiasco-age-check-tech-promises-privacy-by-running-locally-does-it-work/)
無視先前外洩問題，顯示經營者對個資態度多輕忽
最終在社群排山倒海反彈下，才決定[暫緩施行](https://www.eff.org/deeplinks/2026/02/discord-voluntarily-pushes-mandatory-age-verification-despite-recent-data-breach)，改採自願制
所以如果你繼續用，哪天大概會碰上年齡驗證、和隨之而來的外洩風險

這印證「最小化資料蒐集」的重要性，畢竟沒拿就不會外洩
何況取得一堆機敏個資如身分證、生物特徵 (臉照)，用戶和企業的危險程度都倍增
從前駭客沒興趣的對象，如金囤了大筆數位黃金，當然變成標靶


<br/>

---

<br/>

### 長文警告
以下文章極長，敬請**挑有興趣的部分讀就好**

### 先備知識
替代品登台前，得先說明背景知識，否則多數人應該會迷途
以下幾項安全措施，分別提供特定保護功能：
#### 端對端加密 (end-to-end encryption, E2EE)
E2EE 常在私路系列文提到，可用多種方式實現
此處「端」指終端使用者 - 就是你和聯絡對象
概念像「把信鎖進盒子寄給對方，對方再用鑰匙打開讀取」，反之亦然
因為有加鎖，郵局、郵差、撿到信的路人都看不到內容，機密性高
_# 相較之下，多數一般服務中，「郵局」都握有解鎖鑰匙_
#### 完美向前保密 (Perfect Forward Secrecy, PFS)
又稱向前保密 (forward secrecy)，畢竟「完美」有點過度承諾
技術上來說，是為每個 session 或每則訊息獨立生成即逝金鑰 (ephemeral key)
因此就算一組金鑰被破解、盜取，其他訊息依舊安全，包括未來收發的訊息
同前述案例：
    你封裝信件給朋友時，每次都約定不同解鎖密碼
    就算郵差偷聽到你們今天約定的密碼，他也只能拆閱今天的信
    明天你寄出換過密碼的信時，信件又恢復安全了
    
和「沙盒保護」一樣，能在出事時控制災損
#### 網路轉發 (internet routing)
簡單說就是幫你轉個 IP，沒什麼特別
翻 VPN、跳[暗網](./deGoogle-browser.md#tor-是什麼)之類的手法都能達成，主要目的是保護使用者 IP 位址
畢竟任何一方，包括接收者、伺服器、政府，只要拿到真實 IP，就能大致鎖定用戶
因此內建網路轉發，可以防呆避免 IP 暴露

<br/>

---

<br/>

重頭戲終於來啦！

### 替代品

#### [Session](https://getsession.org/)
端對端[加密](https://getsession.org/session-protocol-technical-information)、大致[開源](https://github.com/session-foundation)，由瑞士非營利機構開發維護
_# 起家在澳洲，被政府[查水表](https://www.404media.co/encrypted-chat-app-session-leaves-australia-after-visit-from-police-2/)後搬去瑞士_
程式碼自稍後會介紹的 Signal 分支 (fork)而來，魔改後已大相徑庭
支援各大平台，下載即可使用，無需註冊
_# 不必提供電郵、門號等**任何聯絡資訊**_
無中央統一伺服器，預設有三層網路轉發，與暗網的洋蔥路由相似

<br/>

---

背景與[技術](https://arxiv.org/pdf/2002.04609) (只想看功能者可略)
Session 把區塊鏈 (block chain)技術引進通訊，藉以達成分散式架構
_# 沒錯，就是虛擬貨幣的那個區塊鏈_
既然有了基礎設施，不順便發行虛擬貨幣也太可惜，因此同套網路還有 Oxen 幣
客戶端的應用程式，外觀、使用體驗儼然就是通訊軟體，但底層概念更像**虛擬貨幣錢包**
創帳過程類似設立錢包，但存的是訊息而非貨幣
_# 用戶完全不會接觸到虛擬貨幣，那只是官方的技術實作_
帳號還原碼即錢包種子 (seeds)，和別人互加通聯時，用的則是公鑰
內建的網路轉發和洋蔥路由 (Onion routing)原理相似，只不過改用自己的實作
送出的流量會經三層加密，每個節點 (i.e. 伺服器)解密一層，直到抵達接收裝置
且為了防呆，用戶**無法關閉**轉發功能，確保 IP 不會意外曝光
_# 但語音功能是對等網路 (p2p)，通聯者會知道彼此 IP_
改用 Oxen 而非 Tor，是因為特定實體能在 Tor 網路架一堆惡意節點 (node)
比例夠高即有機會掌控特定流量的出、入節點，破壞 IP 匿名性
還能竄改出口節點的資料、降級安全標準
Oxen 的原理大致相同，不過得[質押](https://getsession.org/introducing-the-session-network-page)一大筆 Oxen 幣，才能維運一個節點
入場難度提升很多，拉高了惡意實體滲透匿名網路的門檻
節點維護者幫忙轉發流量，可獲得一些虛擬貨幣獎賞 (類似區塊鏈交易的 gas fee)
_# 有玩虛擬貨幣的大概知道，這就是 Proof of Stake (PoS)_
訊息寄出後，實際上會有 5-7 個節點接收 (節點群稱為 [swarm](https://getsession.org/blog/dev-diary-the-rise-and-fall-of-the-zombie-swarm))
以免特定伺服器剛好下線，造成訊息消失不見
伺服器會短暫保留加密的訊息，以防接收端剛好不在線上而漏接
通常[留存兩週](https://docs.getsession.org/session-network/session-protocol/onion-requests-and-message-routing)，可在應用程式調整時間長短

通訊流程像是：
你寄出訊息 → Oxen network 轉發 → swarm (一堆節點，i.e. 伺服器)接收 → 接收者

Session 為了裝置聯動，**移除完美向前保密 (Perfect Forward Secrecy)**
好處是不同手機、電腦上的 Session app，可以輕易達成同步
缺點則是一把金鑰丟失，所有訊息都會洩漏，此舉在隱私社群頗具爭議

---

<br/>

Session 支援「閱後焚毀 (disappearing message)」功能，可設定送出後 / 被讀取後多久自動消失
不論傳出後過多久，訊息都可以自由收回 (對方只會看到有一則訊息被收回了)
[Session Protocol V2](https://getsession.org/blog/session-protocol-v2) 還在路上，預計 2026 會規劃、動工
號稱將加回 Perfect Forward Secrecy、後量子時代安全性
_# 一旦量子電腦問世，依賴質數相乘加密的演算法，會幾乎變成零加密_

缺點：
* 無完美向前保密 (Perfect Forward Secrecy)
* 若對外帳號被公開，仍可能遇到騷擾
    雖然帳號識別是隨機碼，但那組隨機碼建立後就不會再更動
    所以如果朋友加了你的 Session，卻又不慎洩漏該連結 QR code
    可能會有陌生人來加你，那就只能手動封鎖了
    _# 聽起來像廢話？那是因為有其他 app 能杜絕社交騷擾，往下看便知_
* 非「全」開源
    精確來說，只有通知推送組件非開源
    因為 Android 需靠 Google Firebase Cloud Messaging (FCM)、iOS 需要 Apple Push Notification service (APNs) 發送通知
    否則有人傳訊息來時，App 不會跳出提醒
    但 Google 和蘋果的通知服務非開源，用了就會含閉源成分
    [官方說法](https://getsession.org/faq)：為推送通知，Google 和蘋果會得到你的 IP，蘋果還會額外拿到發送通知的 token
    _# 這也是 Session 上不了 [F-droid](./deGoogle-appStore.md) 的原因_
    若你很介意 IP 暴露，可以：
    * 開 VPN 
    * 選 slow mode
        app 會在背景運作，每一陣子就連線 swarm 看有沒有通知
        相對耗電很多，而且通知往往有延遲 (除非寄送時 app 正好啟動通知查詢)
    * 別用 Session
        沒開玩笑，每個人的威脅模式不同、在乎的點也不同
        不能接受就選其他的，沒有非哪個 app 不可
* 訊息傳出到送達，會有數秒時間差
    三層加密需要多點時間，就算優化過還是會比直接傳送慢
* 官方資訊可能會護短
在 [FAQ](https://getsession.org/faq) 中，被問到為何沒 Perfect Forward Secrecy，官方顧左右而言他
雖然官方在[其他社群](https://techlore.tv/w/5TpNvVB52d6zSWgTVXfuvz)解答過，但自家問答集是重要資訊來源，本應妥善維護

看不懂技術沒關係，不妨礙使用多數功能
哪怕是新手，體驗就像陽春版的 Line，難度很低
_# 那些噁心的技術，app 畫面上一個都不會出現，敬請安心使用_

#### [SimpleX Chat](https://simplex.chat/)
想像有個軟體，用連結加好友後，該連結就從此失效
沒固定對外帳號名、ID，甚至不用註冊帳號 (連固定對外公鑰都沒有)
那就是 SimpleX Chat - 另一個匿名、去中心化的極致
同樣[開源](https://github.com/simplex-chat)、端對端加密，有完美向前保密 (Perfect Forward Secrecy)
下載即可用，靠一次性連結加好友
**無**聯絡人搜尋功能，因此不怕~~被我~~陌生人騷擾 (沒人知道你帳號)
所有對話資訊都存在本地，且可設定加密，輸入 PIN 才能打開

<br/>

---

技術簡介
個人檔案 (profile)創建時，資訊盡數保存在本地
需用「一次性連結 (可掃 QR code)」加聯絡人，無法任意肉搜
_# 強迫用戶以「其他管道」加通聯，降低中間人攻擊 (MITM)風險_
伺服器不做存儲，主要功能是「處理**單向**訊息佇列 (message queue)」
_# 類似轉發訊息給接收者_
你發送訊息用的管路，和接收的通常不會是同一個
寄出時，會經由你選的 SMP 伺服器，經 Tor 轉發給接收方選的 SMP 伺服器
_# SMP：SimpleX Messaging Protocol，即支援此協議的伺服器_
再從那台 SMP 伺服器轉發給接收者，即所謂 2 跳式轉發
_# Tor 指洋蔥路由，構築高匿名性的暗網迴路_
從設計上避免伺服器分析誰和誰在聊，最小化 metadata 暴露
可設定閱後即焚，訊息消失後就像從未寄出過
每則訊息會 padding 至固定大小，偷窺者無法從封包大小猜內文長度
_# 想避免紅包被從厚度摸出大致金額，可以每次都墊白紙加到固定厚度，訊息亦然_

訊息傳遞流程：
你寄出訊息 → 己方 SMP 伺服器 --`Tor`→ 對方 SMP 伺服器 → 接收者
對方寄出訊息 → 對方 SMP 伺服器 --`Tor`→ 己方 SMP 伺服器 → 你

如果把 Line 理解成「用同一支電話聯絡所有人」，SimpleX 就是「對每個聯絡人都生成一支拋棄式門號，且送出和接收走不同線路」
這種解耦方式下的伺服器，也稱為「無腦管路 (dump pipes)」，只能轉發無法窺探
傳統加密上又疊了後量子加密，即使量子電腦問世資料依舊安全

---

<br/>

缺點：
* 若刪 App 卻沒備份，資料會永久消失
    畢竟資料存在裝置上，伺服器不負責保管
* 耗電
    想「收到訊息即時跳通知」，得讓應用程式在背景執行
    雖然不靠 Google FCM，但對電池消耗較大
* iphone 用戶的通知，會讓蘋果看到總通知數
    iOS 限制 app 在背景運作的能力，所以仍得靠 APNs 推送
    _# APNs：Apple Push Notification service，蘋果推送通知服務_
* 仍在早期開發階段，功能不穩常發生
    版本更新頻繁，如果沒讓應用程式跟上，可能遇到各種不相容事件
* 可用性 (reliability)不佳，有時會發送失敗、沒收到訊息、傳輸時間很久
    有極致的機密性 (confidentiality)、完整性 (integrity)，但犧牲了可用性
* 尚無跨裝置同步
* 另一方離線過久，訊息就可能佚失，因為伺服器僅暫時保管訊息

[作者初衷](https://techlore.tv/w/ajdC9xKFxSC3YcX3K8Cd7E)是提出新標準，讓大家都能安全通聯，未來值得期待

#### [Delta Chat](https://delta.chat/)
民間志願者維運，開發者、資金主要來自歐洲
免費、[開源](https://github.com/deltachat)，受端對端加密保護
技術不特別，本質上就是 email
只是前端經調整，取出訊息本體讓畫面看起來像聊天軟體
因為 email 技術已經很成熟，微調即可
傳遞過程經許多優化，延遲不高
端對端加密用公定標準 [OpenPGP](https://www.openpgp.org/)，部分使用 AutoCrypt
訊息可設閱後即焚，基礎的功能大致都有
支援多裝置同步，Linux 手機 [Ubuntu Touch](./deGoogle-mobile-OS.md#Ubuntu-Touch) 也有 app 可用
資料傳遞方式：
你的裝置 → 某個 email 伺服器 → 接收者的裝置
幾乎就是 email，夠簡單了吧！

缺點：
* 無完美向前保密 (Perfect Forward Secrecy, PFS)
    因為 OpenPGP 尚不支援，不過開發中的 AutoCrypt V2 預計會落實 PFS
    還能提供後量子時代安全性，可以拭目以待
* 沒內建網路轉發
    畢竟技術上是 email，本來就不會自動翻牆
    所以 IP 不會被隱藏，很在意可以自行翻 VPN
* Metadata 保護較弱
    在 email 生態系中，伺服器提供者會看到：
    * 寄 / 收件地址
    * 訊息大小
    * 時間戳記
    沿用既有標準，也難免繼承部分缺點

若不喜歡官方應用程式，[Android 用戶](https://f-droid.org/en/packages/chat.delta.lite/)可裝 [ArcaneChat](https://arcanechat.me/)
_# Delta Chat 的替代前端，開源軟體的好處就在這_
隱私部分幾乎沒差，主要是花俏功能比較多

#### [Briar](https://briarproject.org/)
醜話說前頭，Briar 只有 Android、桌面版
直譯野玫瑰，確實也提供野草般的任性
[開源](https://code.briarproject.org/briar)、非營利、端對端加密的通訊軟體
沒伺服器，靠對等網路 (peer-to-peer, p2p)連線
_# p2p 可理解成「你和對方直接通訊」，沒伺服器在中間_
所有資料都加密存在本地，下載軟體後基本上無「官方」在處理、蒐集你的資料
註冊就是想個名字、密碼，不需輸入個資 (畢竟沒人在後面拿)
特別的是，**Briar 斷網也能用**
有網路時用 Tor，沒網路就轉藍牙，訊號能跳多個中繼使用者，直到抵達目標裝置
_# 類似離線版 mesh，可想像每個中繼站都是 wifi 分享器，只是改成分享 Briar 訊息_
除了保障隱私、安全，在高度言論審查區域也能用，因為幾乎無法線上監控
資料流向很簡單：
你 → 對方
或
你 → 中繼者裝置 x N → 對方

缺點：
* 對方離線時，訊息很可能傳到虛空
* 耗電
    為避免漏接訊息，Briar 會持續在背景運作，所以很耗電
* 若遺失帳密，沒人能幫你找回來
* 一對一通訊有完美向前保密 (Perfect Forward Secrecy)，一對多則無

除了私訊和群組，Briar 還能經營論壇、部落格、RSS，詳情請見[使用手冊](https://briarproject.org/manual/)
若哪天台灣陷入戰亂，Briar 將是突破封鎖的好選擇

#### [Signal](https://signal.org/) ([Molly](https://molly.im/))
直翻「訊號」，可說是訊息安全性、隱私大躍進的重要里程碑
大致[開源](https://github.com/signalapp)、端對端加密、有完美向前保密 (perfect forward secrecy)、[量子時代仍安全](https://signal.org/blog/spqr/)
_# 閉源部分主要是通知組件，Android 用 Google FCM、iOS 用 APNs_
訊息可設閱後即焚，還能發限時動態，是功能完整的替代品

<br/>

---

技術原理 (**可略**)
說到 Signal，不得不提通訊協議 [**Signal Protocol**](https://signal.org/docs/)
其中招牌之一，便是雙棘輪演算法 ([Double Ratchat algorithm](https://signal.org/docs/specifications/doubleratchet/))
用途是每則訊息都配獨立密鑰，所以一組密鑰被取得，不影響其他訊息安全性
帶來的好處即完美向前保密 (Perfect Forward Secrecy, PFS)，及後滲透安全性 (post-compromise security)
_# 此處用完美 (perfect)應該不為過，因為保密的是「每則訊息」_
後來升級成[三棘輪](https://eprint.iacr.org/2025/078)，實現後[量子](https://signal.org/docs/specifications/mlkembraid/)安全性

不過雙棘輪是「為之後每則訊息替換密鑰」，所以還需要起始金鑰
有點像：
    某人 → 父母生的 → 父母怎麼來的 → 父母的父母生的 → 那最初的父母哪來的？
訊息密鑰的原初父母，當然就是另一個加密演算法
[X3DH](https://signal.org/docs/specifications/x3dh/) (Extended Triple Diffie-Hellman)非對稱密鑰協議，可用公鑰產生起始私鑰
兩組私鑰自動互相驗證，即使任何一方不在線也能完成
主密鑰由事前金鑰 (prekey)、即逝金鑰 (ephemeral key)、身份鑰 (identity key)組成
即逝金鑰在每個 session 結束時消失，因此無法還原上一個 session
後來延伸的 [PQXDH](https://signal.org/docs/specifications/pqxdh/)，則提供量子時代的保護
簡單說就是「X3DH (或 PQXDH)提供首則訊息 PFS，之後的 PFS 由雙棘輪接手」
實作時，用 HMAC-SHA256 搭配 AES-256
讓接收方能驗證內容未遭篡改，以及發送者沒被仿冒
若因網路問題，導致訊息未按順序送達、單一方下線等狀況，就靠 [Sesame](https://signal.org/docs/specifications/sesame/) 解決
簡單來說，就是先存幾組金鑰，訊息抵達時再一一解鎖

資料流程沒什麼特別，和傳統通訊軟體無異：
你 → Signal 伺服器 → 接收者

---

不過辦 Signal 帳號需要電話號碼，社群多次反映官方仍維持此做法
強制拿門號能防濫用，缺點是有門號即可定位用戶
而且有些人沒有門號，但那些人可能更需要通訊安全
_# E.g. 戰亂地區、言論管制區，或受暴兒少_

後來 Signal 也推出備份功能，把對話以端對端加密存在雲端
就算換裝置也能還原對話，不怕資料意外遺失
不過此功能似乎還在 beta 測試，要手動開啟才會生效
且備份多媒體有容量限制，付費方案額度比較充足
_# Signal 非營利，付費只是支持理念，不想付自行備份即可_

缺點：
* 官方態度酷似科技巨頭，例如電腦版 Signal 加密問題
    從前 Signal 桌面版靠 [SQLCipher](https://www.reddit.com/r/signal/comments/gujugo/is_signal_safe_to_use_on_windows_is_it_still/) 加密，密碼明文存在同裝置上
    雖然其他 app 看不到加密的訊息，但若裝置被取得就形同虛設
    社群常提及、官方也一直都[知道此問題](https://github.com/signalapp/Signal-Desktop/issues/5703)，但從未優先處理
    [官方說法](https://community.signalusers.org/t/vulnerabilities/4548/7)：
    > 那把金鑰本來就不是機密，用戶可自行加密全硬碟
    
    嗯，沒打算改
    
    現階段最好的做法，就是只用手機版 Signal
    非要用電腦版的話，請記得加密硬碟
    Linux 可用 [LUKS](https://guardianproject.info/archive/luks/)，MacOS 有內建 FileVault
    Windows 的 BitLocker 並[不安全](https://www.virtru.com/blog/zero-trust/microsoft-bitlocker-encryption)，但聊勝於無
* 註冊要門號
    和 Line 不一樣，至少有內建保護措施
    萬一有人取得你的門號、想重新註冊 Signal 劫奪帳號
    他還得知道你當初設的 PIN，否則會被鎖在外面
    從前 Signal 加好友得靠門號，但自從有了[帳號名](https://signal.org/blog/phone-number-privacy-usernames/)，門號基本上不會暴露
    之前因門號衍生的[漏洞](https://arxiv.org/html/2411.11194v4)，也因此不修而復
* Metadata 安全性疑慮
    Signal protocol 保障的是「訊息內容」，不包含其他資料
    例如和誰聯繫、何時聯繫、聯繫頻率、時長...
    不過[隱私政策](https://signal.org/legal/)頗友善，僅保存「最初註冊時間」和「最後連到 Signal 的日期」
    經[法院認證](https://www.aclu.org/news/national-security/new-documents-reveal-government-effort-impose-secrecy-encryption)，應該不必太擔心
* 集中化服務 (且在美國)
    Signal [架在](https://proton.me/blog/is-signal-safe) AWS (亞馬遜雲端)上，哪天政府伸出黑手，服務就得下線
    但理論上不至於發生，因為政府也愛不釋手
    之前 Signal 醜 (或蠢？)[聞](https://www.bbc.com/news/articles/cj0q5r7ggnlo)，是因為有人把媒體高層拉進群組，國家機密直接攤開
    _# 那是參與者智商問題，和技術無關_

題外話，馬斯克曾[宣稱](https://atomicmail.io/blog/xchat-by-elon-musk-overview-privacy-claims-vs-reality?utm_soucre=oncely) χ chat (即推特私訊)比 WhatsApp、Signal 更安全
但 χ chat **無**向前保密 (forward secrecy)、私鑰存在伺服器上、程式碼和 protocol 細節未公開、沒被獨立稽核、記錄大量 metadata、由營利機構維運
_# metadata 可是個人化廣告利器_
更何況復原碼居然是「四位數 PIN」，被暴力破解的風險極高
**真要選，Signal 絕對更安全**

好像...漏講了什麼？

沒錯，就是 [Molly](https://molly.im/)
Molly 是 Android 版 Signal 的分支 (fork)，由社群開發、維護
完完全全的免費[開源](https://github.com/mollyim/mollyim-android)專案，補齊了 Signal 一直沒做好的部分
還追加不少安全、隱私措施，功能體驗也更完整
_# 注意，Molly 只是替代前端，一樣會連到 Signal 伺服器_

主要差異有：
* 拔掉 Google FCM，不再有閉源組件
    Molly 支援 [UnifiedPush](https://unifiedpush.org/) (直翻統一推送)，能即時推通知又不太耗電
    想擺脫 Google 的 Android app，往往會面臨接收通知的難關
    比起「每個軟體都在背景運作」，由「一個背景運作者統一轉發通知」省電的多
    於是就有了 UnifiedPush，問世後許多開源軟體紛紛投入懷抱
    原理是 UnifiedPush 相關 App 如 [Sunup](https://unifiedpush.org/users/distributors/sunup/)、[ntfy](https://unifiedpush.org/users/distributors/ntfy/)，在背景接收所有通知
    收到就轉給對應 app (e.g. Molly)，替代原先 Google FCM 的角色
    且通知伺服器可自架、也有尊重隱私的第三方選擇
* PIN [靜態加密](https://github.com/mollyim/mollyim-android/wiki/Data-Encryption-At-Rest)
    使用者可以設通關密語 (passphrase)，加密保護裝置上的資料
    就算手機被偷、扣留，仍享有基本保護
* 自動鎖
    可以設定閒置多久、或手機螢幕關閉後，app 自動上鎖
* 記憶體覆寫 (RAM shredding)
    一般情況下若手機遭竊，暫存在記憶體的資訊有機會被取出
    因此 Molly 追加了閒置、關閉 app 後，能自動清洗 RAM 的功能
* 多裝置連動
    官方 Signal 長久以來，一直不支援多裝置同步
    Molly 率先提供此功能，平板連線都不成問題
    _# Signal 直到 2025 才支援跨裝置同步，背後原理是將所有裝置加入一個群組_
* 內建 SOCKS proxy，可轉發網路流量給代理或 Orbot (Android 的 Tor app)
    這樣就能隱藏 IP 了！
    _# 當然，手動翻 VPN、Tor 也行_

缺點：
* 僅支援 Android
* 依舊會連回 Signal 後端，因此仍是**集中化服務、需要門號**
* 若未串連 UnifiedPush，會回退使用 Signal 的通知模組，i.e. Google FCM

最糟大不了跟 Signal 一樣，所以多數情況都是 Molly 更理想

#### [Wire](https://wire.com/)
總部在瑞士、註冊在德國的公司，由 Skype 創辦人成立
有端對端加密、完美向前保密 (Perfect Forward Secrecy, PFS)、[量子](https://wire.com/en/security)時代安全性
由官方提供**中心化**服務，[伺服器](https://github.com/wireapp/wire-server)、應用程式都[開源](https://github.com/wireapp/wire)
支援所有平台，包括 iOS、Android、各大桌面、網頁 (可用瀏覽器開)
個人版免費，團體、企業版則須訂閱
對「[超大群組聊天](https://wire.com/en/blog/mls-is-coming-to-wire-app-learn-more)」優化，個人方案最多 500 人，付費版支援到 2000 人
主要獲利來自企業方案，理論上不必擔心個人戶被收割
因此更像 Discord、Slack 替代品

---

**背景**
Wire 起初做消費端產品，進軍 B2B 市場後做得風生水起
企業、政府機構等大戶，已成為主要[收入來源](https://techcrunch.com/2022/08/12/wire-series-c/)
曾因[收受 VC 資金、將控股公司搬到美國](https://techcrunch.com/2019/11/13/messaging-app-wire-confirms-8-2m-raise-responds-to-privacy-concerns-after-moving-holding-company-to-the-us/)，備受隱私倡議者抨擊
後來又搬回德國、瑞士，重回隱私重地懷抱

**技術簡介**
主要使用普羅透斯協定 ([Proteus Protocol](https://arxiv.org/html/2603.06540))，和 Signal Protocol 本出同源
一樣有 Double Ratchet，因此具備向前保密 (forward secrecy)
[群組聊天](https://wire.com/en/blog/wire-messenger-security-explained)引入「訊息層安全性 ([Messaging Layer Security](https://wire.com/en/blog/messaging-layer-security-evolving-secure-communication))」
用樹狀結構處理金鑰流程，有效減少規模提升帶來的運算成本
_# Signal 協議正是因為算力問題，難以擴增到規模千人的群組_

訊息傳遞流程很傳統：
你 → Wire 伺服器 → 接收者

---

雖然有人批評，Wire 主要優化都針對企業戶
但好處就是，個人用戶被撈錢的風險較小
因為營運、獲利都由企業給了保障
_# 除非他們學 Google，兩種韭菜都割_

缺點：
* 註冊需要 email
    雖然比門號好一點，但仍會暴露部分資料
* 會蒐集 Metadata
    E.g. email、通聯對象、時間戳記、裝置 ID 等
    雖然傳輸時有 TLS 加密，但**在伺服器上[明文](https://www.vice.com/en/article/secure-messaging-app-wire-stores-everyone-youve-ever-contacted-in-plain-text/)儲存**

<br/>

---

<br/>

過渡產品之後，就是 Discord 替代品了
<br/>

---

<br/>

#### [Matrix](https://matrix.org/) ([Element](https://element.io/) / [FluffyChat](https://fluffychat.im/))
Matrix 是通訊協議，Element 和 FluffyChat 是兩種前端 (i.e. 能下載的 app)
[開源](https://github.com/matrix-org)、聯邦式去中心化 (可自架伺服器，且各伺服器互通)，預設[端對端加密](https://matrix.org/docs/matrix-concepts/end-to-end-encryption/)
Matrix 由[非營利](https://matrix.org/blog/2022/12/01/funding-matrix-via-the-matrix-org-foundation/)機構 [Matrix.org](https://matrix.org/) 開發、維護，Element 則是[營利公司](https://element.io/en/open-source)的[開源](https://github.com/element-hq/element-web)產品

---

背景與技術
Matrix 由劍橋物理學兼電腦科學家，與電信工程師一同發明
目的是解決通訊碎片化、中心化問題
並成立 Matrix.org 保管協議，確保中立性、任何人都能自架此服務

因應分散式服務本質，Matrix 房間歷史用事件圖 (event graph)寫存
畢竟多伺服器平行運作時，不太可能線性發展，需解決時序衝突
事件圖正好適合處理這種情況，搭配加密就能兼顧效能與安全性
一對一私訊用 Olm 加密，同樣有雙棘輪 (double ratchet)機制
所以端對端加密外，亦有完美向前保密 (Perfect Forward Secrecy)
群組聊天則靠 Megolm，訊息一樣端對端加密
但為降低大群組運算成本，多個訊息會重複使用密鑰，因此向前保密效果有限
_# 1:1、group chat 有端對端加密，但 public chat 沒有，因為那本來就是公開場合_

同批人推出第一個基於 Matrix 協議的 app，稱為向量 (Vector)
後改名 Riot、再改成 **Element**，即官方旗艦應用程式
網頁、Android、iOS、各大桌面都能取得
雖然 Element 背後是營利公司，但收益都來自企業方案、咨詢服務
社群架設、使用完全免費，也不會被塞廣告
有趣的是，數學中「一維矩陣」就是「向量」，每個值則稱為「元素 (element)」
不愧是物理學家的幽默

FluffyChat 是社群專案，由德國開發者 [krille-chan](https://troet.cafe/@krille) 領銜製作
主打開源、非營利、**可愛**的 Matrix 前端，同樣可在所有平台取得
_# [Ubuntu Touch](./deGoogle-mobile-OS.md#Ubuntu-Touch) 也能用喔！_
和其他前端相容，例如 Element
因為符合協議，所以該有的保護都有，只是介面比較直觀
_# 多以泡泡、卡通圖形呈現_
相較適合大群、公司營運的 Element，FluffyChat 少了些花俏管理功能
不過基本聊天很夠用，而且**支援 UnifiedPush**
_# I.e. 若設定得宜，可以更省電_

有些人詬病 Matrix 協議漏洞多，聲稱不夠安全
但各種前端[出過的包](https://matrix.org/blog/2022/09/28/upgrade-now-to-./file_name-encryption-vulns-in-matrix-sdks-and-clients/)，多是實作而非協議問題，後來也都已修復
算是「還行」的方案，至少比 Discord 安全多了

訊息傳遞流程：
你 → 當初加入的 Matrix 伺服器 → 接收者所在的伺服器 → 接收者
如果接收方不在線上，伺服器會暫存訊息，直到他上線才同步過去 (當然，是以密文存放)
雖然 Matrix 可和其他服務橋接 (e.g. Discord、WhatsApp)，但那會破壞原有安全性
畢竟跨協議傳遞，通常得先解密再加密，加解密的脆弱環節就容易被攻擊

---

群組聊天一旦開啟端對端加密，就無法再關閉，以免被惡意人士降級滲透

缺點：
* 群組聊天向前保密能力有限
* [Metadata](https://matrixdocs.github.io/docs/security/overview) 非端對端加密
    E.g. 房間主題、訊息種類與大小、時間戳記等
* 註冊需聯絡資訊，例如電郵或門號

#### [Stoat](https://stoat.chat/)
從前叫 Revolt，後改名 Stoat，號稱最佳 Discord 替代品
[開源](https://github.com/stoatchat/)、去中心化，伺服器可自架但非聯邦制
_# I.e. 每個伺服器自成一國，~~像苗栗那樣~~_
架構和體驗類似 Discord，有伺服器、文字頻道、語音頻道、角色和細緻權限
無廣告、承諾不販售個資，目前靠捐贈維生

缺點：
* 尚無第三方檢核
    雖然開源，但缺乏中立機構檢查程式碼，難確保安全性
* **沒**端對端加密
    伺服器營運者理論上能解鎖內容
    安全性仰賴信任，而非源頭設計
* 服務集中化
    雖然可自架但沒聯邦機制，多數人進入的是預設伺服器，i.e. 官方服務
    大家都在同一個伺服器，形同沒去中心化
    _# 尤其設在英國，政府[很不尊重](https://www.eff.org/pages/uk-online-safety-bill-massive-threat-online-privacy-security-and-speech)數位隱私_
* 註冊需要 email，通聯等 metadata 也因營運所需會蒐集
* 有閉源依賴項
    [隱私政策](https://stoat.chat/legal/privacy)說明，Stoat 服務有用 Cloudflare
    _# 就是之前[掛掉](https://www.cnbc.com/2025/11/18/cloudflare-down-outage-traffic-spike-x-chatgpt.html)，結果害一堆服務進不去的那個 Cloudflare_
    Cloudflare 是閉源美企，座落在用戶和伺服器之間，可看到解密後的流量
    要不要信任它，可自行衡量

如果只要「減害版 Discord」，Stoat 或許能接受
但想要更多隱私，Wire、Matrix 比較適合

<br/>

---

### 其他選項？
iMessage 預設端對端加密，沒開源但不到替換標準
[Threema](https://threema.com/) 遵守 GDPR、開源、設於瑞士，但**沒免費版**不符合 FOSS 條件
雖不在推薦名單，願意付費者還是可選用
至於 Discord 替代品：
[Rocket chat](https://www.rocket.chat/) 免費得自架
[Zulip](https://github.com/zulip/zulip) 免費功能受限、自架仍有功能限制
[mattermost](https://github.com/mattermost/mattermost) 付費才能用

鑑於有更好的選擇，就僅列舉供參考

至於 [Meshtastic](https://meshtastic.org/)，沒 Perfect Forward Secrecy 但免費[開源](https://github.com/meshtastic)
和 Briar 技術類似，不過比較不像常規通訊軟體，幾乎只有文字訊息功能
私訊有端對端加密，但群組聊天預設沒有，得自己手動開啟
有興趣者可以去玩玩


