# deGoogle - 替換 email  

> 我加密我的郵件，因為隱私很重要 - ProtonMail  

老一輩可能有印象，從前 Gmail 打開都會有「信內廣告」  
使用者可曾想過，背後的疑慮？  
能因信件內容投遞個人化廣告，意味他們也能掃描你的信件，Google 還[直接承認](https://www.wsj.com/articles/techs-dirty-secret-the-app-developers-sifting-through-your-gmail-1530544442)，稱大部分企業都會掃描用戶郵件  
這種情況下，你收發的不是信件，是明信片 (誰想看都行)  
雖已在輿論壓力、競爭對手倡議下改善了不少，但[主流 email 服務商](https://www.vice.com/en/article/free-email-apps-spying-on-you-edison-slice-cleanfox/)，幾乎都仍可讀取你的信件內容  
尤其下載 app，又多一層疑慮  

你可能會擔心，現在辦各種帳號，幾乎都需要 email  
就算連動登入，也同樣會把個資交給 [Google](https://www.reuters.com/legal/google-settles-5-billion-consumer-privacy-lawsuit-2023-12-28/)、[Meta](https://www.bbc.com/news/articles/cx2jmledvr3o) 這類素行不良的企業  
Email 形同網路世界的身分證，又取代傳統書信成為正式聯繫管道  
若如此危險，個人隱私、憲法保障的「秘密通訊自由」，難道玩完了嗎？  
> 幾年之後它 (email)可能比我們的真實身分證明還要重要 - [嚴育銓](https://www.twreporter.org/a/protonmail-project)  

別急，替代品這不就來了：  
[deGoogle email](image link)  
圖源：~~做那麼精美~~當然是我  
^non-profit^ ^不是指「非營利機構」，而是「不以盈利為目的」^  
^FOSS^ ^指免費^ ^(^^free^^)^^且開源^ ^(^^open^ ^source^^)^^的軟體^ ^(^^software^^)^  
^皇冠是很推薦的意思，就算同為替代品，仍有出類拔萃者^  
### 端對端加密  
講解之前，先提一下「端對端加密 (end-to-end encryption, e2ee)」  
端對端加密是個「概念」，可用不同技術達成  
指使用特定方式加密，實踐「只有兩端使用者」才能看到內容  
白話文解釋：若我用支援 e2ee 的服務寄信給 Gorhill，則只有我和 Gorhill 本人看得到信件內容  
其他所有人，**包括 email 服務提供商**，都不知道我寫~~恐嚇信~~了什麼  

開始講圖吧！  

已知 Gmail 是[隱私惡夢](https://www.theguardian.com/technology/2013/aug/14/google-gmail-users-privacy-email-lawsuit)，但果粉可能會抗議：「iCloud 有端對端加密！」  
別急，開啟 Apple ADP (Advanced Data Protection)可讓 iCloud 獲得端對端加密  
但[蘋果自己說](https://www.zdnet.com/article/apple-is-bringing-end-to-end-encryption-to-icloud-backups-heres-what-it-means/)，iCloud mail **不受** e2ee 保護，何況加密演算法不明、程式未開源  
蘋果又和 Google、微軟一樣有 [PRISM 醜聞](https://www.theguardian.com/world/2013/jun/06/us-tech-giants-nsa-data)，當然也欠換  

至於第三個被換的，是微軟的 Outlook，我猜很多人沒聽過，畢竟市佔率低 (對，就是在笑它)  
Outlook 至今都還會塞廣告，而且頗難用  
但鑒於市占第三 (其實很低，Google 和蘋果瓜分了近 9 成市場 )，就給點尊重吧！  

### [Proton Mail](https://proton.me/mail)  
特別推薦這家，因為「加密郵件」的風潮，可說是由 Proton Mail 帶起的  
核心價值是「Privacy by default」，Proton 本質是家隱私保障公司  
他們當初披荊斬棘，還遭遇 Google [不當打壓](https://proton.me/blog/search-risk-google)，最後成功迫使各服務商重視隱私，推動數位人權  
Proton 的防護做得很完善：  
* 端對端加密 (Open PGP)，官方也看不到信件內容  
    如寄給 Proton 以外用戶，可設定密碼做加密  
    寄信時還能設定，多久以後該信自動焚毀 (從收件夾消失)  
* 程式碼開源，免費版已夠用  
    Proton 採訂閱制，藉以脫離「濫用個資的廣告商業模式」，但有免費版  
    _# 若支持他們的理念，不妨考慮訂閱，有很多額外功能_  
* 免費版就提供 email alias 服務，也就是轉寄地址  
    辦各種帳號時，可創個 alias 充當 email，信還是會寄到你的電郵地址，只是經過轉發  
    好處是不會暴露真實電郵地址，若發現地址外洩、對方亂寄廣告信，把對應 alias 刪掉即可，~~信就會寄到虛空~~  
    _# 此為整合 [SimpleLogin](https://simplelogin.io/) 的功能，用 Proton 帳號可登入 SimpleLogin  
    SimpleLogin 是法國人創立的**開源信箱別名服務**，收、發信件都能用別名 (假地址)_  
    白話文解釋：你住的社區有警衛統一收信，再由他分發信件給住戶  
    寄件人只知道警衛窗口，不知道你真實地址  
* 伺服器在瑞士地底，只有合乎瑞士法規的命令，他們才會配合 (美、中政府無法勒索)  
    瑞士是中立國，*從前*隱私保障很嚴格，不過近年在吵[監聽法案](https://tuta.com/blog/switzerland-surveillance-plan)，若通過會是場噩夢  
    _# Proton 說如果瑞士不再安全，就會令尋他處，且現已[開始投資歐洲](https://proton.me/blog/lumo-ai)_  
* 創辦人 Andy Yen 是**台灣裔**、原先為**物理學家**，和傳統貪婪商人不同  
    他就是本篇引言提到的嚴育銓，曾受台灣獨立媒體[訪問](https://www.twreporter.org/a/protonmail-project)  
* 有其他[整合雲端服務](https://proton.me/)，生態系相對完善 (日後會陸續介紹)   
    總之，Proton (質子科技)可謂隱私保護第一品牌  

### [Tuta Mail](https://mail.tutanota.com/?r=/login)  
名字很怪嗎？  
Tutanota 是家德國公司，Tuta- 為拉丁文的「安全」，Nota 則是「消息、訊息」  
後來為簡化品牌形象，2023 年改名 Tuta  
Tuta 和 Proton 性質十分類似，前端開源、訂閱制但有免費版、端對端加密等  
因市場棲位重合，兩邊常發文[隔空叫囂](https://tuta.com/best-protonmail-alternative)、遇到重大隱私事件又會合力譴責，互動十分有趣  
Tuta 所在的德國，算歐盟數一數二重視隱私的國家，畢竟有歷史因素  
_# 若展開大監聽，易落話柄：「想找出特定族群進行迫害」，例如**某些人種**_  
Tuta 的加密演算法，就算量子電腦問世仍屬安全 (學術圈有探討過，哪些演算法在量子電腦面前不堪一擊、哪些又能挺過)  
且信件採用 AES 256 加密，連主旨也受保護 (Proton 的 OpenPGP 也會加密主旨，但非端對端)  
**重視環保的看過來**，Tuta 服務 100% 由再生能源驅動，**環保可以從日常選擇做起！**  
缺點：  
* 有些介面不太直觀，可能要摸索一下  

如果你偏好下載手機 app，Tuta 可說是個好選擇  
因為多數其他 email 客戶端，「跳通知」功能來自 Google / Apple  
而 Tuta 用自家服務，所以沒閉源成分  
_# 因此可從 [F-droid](./deGoogle-appStore.md) 下載_  

### [Nextcloud](https://nextcloud.com/)  
Nextcloud 也是德國公司，產品 100% 開源，主張整合雲端服務**去中心化** (≈民主化)  
什麼意思呢？  
Nextcloud 很像 Google 雲端，有各種工具可用，全整合在一個服務中  
任何人皆可自行架設，且企業版和一般版「**沒有差別**」  
他們的商業模式，主要靠提供企業、政府解決方案，例如資安認證、客服、穩定版本維護  
簡單說就是賣服務，所以散戶不用擔心隱藏費用  
但此處要說明，Nextcloud 本身**沒有** email 功能，但能充當 email 前端  
意思是，你可以自架電郵伺服器、或導入某個既有電郵服務，以 Nextcloud 介面呈現  
缺點：  
* 仍須依靠其他服務  
* 有技術門檻  
* 端對端加密靠第三方外掛 Mailvelope 達成，非原生  

### Thunderbird  
Thunderbird 直翻雷鳥，是[開源](https://github.com/thunderbird)、可客製化、靠 OpenPGP 支援端對端加密的 email 前端  
欸別急著滑走，Thunderbird 很平易近人，到官網[下載](https://www.thunderbird.net/en-US/download/)軟體就行了  
此專案歷史悠久，起初由 Mozilla 基金會開發 (Mozilla 另一個代表作，是瀏覽器 [Firefox](https://www.firefox.com/))，後獨立出來，由 Mozilla 資助  
雲端郵件問世前，電子郵件多是由電腦中的 app 負責收發，每個 app 可能差異頗大  
就算雲端郵件出現後，下載各家 app 也得受制於該公司隱私政策、介面設計  
Thunderbird 就是負責提供「統一介面」，可收發所有來源的郵件  
白話文就是「萬用 email 前端」，不論你用哪家服務，通通都能用此 app 管理，有點像所有信箱都轉寄至此  
你可以把 gmail、iCloud mail、Yahoo mail (還有人在用的話) app 刪掉，全改以 Thunderbird 替代  
缺點：  
* 對 Gmail 的支援偶爾會有 bug  
* 只是前端，本身並非信箱服務 (須自備 email 帳號，只是 app 換成 Thunderbird)  

Mozilla 後來推出 [Thundermail](https://thundermail.com/)，企圖加入保障隱私的郵件供應商行列  
不過 Beta 測試很久仍無下文，我登記參與也遲遲未見回音  
若有讀者玩過，懇請分享一下感想  

### [Mailfence](https://mailfence.com/)  
Mailfence 直譯是郵件藩籬，本意是提供藩籬 (加密)的郵件服務  
該公司位於比利時，以 OpenPGP 處理端對端加密  
訂閱制但有免費版，服務也整合了月曆、文件功能 (但我沒用過)  
缺點：  
* 隱私政策[說明](https://mailfence.com/en/privacy.jsp)會蒐集 metadata，包括 IP、寄信人、收件人、時間戳記 (何時寄的)...  
* 服務**極不穩定**，有時會登入失敗，顯示「無此帳號」、有時則會將信件寄到異次元 (寄出即消失)，且客服難以聯繫  
* 垃圾郵件偶爾會擋過頭  
* 非開源，雖未出過大事，但無法檢核是否落實隱私政策、具有漏洞或後門  
    開源很重要，尤其 Mailfence 設立在 14 眼聯盟成員國，比利時境內  
    _# 5 眼、9 眼、14 眼等聯盟，是美英為首的跨國情報合作組織，由 CIA 這類情報局主導，所以有可能配合大監聽計劃_  

### [Mailbox](https://mailbox.org/en/)  
德國 email 公司，用 OpenPGP 做端對端加密  
外圍組件如垃圾郵件過濾器開源，**核心架構閉源**  
訂閱制、提供 30 天免費試用，似乎附帶線上文件編輯功能  
100% 用再生能源驅動，和 Tuta 一樣  
缺點：  
* $$$  
* 部分非開源  

_# 有 Proton 和 Tuta，選這家幹嘛？_  

<br/>

---

<br/>

### 總結~~來說~~  
明明非開源，為何 Mailfence 也被放進來？  
還有 Mailbox，並不符合「免費」定義  
因為好的電郵服務商太少了，只能把「堪用但不建議」的也納入  
資訊都揭露，至於是否要用，交給讀者們決定  
其他選項如 [Fastmail](https://www.fastmail.com/) 同樣是部分開源、訂閱制，且位於澳洲 (5 眼聯盟成員、法規對隱私來說是場夢魘)，風險過高就不介紹  
_# Assistance and Access Act [要求](https://secureprivacy.ai/blog/what-australia-privacy-act-reforms-mean-for-your-business-2025)企業[協助](https://cowellclarke.com.au/insights/do-australia-s-impending-law-reforms-mean-it-s-finally-getting-serious-about-privacy)調查、讓執法單位獲得數據等，否則罰錢_  

### 給懶鬼的建議  
個人推薦 [Tuta](https://mail.tutanota.com/login)、[Proton](https://proton.me/mail) 免費帳戶，都去辦個來玩玩  
喜歡何者就選它，兩個兼用也行，多一組郵件地址無妨  
如果嫌哪家 email 應用程式太爛，則可用 [Thunderbird](https://www.thunderbird.net) 代替  
不是開發者的話，不太建議搞 [Nextcloud](https://nextcloud.com/) 串接，你可能會崩潰 (？)  

---

如內容有誤，歡迎批評指教  

