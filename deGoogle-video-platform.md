# deGoogle - 替換 Youtube

> Youtube 又來一堆詐騙廣告，煩死了！

受夠 Youtube [劣質廣告](https://www.dcard.tw/f/talk/p/258840958)了嗎？
[色情](https://www.dcard.tw/f/talk/p/235733734)、[噁爛](https://www.dcard.tw/f/talk/p/238916782)通通來，簡直沒底線
實際上，那正是[狡猾](https://www.inside.com.tw/article/16293-ie6-killed-by-youtube-engineer) Google 的行銷策略
撒劣質廣告，讓你受不了而入坑 Youtube Premium，進而增加訂閱率
若大眾因此訂閱，反而助長 Google「撒爛廣告就能增加訂閱率、收益」的行為
屈服，只會鼓勵 Google 無良行銷，看看他們[營收](https://affmaven.com/youtube-statistics/)便知

為什麼敢如此囂張？

因為影音市場中，Youtube 市占率極高，可說已經壟斷
不論[電視](https://tw.news.yahoo.com/%E5%B0%BC%E7%88%BE%E6%A3%AE%E6%9C%80%E6%96%B0%E8%AA%BF%E6%9F%A5-youtube%E6%93%8A%E6%95%97netflix%E6%90%B6%E4%B8%8B%E5%B8%82%E5%8D%A0%E7%AC%AC-%E7%8E%8B%E5%BA%A7-223000404.html)[串流](https://techcrunch.com/2009/06/09/youtube-video-streams-top-1-billionday/)、[影音 app](https://www.digitalinformationworld.com/2020/02/youtube-dominates-all-the-major-apps-takes-away-most-streaming-time-on-smartphones.html)、還是[數位廣播(Podcast)](https://www.bloomberg.com/news/newsletters/2024-08-22/apple-loses-its-podcasting-lead-to-youtube-and-spotify)
就算非壟斷的戰場，[短影音](https://www.affiliatebooster.com/youtube-shorts-statistics/)、[直播](https://streamhatchet.com/blog/youtube-stealing-live-streaming-market-share/)、[音樂播放](https://www.forbes.com/sites/billrosenblatt/2024/03/30/music-industry-annual-reports-show-stable-growth-and-youtube-strength/)等，Youtube 仍佔有一席之地
尤其影片平台，並非「做得比較好」就能有效競爭
哪怕消費者願意換，「內容」和「創作者」多半已定居特定平台
想看 [AI 界唯一真神的公開課](https://www.youtube.com/@HungyiLeeNTU)，幾乎只能上 Youtube，畢竟人家只 po 在那

拉回正題，那隱私呢？

Google 老早就收購 Youtube 了，可想而知是隱私噩夢
先看個圖
[deGoogle Youtube](image link)
^FOSS^ ^指免費開源軟體^ ^(^^Free^ ^and^ ^Open^ ^Source^ ^Software^^)^
^non-profit^ ^指「不以營利為目的」^
^下半部多個湊在一起的，主要依特質做分群^

<br/>

## 欠換平台
### Youtube
首先登場的是 - **兒童權益剝削**
Youtube 因未經允許追蹤兒少，付出[一億七千美金](https://www.ftc.gov/news-events/news/press-releases/2019/09/google-youtube-will-pay-record-170-million-alleged-violations-childrens-privacy-law)的代價
他們[被罰](https://www.bbc.com/news/technology-49578971)[又被罰](https://techweez.com/2025/08/20/google-youtube-kids-privacy-lawsuit/)，卻仍[死性不改](https://www.bbc.com/news/technology-64786968)，今年 (2025)再度[砸錢消災](https://www.reuters.com/sustainability/boards-policy-regulation/google-settles-youtube-childrens-privacy-lawsuit-2025-08-19/)
如果賠錢就會收斂，那絕不是我們認識的 Google
甚至順勢推出[年齡推算](https://tech.udn.com/tech/story/123454/8938080)機制，「兒童權益」正好當擋箭牌
你填幾歲僅供參考，官方會用影片瀏覽記錄，推算實際年齡
_# 太愛看卡通、又會造訪成人片，可能導致你被 ban_
停權與否非重點，Google 大概不想踢除客戶
重點是，合理化添加新演算法、追蹤紀錄
年齡區間，也是個人化廣告的一環
別忘了，[Youtube 使用](https://kids.youtube.com/t/terms) [Google 隱私政策](https://policies.google.com/privacy)
該拿的都沒少，個資也會用於廣告推送
近期還有新舉措 - [抓家庭方案濫用](https://www.dcard.tw/f/talk/p/259687722)，[規定](https://support.google.com/youtube/answer/7507744?hl=zh-Hant&co=GENIE.Platform%3DiOS#:~:text=%E5%AE%B6%E5%BA%AD%E6%96%B9%E6%A1%88%E9%87%8D%E8%A6%81%E9%A0%88%E7%9F%A5,YouTube%20%E5%AE%B6%E5%BA%AD%E6%96%B9%E6%A1%88%E7%9A%84%E8%B3%87%E6%A0%BC%E3%80%82)「訂閱者須同住」
_# 旅居外地、住宿舍的，Google 不承認家人關係，謝謝_
Google 可能用「同住家人」當藉口， 合理化此舉
但也變相確立哪些人，真的是彼此親屬 (親屬關係是重要 metadata 喔！)
搭配瀏覽類型，幾乎可推出誰是父母、兒女
親子相關廣告、教材、電玩，都能更精準硬塞給你
更別提[神奇](https://forum.gamer.com.tw/C.php?bsn=60030&snA=635141)的[文字獄](https://www.mobile01.com/topicdetail.php?f=514&t=6900986)，[國內外網友](https://www.reddit.com/r/youtube/comments/11wgrlc/youtube_keeps_deleting_my_comments_for_no_reason/)都是[受災戶](https://www.dcard.tw/f/talk/p/254644138)，標準令人納悶
_# 能想像是為了擋機器人、廣告騷擾、仇恨言論，但那演算法也寫太爛了吧！_

[censored tube](https://www.mobile01.com/topicdetail.php?f=514&t=6900986)


### Vimeo
呃，可能很多人沒聽過這平台，那跳過也無妨
本段落旨在提醒既有用戶，此服務並**不**保障隱私、使用體驗
Vimeo 主打高品質內容、無廣告、使用者付費，試圖營造高階形象
然而，其服務尚欠優化，載入影片速度極慢，酷似早年 Youtube
_# 還記得從前 Youtube 的轉圈符號嗎？用 Vimeo 常會有此困擾_
![youtube loading gif](https://media.tenor.com/JcKHX9Ev7SoAAAAC/youtube-you-tube.gif)
隱私部分呢？
來看看官方[隱私政策](https://vimeo.com/legal/privacy/policy)，為什麼該換掉：
* 蒐集的資訊：
    * 註冊時的電郵、姓名、電話等，或連動登入的相關資訊 (e.g. 以 Google 登入)
        若你在特定國家，為確保年齡還要自拍照 / 證件資訊 (e.g. 身分證)
    * 瀏覽器、OS 種類
    * IP 位址 (還會用來[推算地理位置](https://vimeo.com/legal/privacy/policy#automatically-collected-information)唷！)
    * 互動紀錄，像是：
        * 搜尋了什麼
        * 滑鼠軌跡、頁面捲動
        * 鍵盤活動，如按下的按鍵

拿來做什麼？

不外乎優化服務、營運所需、帳號管理等
但是！
個資也用於廣告推送，包括第三方廣告商
嘿嘿，你以為影片無廣告，就沒廣告商介入嗎？
蒐集統計資料、看過哪些影片、在哪停留最久，可以推斷個人偏好
如 Google、Meta 這類無處不在的廣告商，就算你跨站也躲不掉
在 Vimeo 收集資訊，到其他網站用來推廣告，還是能賺

不僅如此，他們還會蒐集、儲存上傳影片中的生物特徵
細緻入微的臉部資訊，用於辨識年齡、性別、和位置
最大的問題是，那些行為未經用戶同意，甚至沒告知
所以被告了，也[付出 200 多萬美金](https://www.scworld.com/news/vimeo-ai-biometric-privacy-lawsuit)的代價
_# 此事發生在 Vimeo 旗下平台 Magisto，其他服務能亂搞，難保 Vimeo 本身不會_

### Bilibili
社群罵 Youtube 時，總會有人推薦 Bilibili (嗶哩嗶哩)
不過就隱私角度而言，兩者半斤八兩
閉源、中資、個人化廣告，壞事全包辦
_# 之前提過中國線上服務的[風險](./chinese-service-risk.md)_
曾[索求過](https://pandaily.com/bilibili-responds-to-member-privacy-concerns/)用戶姓名、電話、身分證號、地址等私密資訊
且會和其他商家，如中國聯通共享
也有過內部員工，[注入惡意程式碼](https://www.thepaper.cn/newsDetail_forward_29988567)到網頁服務
雖已開除始作俑者，但這顯示安全性漏洞和權限管控問題
大概未落實零信任，無法保證員工還能搞出什麼花樣
_# 資安的零信任概念，可見[前文](./zero-trust_persecurity-delusion.md)_
最「精彩」的事蹟，莫過於後端[程式碼外洩](https://technode.com/2019/04/23/bilibili-source-code-leaked-on-github-containing-usernames-and-passwords/)，包括用戶姓名、密碼
要知道，資訊一旦拋上網，就難以回收

## 獨立替代品
### [Odysee](https://odysee.com/)
希臘史詩奧德賽取諧音，不過似乎沒官方中譯
既然後綴是 -see，我就亂叫它「奧德視」
美國公司，背後是 LBRY Inc. (讀作 Library)
成立背景是不滿 Youtube 過度商業化、偏袒廣告商、詭譎文字獄、[胡亂貼黃標](https://www.blocktempo.com/lbry-100a-blockchain-based-decentralized-digital-content-marketplace/)
於是推出「開源」、「自由」、去中心化的替代品
之所以叫 Library，是希望成為數位圖書館，分享影片、音樂等
Odysee 的去中心化非常徹底，建構在區塊鏈上，沒任何人能「擁有」整個服務
「用戶」本身也是系統的一部份，哪怕只是觀看影片
_# 區塊鏈 (block chain)是虛擬貨幣的基石，不懂沒差，就當很分散、自由_
所以形同無審查，因為沒人能恣意把區塊鏈上的東西刪掉
奧德視介面很像 Youtube，轉換成本不高

畫面看起來像這樣：
[odysee snapshot, 30 分鐘認識深度學習](odysee-interface.png)
影片連結：[點我](https://odysee.com/@%E9%81%8A%E8%95%A9%E8%80%85:4/30-minute-deep-learning:4)

平台給創作者的獎勵，比 Youtube 有感多了
發影片、有流量、開贊助，各種管道都能獲取報償
甚至當觀眾也很爽，看影片、完成特定任務，一樣能拿獎勵
_# 立基虛擬貨幣協定，理所當然用自家貨幣 LBRY Credits (LBC)給酬勞_
有人[實測](https://dianxiaoeryu.com/lbry-odysee-%e7%9c%8b%e5%bd%b1%e7%89%87%e5%85%8d%e5%bb%a3%e5%91%8a%e6%89%93%e6%93%be%e3%80%81%e9%82%84%e5%8f%af%e8%b3%ba%e9%9b%b6%e7%94%a8%e9%8c%a2/)過，光看影片一年就能拿 450 台幣
雖然也蒐集[不少資料](https://lbry.com/faq/privacy-and-data)，但多數可選擇退出

缺點：
* 無自動字幕、外加字幕檔功能
    字幕得內嵌在影片中
* 自由度高，不當內容難杜絕
    Covid-19 時期，充斥許多假訊息、政治陰謀論
    有時也會出現恐怖主義、盜版、血腥內容
    區塊鏈的優點，是把雙面刃
    沒人能輕易移除區塊鏈上的東西，包括營運者
    _# 各地不同的節點上，都存有複本_
    官方做法是，受舉報、確認違規後，會取消那些內容的分潤
    違規影片也會從官網屏蔽，所以你就不會看到了
    畢竟雖可自不同節點存取，但多數人都是從官方入口造訪
    刪不掉沒差，看不到就行了
    _# Odysee 可視為 LBRY 的一個前端_
* 美企，受制美國政府
    近年美國政府[說](https://www.theguardian.com/technology/2023/jul/16/lbry-closes-odysee-cryptocurrency-tech-sec-fraud-extremist)，LBRY 未妥善登記就發行虛擬貨幣，違法應裁罰
    所以 LBRY Inc. 要關門了，LBRY 很快也會從 Odysee 消失
    不過別擔心，Forward Research 接手 Odysee 了
    且會以 [Wander wallet](https://help.odysee.tv/category-monetization/wander/) 替代，簡單說就是換湯不換藥
    繼續用 Odysee，不會有任何問題

你可能會[查到](https://finance.yahoo.com/news/google-buys-odysee-googl-investors-193807588.html) Google 收購 Odysee，但那是同名相片軟體，和奧德視沒半點關係

### [PeerTube](https://joinpeertube.org/)
同儕管 (？)，法國非營利組織 [Framasoft](https://framasoft.org/) 主導[開發](https://joinpeertube.org/zh_Hant/faq#who-is-working-on-peertube)的自由軟體
程式碼採 AGPLv3 開源，任何人都能自行架設
沒錯，就是架設

---

且容我細細說來：
* 聯邦宇宙 (Fediverse) 實現**半**分散式架構
    Fediverse 藉一系列獨立服務串連，形成完整的社群生態系
    Peertube 代替 Youtube、Mastodon 替換推特、Pixelfed 替換 Ig...
    _# 有趣的是，Meta 的~~降智程式~~ Threads，也支援 Fediverse 的協議唷！_
    每個極權、貪取個資的服務，幾乎都有 Fediverse 替代品
    且正因為互通，你可以用任一服務的帳號，去追另一個服務的帳號、頻道
    Fediverse 生態系還有個特色 - 半分散式架構
    任何人得自行架設實例 (instance)，加入整個生態系統，和其他實例互通有無
    _# 各種服務都採 W3C 標準的 ActivityPub protocol，所以溝通無礙_
    E.g. 你爽的話，立刻架個 Peertube 伺服器，就能變成 Fediverse 的一分子

    為什麼叫「半」分散式？

    分散式系統，通常會為資料製作複本，儲存到每個節點 (node)上
    節點和實例不盡相同，就算你炸掉任何一個節點，複本仍會保障資料安全
    經典案例就是區塊鏈 (blockchain)，如前述 LBRY 奧德視
    但 Fediverse 的做法，是多個「獨立」伺服器彼此聯繫
    除非事先備份、遷移，否則若實例突然掛掉，資料難以救回
    儘管能訪問其他實例，但登入時須從註冊的伺服器進場
    雖不被單一公司 / 政權控制，但每個實例都受維運者管轄
    伺服器所在國的法令，當然也適用
    _# 好處是當你看所有人都不爽，自己架服務、制定規則即可_
    因此多數情況下，Peertube 沒有統一的「官方」，但也不到完全無政府
    如果說 Youtube 為「帝國制」，Fediverse 就是「封建制」，區塊鏈則是「直接式民主」
    當然，沒人規定你一定要架服務，選個喜歡的實例註冊也行
    _# 只想看影片的話，甚至不用註冊、登入，就像 Youtube 一樣_

---

既然名叫「Peer」，當然有用上對等網路 (peer-to-peer, p2p)
_# 翻成「對等管路」可能更好？_
靠瀏覽器的 WebRTC、WebTorrent 技術，讓用戶分攤伺服器負載
所以越多人看同一部影片，伺服器反而越省資源
_# 因為使用者提供部分算力_
官方沒商業模式，多數實例志願維護者也沒有 (僅少數服務要訂閱、引入廣告外掛)

缺點：
* 影片載入速度較慢
    沒像 Youtube 或 Odysee 那般，對影片做壓縮優化 (或做得不多)
* 一樣有不當內容問題
    推廣時被朋友問過：「那不是放 A 片的地方嗎？」
    呃，Peertube 只是平台，不違法、合乎實例規定都能上架，自然什麼影片都有
    官方預設隱藏 NSFW 內容，你也可以自行設定屏蔽 (用戶、站方都行)
    有些實例標榜 NSFW，人家都標明了，是否加入就看你決定囉！
    若有侵害著作權、違法影片 (e.g. 屠殺)，須自行向營運者檢舉
    相較區塊鏈，至少不到近乎無法可管的程度
    且官方統計，所有實例中僅約 1% 為 NSFW 內容，不慎點入的機率低

Peertube 的吉祥物，是隻可愛的墨魚 Sepia
官方發文 Sepia 通常也會跟著露面，很想抱一隻來養 (？)
[By David Revoy - https://joinpeertube.org/, CC BY 4.0, https://commons.wikimedia.org/w/index.php?curid=84134714](peertube-sepia.jpg)

### DTube
和奧德視相似，同樣建構於區塊鏈上、靠虛擬貨幣打賞
不過易用程度天差地遠，新手、甚至開發者，初次進入往往會很困惑
[官方入口](https://d.tube/)看不到影片，得從[其他](https://dtube.luminade.fun/)節點進入
_# 此情形存在已久，恐怕等不到修復_

---

講古：

法國工程師 [Adrien Marie](https://www.crunchbase.com/person/adrien-marie) (網名 heimindanger)，原為 Steem 社群開發者
2016 年嘗試結合 Steem 區塊鏈、影片分享，隔年推出 DTube (可見結合應該算成功)
2020 年開始轉到自研區塊鏈 Avalon 上，使用 DTube Coin (DTC)
由社群選出領銜人 (Leader)，架設節點供大家使用
任何「上傳、轉貼、投票、留言、標籤」都會[寫入](https://token.d.tube/)區塊鏈，並按演算法即時發放 DTC
持幣者每小時會獲得投票權 (Vote Power)，可投票挖礦或贊助創作者
投票權能按讚、倒讚，靠互動決定影片排序
DTube 分配 90% 收益給用戶、創作者，**和 Odysee 一樣沒有廣告**
_# Odysee 甚至只抽 5% 平台費，加上 2.5% 交易手續費也不過 7.5%_
相較之下，Youtube 創作者僅得到 55% 廣告分潤、70% 「超級感謝」贊助
也就是平台拿走 45% 廣告費、三成贊助金
很多人說擋 Youtube 廣告傷害創作者，拜託，**選 Youtube 才是傷害創作者！**

---

缺點：
* 易用性低
    官方入口沒影片，對用戶很不友善
    得找其他頁面進入，有被仿冒、釣魚的風險
* 若帳戶裡沒 DTC，互動能力受限
    畢竟投票權來自虛擬貨幣，沒錢就沒~~人~~權
* 流量、內容不多，月活躍用戶大約 20 萬人而已
    _# Youtube 有數十億以上_
    那麼難用，當然不易吸引新用戶
* 同樣有不當內容問題
    身為區塊鏈，幾乎不可能強制刪除內容
    只能靠大眾給倒讚、平台屏蔽，緩解負面效應
    因此盜版影片、不當內容，管理難度較高
    _# 除非難用到侵權者也不想來 XD_

<br/>

---

<br/>

## 權宜替代品
怎麼會有這項？
因為 Youtube 已壟斷市場，許多創作者、內容都在上面
雖然 Google 仗著高市佔率胡作非為，但直接離席對許多人來說有難度
_# 當你追的網紅、愛聽的音樂只在 Youtube 上，換平台就等於放棄一切_
所以「相對保障隱私」、「提升使用體驗」、「開源」的選擇，因此變得重要
以下選項多是 **Youtube 隱私前端**，未完全擺脫 Google
_# 由於種類繁多但原理相似，介紹會相對簡略_

### [Invidious](https://invidious.io/)
社群開發者 [Omar Roth](https://omar.yt/) 希望使用 Youtube 時，不必犧牲隱私
所以創立 Invidious，作為代理伺服器取得 Youtube 影片資料、標題等 Metadata
原理是「你訪問 Invidious，Invidious 替你訪問 Youtube，再把資料回傳給你」
Invidious 未使用 Youtube API，而是用爬蟲方式搜羅資料
變成「少了廣告、追蹤器的 Youtube」，仍有訂閱、播放清單功能
還支援 [SponsorBlock](https://sponsor.ajay.app/)，能把業配片段拔掉

缺點：
* 依賴 Youtube，且服務不穩定
    Google 三不五時調整 Youtube 結構，常導致爬取流程出狀況
* 仰賴服務架設者
    Invidious 代理伺服器人人可架設，營運者會不會哪天停掉 instance 無法保證
    2020 年時，連創辦人 Omar Roth 都從 Invidious 退休了，長期服務堪慮
    _# 創辦人說無法負荷龐大工作量、心理健康出問題，畢竟這是無償的_

想試試的，可參見實例 (instance)[列表](https://docs.invidious.io/instances/)

### [Piped](https://piped.video/)
和 Invidious 原理相似，都透過第三方 instance，用爬蟲取得 Youtube 內容轉發給用戶
創辦人厭倦 Invidious 常常掛掉，所以另立新專案
_# 諷刺的是，Piped 也常崩潰_
Invidious 有的功能，Piped 大致都有，還能跨越年齡限制
且效率更高，前端用 Vue、後端用 Java (使用 NewPipeExtractor)
代理伺服器則以 Rust 寫成，架設可參考[中文指南](https://ivonblog.com/posts/piped-youtube-alternative-frontend/)
只想使用的話，請見實例 (instance)[列表](https://github.com/TeamPiped/documentation/blob/main/content/docs/public-instances/index.md)

缺點：
* 依賴 Youtube，且服務不穩定

### [FreeTube](https://freetubeapp.io/)
社群做的**電腦版** Youtube app，[開源](https://github.com/FreeTubeApp/FreeTube)、免費
可避開 Youtube 廣告、追蹤器，甚至不用帳號
支援 SponsorBlock 和訂閱頻道，也能透過 Invidious 代理連線至 Youtube
_# 否則會直接依賴 Youtube，所以官方建議翻 VPN 或 [Tor](./deGoogle-browser.md)_
Windows、MacOS、多種 Linux 分支都能用

缺點：
* 系統[有限制](https://github.com/FreeTubeApp/FreeTube?tab=readme-ov-file#official-downloads)，太舊的可能不相容
    官方說 Windows 要 10 以上、MacOS 12 以上
* 若未使用代理伺服器、VPN 或 Tor，IP 仍會被 Google 知道
    畢竟是直接連線到 Youtube，透過非官方手段取得內容
    所以連線資訊如 IP，依舊會傳給 Google

---

**接下來連三個是 Android App**

### [NewPipe](https://github.com/FreeTubeApp/FreeTube?tab=readme-ov-file#official-downloads)
新管 (？)，是社群開發的 Android app，用以代替 Youtube 應用程式
無廣告、可匯入播放清單、能追頻道，同樣不需 Youtube 帳號
且不只 Youtube，NewPipe 也支援 [PeerTube](https://joinpeertube.org/) 和諸多平台，功能很多樣
優勢是效能高 (幾乎無延遲)、服務穩定，可從 [F-Droid](https://f-droid.org/packages/org.schabi.newpipe/) 取得
_# F-Droid 是開源 Google Play 替代品，詳情請見[這篇](./deGoogle-appStore.md)_
連 Piped 都採相同 API，Android 玩家值得一試

缺點：
* 仰賴 Youtube (除非你拿來看 Peertube 或其他平台)
    NewPipe 本質是隱私前端，所以仍需有後端服務
    因無代理伺服器，你的 IP 會被 Youtube 看到
    _# 在意的話請翻 VPN、Tor_
* 目前在 Beta 公測，可能有 bug
    說是這麼說，但除了斷網會跳 bug 警示，鮮少碰到問題
* 不支援 SponsorBlock
    官方團隊說，業配屬「非侵入式廣告」，且對創作者來說是重要收入來源
    因此不納入考量，確實頗合理
    
支援多種語言，包括[正體中文](https://github.com/TeamNewPipe/NewPipe/blob/dev/doc/README.zh_TW.md)，不怕語言隔閡

### [Youtube ReVanced](https://vanced.to/)
常簡稱 ReVanced，不過 ReVanced 本身是個社群，推出各種 app
只是 Youtube ReVanced 特別受歡迎，因以為號焉

---

鑑於發展歷程精彩，來講古一下：
從前 Vanced 破解 Youtube 應用程式，用戶能免費享受無廣告、背景播放功能
但這種逆向工程違法，被 Google 警告後停止更新
後繼者 ReVanced 於是接手，改釋出「工具」給用戶
換句話說，破解是你破解的、擋廣告程式是你裝的，不關他們的事
_# 即「刀子放在路邊，是你自己拿去砍人的」_
程式碼[開源](https://github.com/revanced)、免費，沒有「不當獲益」的把柄給 Google 抓

---

缺點：
* 仰賴 Youtube，畢竟它只是應用程式
* 需手動「補丁」，有些技術門檻
不過[社群資源](https://www.reddit.com/r/revancedapp/comments/10nyr2t/complete_guide_frequently_asked_questions/)很多，也有[中文教材](https://ivonblog.com/posts/youtube-revanced/)，應該不是難事

### [LibreTube](https://libretube.dev/)
社群的[開源](https://github.com/libre-tube/LibreTube?tab=readme-ov-file)專案，用以替代 Youtube Android 應用程式
「號稱」可建播放清單、無廣告、支援 SponsorBlock、影片下載...
但使用 Piped API，可想而知只要 Piped 掛了就會跟著掛
_# Piped 又常常掛，所以 LibreTube 可用性難保證_
假設運作正常，則不會暴露 IP (畢竟連到代理伺服器)、輕量、保障隱私

缺點：
* 服務不穩定
    看得見吃不著，優點再多也沒用啊！

鑑於頗受歡迎，就還是提一下

---

果迷別急，接下來就該你們了
### [Yattee](https://github.com/yattee/yattee)
社群開源專案，不僅 iOS，Mac 也能用
原理是連到代理伺服器，獲取影片再傳給用戶
_# 代理伺服器通常是 Piped 或 Invidious_
無廣告、免費，可背景播放、懸浮視窗播放，也支援 SponsorBlock
為掩人耳目 (？)，Yattee 剛下載會發現只能播放本機影片
但別擔心，把站台網址加進去就能用了

缺點：
* 非全自動化，下載完尚需手動初始化站台 (代理伺服器端點)
    不知道怎麼加的，可參閱[中文教學](https://ivonblog.com/posts/ios-yattee/)
* 仰賴 Invidious 或 Piped 服務，可想而知很不穩定

### [YTLitePlus](https://ytliteplus.github.io/)
社群有 [YTLite](https://github.com/dayanch96/YTLite?tab=readme-ov-file) 和 [YTLitePlus](https://github.com/YTLitePlus/YTLitePlus)，兩者皆開源
都是 iOS Youtube app 的修改版，堪稱 iOS 版的 ReVanced
前者極簡、重效能，所以僅有背景播放、去除廣告、下載影片等核心功能
後者除基礎功能，還有 OLED 暗色模式、倒讚、iSponsorBlock...
_# iSponsorBlock 就是 iOS 版的 SponsorBlock，用於移除業配片段_

缺點：
* 服務不穩定，偶有用戶[反映](https://www.reddit.com/r/sideloaded/comments/1l82ke3/ytliteplus_not_working/)當機
* 使用者較小眾，維護、更新的頻率都較低
    也因為用的人少，可能有潛在優 / 缺點沒被我查到
    如果你用後發現極大亮點、或大爛 bug，歡迎補充

---

再來就是其餘~~人口~~裝置
### [SmartTube(Next)](https://smarttubeapp.github.io/)
給 Android 電視的 Youtube app 開源替代品，主要開發者為烏克蘭人
近期改名叫 SmartTube，兩者是[同一回事](https://smarttubenext.com/faq/)
基本上就是「電視版 Youtube ReVanced」，Android TV [相關設備](https://github.com/yuliskov/SmartTube#device-support)都支援
特色包括無廣告、整合 SponsorBlock、登入功能...，詳見[官方說明](https://github.com/yuliskov/SmartTube#-features)

缺點：
* 主要支援烏文、俄文、英文，其他語言可能要等
    _# 或是你去幫忙翻譯_
* [部分功能](https://github.com/yuliskov/SmartTube#-limitations)不穩定，或效果不佳
* 安裝、建置較麻煩，有技術門檻

### [Avideo](https://www.avideo.com/)
舊稱 YouPHPTube，可想而知使用 PHP 語法、生態系
開源，不過**背後是美國公司** WWBN (World Wide Broadcast Network, Inc.)
是「可自架的串流平台」，類似 PeerTube

缺點：
* 資安問題大，[漏洞](https://portswigger.net/daily-swig/vulnerabilities-in-open-source-streaming-platforms-youphptube-and-avideo-could-lead-to-rce)[層出不窮](https://github.com/Chocapikk/CVE-2024-31819)
    資安有破口，隱私便不保
* 美國公司所有，**受制美國政府**
    優點是開源，若有後門容易被發現

主要開發者蠻奇葩的，還在程式碼倉庫[傳教](https://github.com/WWBN/AVideo#first-thing)
論功能完整性、易用性、社群活躍與健全度，怎樣也是**選 PeerTube**
但人家開源，就還是提一下囉！

<br/>

---

<br/>

## 加碼！

### [Brave 瀏覽器](https://brave.com/zh-tw/download/)
想要零廣告、背景播放的 Youtube，直接裝 Brave 瀏覽器就行了
內建的廣告攔截器，就能給你絲滑體驗
且各大桌面平台、行動裝置，通通都支援
_# 這應該算公開的秘密了_
當正常瀏覽器用，也沒問題！

### [uBlock Origin](https://ublockorigin.com/)
簡稱 UBO，堪稱地表最強內容攔截器，是個瀏覽器外掛
能高效擋下追蹤器、廣告，卻幾乎不影響使用體驗
開源、完全免費，詳情見我的[瀏覽器介紹](./deGoogle-browser.md)
找個 Firefox 基底的瀏覽器，加裝 uBlock Origin，就進入無廣告世界啦！
_# 連 Youtube 廣告，也完全不會感覺到喔！_

### [Grayjay](https://grayjay.app/)
一言難盡，這是個程式碼公開的 Youtube 隱私前端
可訪問 Youtube、PeerTube 和 Odysee
然而 Grayjay 推出時，暫時使用 [FUTO 授權](https://discuss.privacyguides.net/t/grayjay-frontend/14616/2?u=jonah)
程式碼可取得，但**非開源**
_# 詳情請見[開源簡介](./open-source-intro.md)_
雖然只是暫時，但作者預計將來會[收費](https://discuss.techlore.tech/t/louis-rossmann-announces-grayjay-app/5838/2)
既不開源、也非免費，完全不符合 FOSS 定義，所以沒放到推薦圖中
順帶一提，應用程式裡有遙測喔！

社群有人推薦過 Tube PiP，是蘋果生態系的 Youtube 前端
雖然免費但**閉源**，因此不推薦

電腦版還有 [Youtbe Music](https://ivonblog.com/posts/th-ch-youtube-music/) (後改名 [pear-desktop](https://github.com/pear-devs/pear-desktop))，從官方 PWA 改來，有興趣者可參考
_# 手機可直接用 NewPipe、Yattee_

<br/>

---

<br/>

## 懶人包
* 一般用戶，以收看、收聽為主：
    * 想完全甩掉偷窺狂 Google → [Odysee](https://odysee.com/) / [PeerTube](https://joinpeertube.org/) / [DTube](https://d.tube/)
        看你追的創作者在哪，就選那個平台
    * 線上訪問 → [Invidious](https://invidious.io/) / [Piped](https://piped.video/)
        瀏覽器用 [Brave](https://brave.com/zh-tw/download/)，或 [Firefox](https://www.firefox.com) 系列 + [uBlock Origin](https://ublockorigin.com/) 也行
    * Android 用戶 → [NewPipe](https://newpipe.net/)
        有技術能力者可選 [Youtube ReVanced](https://vanced.to/)
    * 想要電腦應用程式 → [FreeTube](https://freetubeapp.io/)
    * iOS 用戶 → [Yattee](https://github.com/yattee/yattee) / [YTLitePlus](https://ytliteplus.github.io/)
    * Android TV 使用者 → [SmartTubeNext](https://smarttubeapp.github.io/)
* 內容創作者
    * 開發者，想自架服務 → [PeerTube](https://joinpeertube.org/)
    * 想多拿點收益 → [Odysee](https://odysee.com/) / [DTube](https://d.tube/)
        不過 [DTube](https://d.tube/) 有點難用，[Odysee](https://odysee.com/) 比較友善

    流量都在 Youtube 怎麼辦？
    經營多個平台，靠 Youtube 引流到 [Odysee](https://odysee.com/) / [PeerTube](https://joinpeertube.org/) / [DTube](https://d.tube/) 囉！

---

用廣告攔截器，看似損害創作者
但形塑這種生態的，正是平台本身
嚴格來說，是 Youtube 在壓榨內容創作者、把用戶當韭菜割
利用壟斷優勢做不當行為，大眾走灰色地帶剛好而已
想像自來水收費十倍漲，9 成 9 民眾根本沒替代選項
何況 Youtube 盈利來源是**內容**，由創作者產生
結果還要被削一大筆，錢太多請拿去[助人](https://www.msf.org.tw/)，別餵給貪婪企業

有個影片平台 Dailymotion，為何沒被替換掉？
因為它的聲量有點低，我不講你恐怕也沒聽過
放到圖上大肆批評，反而可能有廣告效果，因此略過

---

為了以身作則，我也把 [Youtube](https://www.youtube.com/@%E9%81%8A%E8%95%A9%E8%80%85) 頻道搬遷至 [PeerTube](https://video.hardlimit.com/c/aibycter/videos)、[Odysee](https://odysee.com/@%E9%81%8A%E8%95%A9%E8%80%85:4) 了
全都免費觀看，歡迎捧場 (不看也無所謂)




