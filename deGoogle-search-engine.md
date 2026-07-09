# deGoogle - 替換搜尋引擎  

> 欸，Google 一下美國又用關稅勒索了什麼  

日常生活中，是不是很習慣用「Google」直接替代「搜尋」呢？  
外國人也是，用「Google」當「search」的替代詞，似乎再正常不過  
此般盛況，可見 Google 市佔率多高 (中國人說「百度一下」也是同理)  
_# Google 甚至曾[呼籲](https://www.nbcnews.com/technolog/no-googling-says-google-unless-you-really-mean-it-1c9078566)不要亂用他們的名字，但顯然沒人理_  
如果你的瀏覽器首頁、預設搜尋引擎都是 Google，那你應該很熟悉上述情景  
有些人甚至不知道，世上除了 Google 還有其他搜尋引擎  

---

### 其他搜尋引擎  
你可能聽過 [Bing](https://joindeleteme.com/is-site-safe/is-bing-safe/)、Yandex、百度等搜尋引擎，但此處「**不會**」仔細介紹它們，因為那些也是[隱私陷阱](https://www.bankinfosecurity.com/researchers-meta-yandex-broke-android-privacy-a-28578)  
別忘記這趟旅程，目的是填平隱私坑洞、選擇更好的替代品  
不囉唆，直接上圖：  
[deGoogle search engine](image link)  
^圖源：我辛苦做的^  
^圖中的「tracker-free」，指前端無可見追蹤器，意思就是至少不公然追蹤你^  
^non-profit^ ^不是指「非營利機構」，而是「不以盈利為目的」^  
左方的 Google、百度、Bing 是欠換的引擎，右邊的替代選項稍後會一一介紹  
此處須先聲明，為何不全都用高隱私、開源產品替代  
因為搜尋引擎的本質是資料庫，透過建立索引讓搜尋者找到特定內容，同時還提供排序  
類似為書中每個章節編碼，並放到目錄頁  
也就是，幾乎得爬下整個網際網路，並用特定演算法將內容歸類、排序  
開發和維運都所費不貲，現階段無單一機構提供「不收費」、「保護隱私」、「開源」、「獨立」全數涵蓋的服務，只能適度妥協  
右半邊的替代品，至少符合「免費」、「相對重視隱私」，也有些是開源  
除 Whoogle 外，其餘選項都有瀏覽器外掛，可取代網址列的預設搜尋引擎  
_# 許多瀏覽器也支援在設定中，手動替換預設搜尋引擎_  

那就開始吧！  

### [Searxng](https://github.com/searxng/searxng) (前身為 [Searx](https://github.com/searx/searx))  
Searxng 是社群建立的開源專案，也就是一群人自發合作，**無**商業機構撐腰  
它是整合搜尋 (meta search)引擎，沒有自己獨立的索引 (index)，但會從各大搜尋引擎如 Google、Bing 抓取結果，混合後送給使用者，例如這樣：  
[wechat data breach](image link)  
^圖源：本人搜尋結果^  
因為開源，各項設定皆可自訂，搜尋結果也較不易受單一引擎影響  
你可能會問，結果來自 Google、Bing，還有隱私可言嗎？  

有！  

Meta search 的好處就是，作為使用者的「代理伺服器」向各引擎發送請求  
什麼意思呢？  
就像你叫別人幫你找資料，Google 蒐集到的資訊，來自**幫你搜尋的人**，不是你  
而且代理伺服器，任何人都能自行架設 (只要你有資源)，不必受制於誰  
值得注意的是，如果該代理伺服器只有你一人使用，那就幾乎形同你自己做搜尋，只是換台電腦而已  
理想的做法是，找個多人使用的實例 ([instance](https://searx.space/))當代理，讓大家的資訊混雜在一起，不易個別追蹤、也不用自己花錢架設  
什麼！？哪有人那麼好心，免費架代理伺服器給大家用？  
就是有，別小看重視隱私的人、機構，有些機構純粹追求「隱私是基本人權」，而無償提供服務  
有些人則是想保障自己隱私，但單獨使用形同沒保護層，於是公開給世人用，順路保障自己  

### [~~Mullvad Leta~~](https://leta.mullvad.net/)  
**Mullvad 公司表示，將不再維運此服務**  
Mullvad 是一家瑞典 VPN 公司，推出很多開源、保障隱私的產品  
Mullvad Leta 是他們的代理搜尋引擎，「Leta」是瑞典文的「搜尋」  
原理和 searxng 差不多，但介面比較友善，不過代理的對象只有 Brave search 和 Google  
目標用戶比較像大眾，而非開發者  

### [Whoogle search](https://github.com/benbusby/whoogle-search)  
Whoogle 是個取名很針對的代理搜尋引擎，可想而知是衝 Google 而來，連首頁都十分神似  
這也是社群自發的開源專案，沒公司撐腰、可自行架設  
官方程式碼倉庫有列出幾個[實例](https://github.com/benbusby/whoogle-search/blob/main/misc/instances.txt)，有些已下線，可自行試試  

接下來要介紹的，就都是**非開源**的了  

### [Brave search](https://search.brave.com/)  
你可能聽說過 [Brave 瀏覽器](./deGoogle-browser.md#brave-browser)，就是被大家當 Youtube premium 的那款  
沒錯！是同一家美國公司！  
Brave 有「自行建立」的索引，只有在搜尋結果不佳、內容過少時，才會導入其他引擎的結果  
前端沒追蹤器、支援 AI 摘要、有適量可自訂功能，且隱私政策友善，算還不錯的替代品  
從前 Brave search 很難用，但改進非常快，現已體驗良好  
缺點：  
* 非開源，無法驗證隱私政策是否落實  
* 美國公司，會不會被國家要求提供資料，難以保證 (莫忘 PRISM 稜鏡計畫)  
* ~~使用加密 VPN 的話，可能會陷入無止盡機器人驗證~~  
    _# 似乎已解決_  

Claude 的搜尋 API，就是[用 Brave search](https://odysee.com/@techlore:3/only-3-search-engines-actually-exist:7) 呢！  

### [Ecosia](https://www.ecosia.org/)  
嗯，看名字就知道，這家德國社會企業很重視環境  
Ecosia 是個代理搜尋引擎，從 Bing 獲取結果，靠非個人化廣告獲利  
利潤全用在改善環境，尤其是種樹，所以如果你在乎環保，不妨把它換成預設搜尋引擎  
_# 他們真的有做，這家企業的好處就是透明，捐助了什麼機構、在哪造林都能查到_  
缺點：  
* 有 10 個以下的可見追蹤器  
* 隱私政策說明：「用戶資料會在一週內去識別化」，意思就是他們會蒐集 IP、搜尋內容等，但會在一週內將之斷開，僅知道有人搜尋什麼、用戶來自哪裡，但兩者配不起來  
_# 有些人可接受，但「一週」對我來說太久，明明可以不蒐集、或即時解耦  
所以我幾乎不用 Ecosia，因為`隱私不容妥協，不論任何原因`_  
* 搜尋結果不佳，畢竟是來自~~破 Bing、有 Bing~~ Bing，微軟的搜尋引擎實在...  

現在也有 AI 模式，運作都是靠再生能源，但畫面渲染頗陽春  

### [Mojeek](https://www.mojeek.com/)  
這是家英國公司，**有獨立索引、也可當代理搜尋引擎**，且[隱私政策](https://www.mojeek.com/about/privacy/)非常簡短、友善  

不該拿的資料，幾乎都不拿  

對使用者，僅定位到「國家」層級，以提供較好的搜尋結果 (Google 可是連你在哪個行政區，都會知道)  
獲利來源是非個人化廣告，網頁無可見追蹤器，算很棒的選擇  
你可能會擔心，[英國對隱私很不友善](https://www.bbc.com/news/articles/cgj54eq4vejo)，不怕出事嗎？  
若 Mojeek 有落實自家隱私政策，就不必擔心  
因為它遵守歐盟 GDPR、不記錄使用者個資，[官方說](https://blog.mojeek.com/2020/12/frequently-asked-questions-about-mojeek-business-model-surveillance-privacy.html)「就算政府來要，他們沒記錄的東西如 IP，還是給不出來」，所以別怕！  
一般搜尋模式介面類似傳統搜尋引擎，「summary」則會有 [AI 摘要](https://blog.mojeek.com/2024/04/mojeek-search-summary.html)  
缺點：  
* 有個很致命的缺點：非英語系的網頁幾乎都未建索引，意思是不支援中文搜尋  
_# 我在社群問過官方，他們說「還沒」建，但為日、韓、中文網頁建索引在計劃中_  
* 非開源之外，大概沒缺點了  

我搜尋英文內容時，也很愛用 Mojeek  


### [Startpage](https://www.startpage.com/)  
顧名思義，它希望代替 Google，變成瀏覽器首頁  
此公司歷史複雜，請容我細細說來  
起初 Starpage 是家荷蘭公司，提供保障隱私的代理伺服器，讓用戶安全連線至 Google search (沒錯，搜尋結果來自 Google)  
因為是荷蘭公司，所以遵守歐盟隱私法規，獲利來自非個人化廣告，且提供匿名造訪網站功能 (改從他們的 IP 進入網站)  
有 Google 等級的搜尋結果，又保障隱私，聽起來很棒吧？  
**注意了**，Startpage 後來被**美國廣告公司** System1 收購，儘管 System1 承諾不改變 Startpage 隱私政策、維持其獨立性 (被收購還獨立？)  
但 System1 是美國公司、主業還是廣告、Startpage 又沒開源，背後究竟怎麼做，誰知道呢？  

缺點：  
* 有可見追蹤器  
* 屬**美國廣告公司**、架構非開源  
* 沒獨立索引，仰仗 Google 結果  

### [DuckDuckGo](https://duckduckgo.com/)  
DuckDuckGo (直翻為**鴨鴨跑**，有點可愛 XD) 是知名隱私搜尋引擎，靠非個人化廣告賺錢 (官方宣稱)，幾乎可說是最早的 Google 替代品  
NSA 稜鏡計劃曝光後，創辦人成立 DuckDuckGo，隱私政策聲明「不追蹤個人化資訊」，誓言提供保障個資的選擇  
搜尋結果也加入「相對隱私」的 AI 統整，AI 來自主流供應商，但由 DuckDuckGo 提供代理橋接 (類似代理伺服器)  
_# 討厭 AI 的人可以手動關閉，或改選[無 AI 版](https://noai.duckduckgo.com/)_  
而且 DuckDuckGo 部分組件開源，和開發者社群整合良好  
不過 DuckDuckGo 是**美國公司**，首頁和搜尋結果頁也有數個可見追蹤器  
且旗下的閉源瀏覽器曾[開後門給微軟](https://cyberinsider.com/duckduckgo-browser-microsoft-tracking/)追蹤、投放個人化廣告，隱私保障不甚理想  
鴨鴨跑還有另一個輕量化產品，[DuckDuckGo Lite](https://start.duckduckgo.com/lite)，版面簡潔許多、沒可見追蹤器 (搜尋結果頁有一兩個)，也沒 AI 統整  
不論是 DuckDuckGo 還是輕量版，官方都宣稱「搜尋引擎」，不過它們其實是整合搜尋引擎 (meta search engine)  
主要結果來自 Bing、少量來自其他引擎 (現在知道為何後門是開給微軟了吧？)，並**無**獨立索引  
烏俄戰爭爆發後，鑑於俄羅斯媒體假訊息氾濫，DuckDuckGo 不再從俄國搜尋引擎 Yandex 獲取結果，因此更依賴美國企業  
缺點：  
* 有追蹤器  
* 美國公司，曾有劣跡  
* 無獨立索引，搜尋品質不若 Google (畢竟是 Bing)  

### 其他  
可能有人好奇，怎沒介紹 [Qwant](https://www.qwant.com/)、[Kagi](https://kagi.com/)、[MetaGer](https://metager.org/)？  
因為 Qwant 不支援台灣，本地 IP 無法使用  
Kagi 和 MetaGer 是**付費**服務，此處以免費替代品為主，所以暫不考慮  
_# Kagi 是**美國**公司，且**非**全開源_  
_MetaGer 則是**德國**非營利機構維運、**開源**的 meta search 引擎，若想付費也是選這個_  

---

### 總結  
~~總的來說~~ (這篇才不是 AI 寫的)，本文提供的是「替代搜尋引擎的詳細比較」，優缺點都揭露、不偏袒特定公司 (沒人付我錢哪 XD)  
至於選哪個，留給使用者 (對，就是你)決定  
若有選擇障礙，可參考以下指引：  
* 不想受制任何一方，可在最上排 Searxng、~~Mullvad Leta~~、Whoogle 擇一  
    _# 對一般用戶而言，Mullvad Leta 應該比較友善，可惜已停止服務_  
* 依任務選擇  
    _# 英語系的搜尋，可用 Mojeek_  
* 若可接受美國公司、又想有 AI 體驗，Brave search 是個權衡替代品  
* 覺得隱私「比 Google 好」就行、且熱愛環保的話，不妨考慮 Ecosia  
* 如果相信 System1 不會搞爛 Startpage，就用吧 (搜尋效果好，畢竟結果來自 Google)！  
* 是老牌鴨鴨跑粉絲、願意再次信任~~等著被背叛~~，就用 DuckDuckGo 囉！  

對習慣 Google 的人：  
DuckDuckGo、Brave、~~Mullvad Leta~~ 都支援 Google 的語法、[快捷鍵](https://duckduckgo.com/bangs)  
* 例如 `/` 進入搜尋列  
* Google `"侵害隱私"` 表示搜尋結果需包含「侵害隱私」  
* `!w` 直接進入維基百科  
* ...  
_# 第一次聽到嗎？那至少你也學會了_  

---

如上述內容有誤，歡迎指正  

