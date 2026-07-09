# deGoogle - 替換日曆  

> 你有記得把時間加到 Google Calendar 上嗎？  

雖然 Google 宣稱不會用日曆內容推廣告，但仍會蒐集用戶資訊  
包括時間、事件標題、描述、參與者...  
_# 何況 Google 無信用可言_  
且無端對端加密，所以 Google 能輕鬆如意地拿到資料  
再者，Google 身為美國企業，若該國政府用[監聽法案](https://proton.me/blog/us-warrantless-surveillance)索取資料  
Google 極可能積極配合，不論要求是否合理  
畢竟 [PRISM](https://www.theguardian.com/world/2013/jun/06/us-tech-giants-nsa-data) 都跪過了，哪可能為了你得罪政府？  

#### 開換吧！  
[deGoogle Calendar](image link)  
<sup>圖源：隱私倡議者 - 我</sup>  
<sup>FOSS 指免費開源軟體 (Free and Open Source Software)，或開源、至少有長久免費版者</sup>  
<sup>End-to-end encryption 為端對端加密，僅當事人、經授權者能看到內容</sup>  
<sup>non-profit 指「不以營利為目的」，不是「非營利機構」</sup>  
除了 Google 日曆，Apple Calendar 也該換  
Apple Calendar [沒端對端加密](https://support.apple.com/en-us/102651)，即使開啟進階資料保護 (Advanced Data Protection, ADP)仍[不支援](https://support.apple.com/en-ca/guide/security/sec973254c5f/web)  
_# 端對端加密代表只有你、經授權者能看到內容，即便公司方亦無從窺探_  
蘋果曾參與稜鏡計劃 (PRISM)，過去也[不甚光彩](https://www.reuters.com/legal/apple-must-face-narrowed-privacy-lawsuit-over-its-apps-2024-09-27/)  
沒端對端加密、程式碼又閉源，實在不怎麼隱私  

替代品眾多，畢竟日曆不是什麼艱深科技  
更因如此，不必拘泥特定公司的~~噁爛~~產品  

#### [Proton Calendar](https://proton.me/calendar)  
沒錯，又是 Proton！  
專做隱私產品，自然常常出現  
Proton 是瑞士公司，從加密郵件起家  
_# Proton 品牌故事，可參見我[介紹 Email 的文章](./deGoogle-email.md)_  
日曆開源、端對端加密  
[免費版](https://proton.me/pricing)可創三個日曆，欲分享則須訂閱  
_# 訂閱可享有 Proton 生態系服務_  
缺點：  
* 免費版功能較少  
* 會蒐集意外資訊  
    _# 例如 app 當機、意外掛掉_  

#### [Tuta Calendar](https://tuta.com/calendar)  
就是做[加密 Email](./deGoogle-email.md) 的那家德國公司，Tuta，~~土塔~~ (官方沒這樣翻)  
幾乎什麼資料都不蒐集，日曆端對端加密、開源  
免費版可建單一自用日曆，訂閱則享更多服務  
![Tuta calendar vs Google calendar](https://tuta.com/assets/google-calendar-app-privacy-review.DCRafG9D_Z1NhQuq.webp)  
圖源：Tuta 日曆[介紹](https://tuta.com/blog/private-calendar-alternative-to-google#google-calendar-alternatives-tuta-vs-proton-vs-ourcal)  
官方的比較圖，可見左方 Tuta 不蒐集個資，右方 Google 日曆則搜刮一堆  
缺點：  
* 免費版功能較少  
* ~~過於安全~~  

#### [Nextcloud Calendar](https://apps.nextcloud.com/apps/calendar)  
同樣是熟面孔德國公司，Nextcloud  
產品百分百開源，體驗類似 Google 的整合雲端服務  
因可自行架設，日曆無端對端加密  
_# 你應該不必擔心，自己偷自己資料_  
缺點：  
* 自行架設有技術門檻  
* 無端對端加密  
    若和親友共享服務，則架設者有機會看到眾人資訊  

#### [Fossify Calendar](https://www.fossify.org/apps/)  
從名稱可知，想把東西變「開源免費」  
_# FOSS: Free and Open Source; Fossify: 把東西 FOSS 化_  
社群建立的免費、開源專案，可完全離線使用  
若欲同步日期、各種功能，須找到適當服務  
_# 其為 Android app，支援 CalDAV protocol_  
意思是，想更新日期、連結信箱的話，仍須串接線上服務  
和 Google、Nextcloud 等各種 CalDAV 伺服器相容  
缺點：  
* 同步功能須找服務支持，Google 或第三方都行  
    _# 你可以不同步，當離線 app 用_  
* 僅支援 Android  
* 無端對端加密  

Fossify 亦提供「聯絡人」、「檔案管理員」、「相簿」、「簡訊」等 app  

#### [Etar](https://github.com/Etar-Group/Etar-Calendar)  
開源、免費的社群專案， 用於替代 Google 日曆  
介面簡潔直觀，功能齊全  
_# 可用日、週、月檢視，有亮、暗主題..._  
能完全離線使用，若想同步則須連接線上服務 (和 Fossify 類似)  
缺點：  
* 只有 Android 版  
* 無端對端加密  
* 同步功能仰賴線上服務  
    _# 但可離線使用，不一定得同步_  

純粹替代 Google 日曆應用程式，很夠用  
且社群評價不錯，值得一試  

#### [DAVx<sup>5</sup>](https://www.davx5.com/)  
奧地利公司 bitfire web engineering 維運，遵守歐盟 [GDPR](https://gdpr-info.eu/) 隱私保護法規  
橋接線上服務和應用程式，用以同步日曆、聯絡人，可視為轉接器  
前述 Fossify、Etar 都能靠 DAVx<sup>5</sup> 連上想要的服務  
缺點：  
* 僅支援 Android  
* 無端對端加密  
    畢竟是轉接器，傳輸層加密比較合理  

#### [Thunderbird](https://www.thunderbird.net/en-US/calendar/)  
Thunderbird (直翻雷鳥) 是萬用郵件前端，可連接各家 email 信箱  
由 Mozilla 開發，後脫離成獨立專案  
開源、免費，各大桌面平台、Android 都可取得  

在這裡提 email app，跑錯篇了？  

別走！你聽我解釋 (八點檔戲碼)！  
從前官方外掛 lightning，賦予雷鳥日曆功能  
後來 lightning 被整入雷鳥，不必再另裝外掛  
意思是，下載 Thunderbird 就會有內建日曆  
可離線使用，也可連接線上服務以同步資訊  
缺點：  
* 非獨立日曆，跟郵件 app 同捆  
    對某些人可能是優點，兩個願望一次滿足  
    我[替換郵件](./deGoogle-email.md)那篇文，有介紹 [Thunderbird](https://www.thunderbird.net/en-US/)  
* 日曆無端對端加密  
* 尚無 iOS 版 (仍在開發中)  
    _# 官方[說法](https://blog.thunderbird.net/2025/06/thunderbird-mobile-progress-report-may-2025/)：預計 2025 年底進入 alpha 測試_  
#### [Cal.com](https://cal.com/)  
開源議程排定工具，由**美國公司**開發  
串接其他日曆服務，用以排定開會時間、設定提醒等  
產品定位是 Calendly 繼任者，提供較隱私友善、開源的選擇  
有個人用免費版，也可訂閱  
_# 核心以 AGPL [開源](https://github.com/calcom/cal.com)、部分企業版功能需商業授權，個人用途基本上可自架_  
缺點：  
* 僅協調議程排定，無完整日曆功能  
* 美國公司所有、無端對端加密  
    _# 鑑於開源、相對友善的隱私政策，才提此 app_  

若習慣 Calendly，不妨換 Cal.com 玩玩看  

---

### 別找了，懶人包在此  
* ~~無知愚民~~一般大眾、想要完整功能者 → [Proton](https://proton.me/calendar) / [Tuta Calendar](https://tuta.com/calendar)  
    不排斥付費的話，可訂閱享完整功能  
* 免費仔、想要離線 app → [Etar](https://github.com/Etar-Group/Etar-Calendar) / [Fossify Calendar](https://www.fossify.org/apps/)  
* 想要 Email、日曆一個 app 搞定 → [Thunderbird](https://www.thunderbird.net/en-US/calendar/)  
* 喜歡客製化的開發者 → [Nextcloud Calendar](https://apps.nextcloud.com/apps/calendar) (可配 [DAVx<sup>5</sup>](https://www.davx5.com/) 再串接至 [Etar](https://github.com/Etar-Group/Etar-Calendar) / [Fossify Calendar](https://www.fossify.org/apps/))  
* ~~墮落者~~想要類似 Calendly 服務者 → [Cal.com](https://cal.com/)  

---

至於社群有些討論的 [OurCal](https://ourcal.com/)，為何沒提呢？  
開源、端對端加密，又主打隱私，似乎挺不錯？  
因為：  
* OurCal 免費試用 14 天，之後就要錢  
    I.e. 無永久免費版，不符合廣義 FOSS  
* 蒐集較多 metadata，如聯絡人、用量、個人識別資訊等  
_# 僅日曆本身隱私，何況公司在[隱私災難地](https://www.amnesty.org/en/latest/news/2025/02/https-www-amnesty-org-en-latest-news-2025-02-uk-encryption-order-threatens-global-privacy-rights/)英國_  

光第一點就出局，所以不推薦  


