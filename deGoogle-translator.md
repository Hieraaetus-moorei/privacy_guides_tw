# deGoogle - 替換翻譯軟體  

> 要你逐字翻，還不如丟 Google 翻譯  

撇除正確性問題，Google 翻譯也存在安全、隱私[風險](https://naipnews.naipo.com/17095)  
此服務沒出過大事，但[隱私權政策](https://policies.google.com/privacy?hl=en-US)都有載明  
用戶內容可能被用於「個人化廣告」、「改善服務」、「開發新產品」等  
意思是，最好別用 Google 翻譯處理機敏文件  

重視隱私者，也應儘量避免  
畢竟把一堆資料交給單一實體 (Google)，是非常危險的  
別忘了，Google 十分擅長[違法蒐集個資](https://www.reuters.com/sustainability/boards-policy-regulation/google-hit-with-314-million-us-verdict-cellular-data-class-action-2025-07-01/)  

### 「圖」個方便  
[deGoogle translator](image link)  
^圖源：不用想，當然是我^  
^FOSS^ ^指免費開源軟體^ ^(^^Free^ ^and^ ^Open^ ^Source^ ^Software^^)^  
^privacy^ ^proxy^ ^為保護隱私的代理服務，但仍仰賴^ ^Google^ ^翻譯^  

### 該換掉的服務  
撤換 Google、[百度](https://www.reuters.com/technology/cybersecurity/chinas-baidu-denies-data-breach-after-executives-daughter-leaks-personal-info-2025-03-20/)翻譯，可能沒太多疑慮  
兩者都非開源、由[隱私爭議](https://www.sixthtone.com/news/1016839)[不斷](https://www.chosun.com/english/industry-en/2024/09/23/REM66Q63QRDX3AOXEIEBVSJHLE/)的企業維運  
但不少台灣人，可能已習慣「沉浸式翻譯 (Immersive Translate)」  

什麼，那也有風險嗎！？  

![shocked meme gif](https://media.tenor.com/SpCaZonGbLUAAAAC/joey-shocked.gif)  


沒錯，而且跟百度是同個等級  

#### 沉浸式翻譯 - 資安風險  
* 公司背景  
    [沉浸式翻譯](https://ithelp.ithome.com.tw/m/articles/10364522) 2023 年被「[推文科技](https://news.qq.com/rain/a/20230525A02W6N00)」收購，推文科技是中國公司  
    海外市場由 Funstory.ai Limited 負責，登記在香港 (本質上是同家公司)  
    _# Funstory.ai Limited 為推文科技 2020 年[在港註冊](https://www.ltddir.com/companies/funstoryai-limited/)的「海外實體」_  
    服務條款也誠實[標示](https://immersivetranslate.com/zh-TW/docs/TERMS/)，自己是**中國公司**  
* 隱私條款  
    沉浸式翻譯自家[隱私條款](https://immersivetranslate.com/docs/PRIVACY/)，寫著：  
    * 網頁翻譯時，會將內容傳送給第三方 (你選的翻譯引擎)  
    此屬合理，因為它是橋接器，把網頁內容丟給翻譯引擎，再回傳結果給你  
    有點類似翻譯外包，沉浸式翻譯當郵差  
    第三方包括、Google、微軟、Qwen (阿里巴巴)...  
    那些公司的[黑歷史](https://phys.org/news/2018-01-china-alibaba-customer.html)，可說十分「[輝煌](https://www.cpomagazine.com/cyber-security/web-scraping-on-alibabas-taobao-resulted-in-data-leak-of-1-1-billion-records/)」  
    * 收集的個資 (metadata)  
        * 各功能使用頻率  
        * 裝置 ID  
        * 瀏覽器版本  
        * IP  
        * Email (若有登入)  
        * 上傳的檔案、偵錯日誌，號稱用於「改善服務」(Google 也常這麼說)  
    用個翻譯，交出如此個人化的資訊，似乎不太划算  
    * 第三方共享  
Mathpix：翻譯 PDF 時，會將檔案傳給 Mathpix 以獲得維持排版的結果  
**Google** Analytics、Adjust、**Meta** Pixel  
    沒錯，就是 Google 和 Meta，人家要靠廣告賺錢哪！  
    Adjust 是美國公司 AppLovin 的產品，用於分析行動裝置活動 (e.g. 廣告歸因)  
    * 權限  
        * 沉浸式翻譯瀏覽器外掛，取得的是 <all_urls>  
        意思是「能閱讀並修改你開啟的**所有**網頁內容」，電商、網銀也不例外  
        蘋果瀏覽器 Safari 還會警告用戶，該外掛「可讀取信用卡等敏感資訊」  
        想清楚再裝吧！  
        * 它的手機 app 可就更有趣了，要求一堆權限：  
使用網路、存取檔案、定位、相機、麥克風、剪貼簿、已安裝 APP 清單  
當然號稱是「翻譯用途」，但權限大，風險就高  
    * 出包歷史  
別以為新公司，就沒出過事  
        * 網頁 Snapshot 分享功能，曾將翻譯成果上傳騰訊雲端，並允許搜尋引擎建索引  
什麼意思呢？  
一、你的內容跑進騰訊雲了，而騰訊是中國公司  
二、搜尋引擎建索引，代表[別人能搜尋到你的翻譯內容](https://www.techbang.com/posts/124832-immersive-translation-security-flaw)，[形同公開](https://stable-learn.com/en/immersive-translate-2025-security-incident/)  
    如果翻譯重要文件、網頁，用 Google 都查得到喔！  
    * 曾想限制第三方 API，強制用戶都用他們的服務  
社群諷刺此舉是故意收割 API 金鑰，然後再說不能用  
太過依賴單一產品，就得承擔「養 → 套 → 殺」風險  
 養：先開放給你用，免費、自由度高  
 套：用戶固著，不容易隨便棄船  
 殺：收割行為，例如收費、限縮權益、置入討厭的功能 (但能賺錢)  
_# 順帶一提，養套殺方面 Google、Meta 和微軟可是行家_  

---

給開發者：  
沉浸式翻譯搞「假開源」，從[別人的專案](https://github.com/FilipePS/Traduzir-paginas-web)建立分枝 (fork)，修改成[初版](https://github.com/immersive-translate/old-immersive-translate)  
但初版程式碼已封存，沒意外不會再更新 (截稿時末次修改在 2 年前，只改了 readme)  
新版的呢？  
創了個[新倉庫](https://github.com/immersive-translate/immersive-translate)，裡面卻只有文件和版型，根本空殼  

---

更重要的是，設立在哪國就適用該國法律  
中國有多條法令，能讓政府向企業索取資料 (詳見我[另一篇](./chinese-service-risk.md)簡介)  
何況兩岸關係微妙，對岸政權動機充分  

#### Grammarly  
![Grammarly ad gif](https://media.tenor.com/wDaTHbaIeogAAAAC/spelling.gif)  
你可能看過這個廣告，它就是 Grammarly  
用途是修改文法、給寫作建議  
由三位烏克蘭人創辦，後在美國成立公司，因此算**美國企業**  
軟體架在 AWS (亞馬遜雲端)上，資料也是  
鑑於閉源，只能透過 Grammarly [隱私政策](https://www.grammarly.com/privacy-policy-november-2024)一探究竟：  
    身為文法檢查軟體，當然會蒐集寫作資料  
    幾乎只要是你打的內容，都會被記錄  
    因此社群有[不少人說](https://news.ycombinator.com/item?id=30470457)，Grammarly 是[鍵盤側錄器](https://www.reddit.com/r/privacy/comments/toskoq/grammarly_is_a_keylogger/) ([keylogger](https://medium.com/@Anthony-Lam/grammarly-might-be-the-most-polite-keylogger-ever-made-05027b4c54d1))  
    Email 內文、主旨、收件人、Slack 頻道名稱等項目，也會收集  
    使用者的互動內容，預設拿去練 AI 模型、改進產品 (歐盟、英國用戶除外)  
    資料「一年內」去識別化，之後最長留存「 13 個月」，實在太久  
    Cookie 和個資，會與廣告夥伴合作使用  
    _# I.e. 拿你的資料推廣告，有沒有很眼熟啊 (Google、Meta)？_  
    也因為追蹤功能，常跳出[過多](https://100mediaflow.com/article/3751)視窗、建議  
    佔據大量資源，拖慢電腦效能  
閉源美企，隱私政策也不友善，就換掉吧！  

### 替代選項  
#### [Lingva Translate](https://lingva.ml/)  
~~凌華翻譯~~ (沒人那樣叫)，是社群發起的[開源](https://github.com/thedaviddelta/lingva-translate)、非營利專案  
_# Lingva 自己翻成「語言翻譯」，因 Lingua 是拉丁文「語言」之意_  
[主要開發者](https://github.com/thedaviddelta)多為[歐洲人](https://github.com/thedaviddelta/lingva-translate/graphs/contributors)，重視開源和隱私  
原理是提供中間層，代替用戶訪問 Google 翻譯、再回傳翻譯結果  
Lingva 不蒐集機敏個資，也不將之傳給 Google  
本質上形同 Google 翻譯，但多了隱私保障  
_# 稱為[隱私代理伺服](./deGoogle-search-engine.md)：敵國很可怕，但信使幫你跑這趟_  
代理伺服器可自架，也有[官方](https://lingva.ml/)、[志願者](https://github.com/thedaviddelta/lingva-translate?tab=readme-ov-file#instances)的服務  
缺點：  
* 依賴 Google 翻譯，內文仍會被 Google 看到  
    _# 使者替你犯險，但還是得讓對方讀信，不然怎麼回覆？_  
* 翻譯品質就是 Google 翻譯水準 ~~(啊它就 Google 翻譯，不然你想怎樣？)~~  

習慣用 Google 翻譯的人，可以無痛轉換  
至少拿點隱私回來，又不會犧牲太多體驗  

#### [LibreTranslate](https://libretranslate.com/)  
社群自主開發的專案，靠 [Argos Translate](https://github.com/argosopentech/argos-translate/) 引擎驅動，非營利  
LibreTranslate 自己翻成「自由翻譯」，「Libre-」前綴是拉丁文的「自由」  
靠機器學習模型翻譯，但用的是開源、自架的模型  
能翻譯文字、檔案，也可[訂閱](https://portal.libretranslate.com/)獲得 API 金鑰  
伺服器可[自架](https://github.com/LibreTranslate/LibreTranslate)、也有[官方服務](https://libretranslate.com/)，要包自己的 API 服務也行  
幾乎可說是「人人能架設的翻譯服務」  
缺點：  
* 尚待發掘，歡迎讀者補充  

介面簡潔乾淨，也很直觀，不妨試試  

#### [SimplyTranslate](https://simplytranslate.org/)  
直翻「簡單翻譯」，同樣是[社群](https://codeberg.org/ManeraKai/simplytranslate)非營利專案  
其為隱私前端，連接至 Google 翻譯 (和 Lingva 類似)  
_# 已可改選 iCIBA、Reverso 翻譯引擎_  
[應用程式](https://f-droid.org/packages/com.simplytranslate_mobile/)只有 Android 版，網頁版則瀏覽器都能訪問  
缺點：  
* 頁面設計較舊，方便性不若其他選擇  
* App 只有 Android 版  
* 仍依賴 Google (或其他第三方翻譯)  

適合原本有裝 Google 翻譯的 Android 用戶  

#### [Linguist](https://linguister.io/)  
社群創立的[開源專案](https://github.com/translate-tools/linguist)，主要作者之一是賽普勒斯人  
Linguist 為瀏覽器外掛，提供「離線翻譯」功能  
也支援 ChatGPT、DeepL、Yandex 等翻譯服務，但就非離線   
_# 線上服務的缺點，就是第三方會拿到你翻譯的內容_  
本地翻譯使用「香檸翻譯器 ([bergamot-translator](https://github.com/browsermt/bergamot-translator))」，同樣開源  
_# 好處是資料只經過你的電腦，沒外人會看到_  
如果是開發者，也能架個 LibreTranslate 提供 API 給 Linguist 用  
功能很全面，可翻譯：  
* 輸入的內容  
* 整個網頁  
* 反白文字  
* Netflix 字幕  
* 私人訊息  
* ...  
亦可儲存個人字典、唸出譯文  

缺點：  
* 若選第三方服務，仍會交出資料 (但那是用戶自己選的，嚴格來說不算缺點？)  
* 僅支援 [Chrome](https://chromewebstore.google.com/detail/linguist-web-page-transla/gbefmodhlophhakmoecijeppjblibmie)、[Firefox](https://addons.mozilla.org/en-GB/firefox/addon/linguist-translator/) 外掛商店，Safari 無福消受  

定位像「開源版的沉浸式翻譯」，但不局限於中文 (支援 130 種語言)  

#### [Harper](https://writewithharper.com/)  
[社群開發者](https://elijahpotter.dev/)做的文法檢查工具，主打[開源](https://github.com/automattic/harper)、重隱私 (本地運作)、高效能  
可完全離線運作，資料不離開你的電腦  
由 Rust 編寫，執行效率極高  
類似 Grammarly，但更快、更輕量、更保障隱私  
本身以外掛形式推出，兼容於許多軟體  
[Firefox](https://addons.mozilla.org/en-US/firefox/addon/private-grammar-checker-harper/)、[Chrome](https://chromewebstore.google.com/detail/private-grammar-checker-h/lodbfhdipoipcjmlebjbgmmgekckhpfb) 商店、[VS code](https://marketplace.visualstudio.com/items?itemName=elijah-potter.harper) (程式開發工具)、Obsidian 都能用  
缺點：  
* 現為美國公司 [Automattic](https://github.com/Automattic) 所有 (專案被收購後，作者也加入該公司)  
Automattic 創辦人之一，也建立了 [WordPress](https://wordpress.org/)、並構築周圍生態系  
_# WordPress 是知名開源部落格工具_  
鑑於 Harper 開源、離線運作，該公司也尚無隱私爭議，仍值得推薦  

#### [LanguageTool](https://languagetool.org/)  
直翻為「語言工具」，可協助文法、拼字檢查，和文章改寫  
_# 類似 Grammarly 或 DeepL Write_  
有官方網站服務，和支援各種軟體的外掛  
例如[瀏覽器](https://addons.mozilla.org/en-GB/firefox/addon/languagetool/)、[Office](https://languagetool.org/insights/post/product-libreoffice/#how-to-enable-languagetool-on-libreoffice)、[Email](https://languagetool.org/thunderbird)、[iOS app](https://apps.apple.com/us/app/languagetool-grammar-checker/id1534275760)，以及[桌面版](https://languagetool.org/mac-desktop)  
免費版即享多數服務，也可付費訂閱  

---

公司背景：  
德國計算語言學者所創，公司設立於德國漢堡  
因在歐盟境內，適用歐盟隱私法規  
2023 年初被**美國**公司 Learneo 收購，法定資料主體也在同年底移替  
Learneo 併購後，仍維持 LanguageTool 的開源性，且號稱不會拿用戶資料練 AI 模型  
不過 Learneo 前身 Course Hero，曾出過[隱私爭議](https://www.insidehighered.com/news/2022/02/15/course-hero-contends-student-privacy-concerns)  
_# 鼓勵學生上傳機敏內容，以獲得免費獎勵。但移除流程、授權條款不友善_  
* 偵錯、記錄工具和許多第三方[合作](https://assets.coursehero.com/privacy-policies/privacy_policy_master.html)，包括 FullStory、Amplitude 和**微軟** Clarity  
    可能蒐集 IP、裝置資訊、互動行為與按鍵記錄  
    雖侵入性，但至少做到透明、揭露  
* 改寫功能與模型供應商合作，例如 OpenAI、Aleph Alpha  
* 雲端用 Cloudflare、AWS、Google Cloud  

---

缺點：  
* 美國公司擁有  
* 改寫功能合作企業，對隱私很不友善 (e.g. OpenAI)  
* 速度較 Harper 慢、所需資源較多  
    [Harper](https://writewithharper.com/) 說法，速度差距 50 倍以上 (但都比 Grammarly 快)  
* 自行架設的社群版，幾乎只有免費功能  
    畢竟他們想要你付錢哪！  
* 網頁很繚亂  

---

### [DeepL](https://www.deepl.com/en/translator)？  
DeepL 前身是 Linguee 字典服務，累積許多高品質資料  
後來訓練了人工神經網路 (AI 模型)，提供優質翻譯  
2017 年改名為 DeepL，成為專業翻譯知名品牌  
旗下有：  
* [DeepL Translator](https://www.deepl.com/en/translator) (翻譯)  
    類似 Google 翻譯，但品質好很多，還能[翻譯檔案](https://www.deepl.com/en/translator/files)  
* [DeepL Write](https://www.deepl.com/en/write) (改寫工具)  
    用於檢查文法錯誤、提供修訂建議  
    亦可改善文風、措辭語氣，讓內容更道地  
    品質非常高，甚至可用於論文、商業文書撰寫  
* [DeepL Voice](https://www.deepl.com/en/products/voice) (語音處理)  
    即時語音翻譯，或為語音產字幕  
      
有網頁服務、瀏覽器外掛、Office 整合等  
亦提供 API，對開發者算友善  
雖為付費服務，但也有免費版  
對散戶來說，免費版就很夠用  

那為什麼不推薦呢？  

DeepL 付費版[遵守歐盟 GDPR](https://www.deepl.com/en/pro-data-security)，資料僅存於記憶體、客戶端，且不用於模型訓練  
翻譯完成即刪除資料，不永久儲存  
_# 通過 ISO/IEC 27001 與 SOC 2 Type II，也合規於 HIPAA (可進美國醫療場域)_  
伺服器主要部署在歐洲、傳輸有 TLS 加密，防止第三方竊取  

！！！但是！！！  

免費版的互動資料，會被用於改善服務、訓練模型  
雖匿名化蒐集，依舊不適合上傳機敏資訊  
**那些美妙的個資保護，是付費用戶 (DeepL PRO)才有的福利**  
_# 但對免費戶的隱私政策，仍比 Google 翻譯友善得多_  
且 DeepL **非開源**，無法審視原始碼  
不能檢查，如何相信他們的承諾呢？  

---

### 懶人包  
* Google 翻譯愛好者 (有這種人？)：  
    * 習慣至特定網站翻譯 → [LibreTranslate](https://libretranslate.com/) / [Lingva Translate](https://lingva.ml/)  
    * 想下載手機應用程式 → [SimplyTranslate](https://simplytranslate.org/)  
    _# 只有 Android 版_  
_# 若身為開發者，不妨自架伺服器_  
* 開發者，有翻譯 API 需求 → [LibreTranslate](https://libretranslate.com/)  
* 想替換「沉浸式翻譯」外掛 → [Linguist](https://linguister.io/)  
    Linguist 亦可自架翻譯服務，或完全本地運作  
* 想替換 Grammarly 者 → [Harper](https://writewithharper.com/) / [LanguageTool](https://languagetool.org/)  
* 開發者，會在 IDE 寫文件 → [Harper](https://writewithharper.com/)  
* ~~盤子、傻子~~不排斥付費、閉源產品者 → [DeepL **PRO**](https://www.deepl.com/en/pro)  
    _# 沒訂閱的話，資料一樣會被拿去練 AI 唷！_  

---

若「Google 翻譯」在你瀏覽器書籤裡，可以現在就換掉它  

