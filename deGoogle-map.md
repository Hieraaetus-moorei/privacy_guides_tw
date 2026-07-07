# deGoogle - 替換地圖

> 糟糕迷路了，用 Google 地圖查一下地獄怎麼去

說到地圖，許多人直覺就想到 Google map
多數人根本不知道，還有其他選擇

#### 讓我們細說從圖
[deGoogle Map](image link)
圖源：~~地獄歸來者~~我自己
^FOSS^ ^指免費開源軟體^ ^(^^Free^ ^and^ ^Open^ ^Source^ ^Software^^)^
^non-profit^ ^指「不以營利為目的」^

### 該被換的地圖
#### Google Map
若未另行阻擋，Google Map 可定位使用者
官方號稱以之規劃路線、預測抵達時間等功能
也許定位的確有惠於正當功能，但廣告和侵入性個資取得，自然也躲不掉

你以為關閉定位，或未使用 app 就沒事嗎？

法院可[不這麼認為](https://www.washingtonpost.com/technology/2022/11/15/google-privacy-settlement-location-data/)，即便「關閉定位」，Google 仍偷偷追蹤用戶位置
蒐集用戶機敏個資以推送廣告，被美國 40 個州[開罰近 4 億美元](https://www.npr.org/2022/11/14/1136521305/google-settlement-location-tracking-data-privacy)
不僅地圖，多項 Google 服務都會定位使用者，就算從裝置設定擋追蹤也一樣
_# 果粉別笑太早，Android、iPhone 用戶都[沒能倖免](https://apnews.com/article/828aefab64d4411bac257a07c1af0ecb)_

#### Apple Map
就算選蘋果地圖，[資料蒐集](https://www.apple.com/legal/privacy/data/en/apple-maps/)只是比較輕微、可控，不是完全不做
蘋果[自家律師說](https://proton.me/blog/iphone-privacy)，理性蘋果 app 用戶，不該指望其活動對蘋果有隱私性
> no reasonable user would expect that their actions in Apple’s apps would be private from Apple

除了從前的商業模式，蘋果也[靠廣告賺錢](https://www.bloomberg.com/news/newsletters/2022-08-14/apple-aapl-set-to-expand-advertising-bringing-ads-to-maps-tv-and-books-apps-l6tdqqmg)
個人化[廣告](https://asymco.com/2026/03/29/apple-maps-is-getting-ads-its-apples-riskiest-bet-yet/)那麼好賺，別以為當果粉個資就很安全

#### 百度地圖
至於百度，陸企就不用說了，中國企業須配合政府做事
若官方要求資訊，誰敢不配合？
不僅軟體不開源、埋設[漏洞](https://cyberscoop.com/baidu-maps-search-app-data-google/)，也[蒐集](https://thehackernews.com/2020/11/baidus-android-apps-caught-collecting.html)用戶[機敏個資](https://www.zdnet.com/article/baidus-android-apps-caught-collecting-sensitive-user-details/)
[百度搜尋和地圖](https://unit42.paloaltonetworks.com/android-apps-data-leakage/)都入列、和台灣又有直接利害關係，更該換掉

### 隱私替代品
本篇替代品全開源、非營利導向
#### [OpenStreetMap](https://www.openstreetmap.org/#map=8/23.611/120.768)
OpenStreetMap (OSM) 直翻開放街圖，是類似 Google Map 的公開地圖服務
不只是地圖，它也存有各種地理資訊，能讓開發者串接、製作衍生產品
_# 商業使用也行，開放街圖用[開放資料庫授權](https://opendatacommons.org/licenses/odbl/) (ODbL)開源_

---

講古 (~~不爽~~可略)：
OpenStreetMap 簡稱 OSM，由英國人 Steve Coast 在 2004 年發起
當時英國地理圖資數據，由政府稅收支持測繪而來，但沒開放給公眾使用
Coast 覺得地圖資訊應能自由流通，而非受政府、商業寡頭把持
受維基百科的成功啟發，他發起 OSM 專案，讓群眾參與繪製、編輯、使用
初期由貢獻者持 GPS 記錄軌跡、實地勘察，土法煉鋼蒐集地理資料
後來加入航空、衛星影像，和政府公開資訊，計畫蓬勃發展
並成立開放街圖基金會 (OpenStreetMap Foundation, OSMF)維運
OSMF 是[非營利組織](https://welcome.openstreetmap.org/about-osm-community/donate-to-osm/)，你也可以[捐款](https://supporting.openstreetmap.org/donate/)支持

---

開放街圖的資料，也為下文其他產品灌溉
且 OSM 有[台灣頁面](https://osm.tw/)，你我都能加入！
缺點：
* 面對大眾的功能有限
* 只有線上版
* ~~介面有點醜~~ (個人觀感)

日常用途或許不那麼方便，但對研究、開發者來說，無疑是個寶藏
大眾可選用依賴 OSM 開發的 app，會比較人性化一點 (如底下介紹者)


#### [FacilMap](https://facilmap.org/)
FacilMap 是[社群開發者](https://github.com/FacilMap/facilmap?tab=readme-ov-file)基於開放街圖，整合第三方服務、調整使用者介面而成
資料來源仍是 OSM，不過功能更完善，也更能客製化
同樣非營利、接受捐助，能多人同時協作
伺服器可自行架設，也可用[官方服務](https://facilmap.org/)
缺點：
* 只有線上版

#### [Organic Maps](https://organicmaps.app/)
直翻有機地圖，是[群眾協作](https://github.com/organicmaps/organicmaps)的行動版地圖
支援離線使用，起初客群是觀光客、旅行者、登山客、單車騎士等
_# 先預載地圖，到當地離線照樣能用_
可離線導航、自訂圖標、記錄足跡，而且有**暗色、語音模式**喔！
_# 開發者[說法](https://odysee.com/@techlore:3/the-maps-app-that-collects-zero-data:0)是，本地圖「離線優先 (offline first)」，從源頭設計保護隱私_
離線運作原理是：先下載壓縮過的向量指標，再即時依需求展開地圖
即使是舊手機，一樣能流暢使用
唯一需要連網的時間，只有初次下載 app 和地圖
鑑於口碑佳，很快擴散到一般大眾
許多追求隱私、程式效能者，也加入用戶行列
介面簡潔、運作效率高，操作也很直觀
_# 程式主體由 C++ 寫成_
缺點：
* 還沒找到 (歡迎提供)

資料來自開放街圖，但包成好用的手機 app
Android 和 iOS 都可取得，不妨立刻載來試試

#### [OsmAnd](https://osmand.net/)
全名「OSM Automated Navigation Directions」，意指自動導航
客群主要是交通工具使用者，e.g. 駕駛、騎士、登山客、船員等
同樣支援離線使用、語音導航、軌跡記錄、暗色模式等
多數功能和有機地圖相近，同樣基於 OSM (看名字就知道)
OsmAnd 甚至更多用途，恕無法一一列舉，堪稱「完整版萬能地圖」
_# 相較之下，有機地圖主打「簡單」、「易用」_
Android 和 iOS 都可取得
缺點：
* 分免費、付費版
    免費版就很夠用，但既然出了收錢版，免費版功能就會被砍一些
* 功能多的缺點：複雜性較高，可能需摸索適應一下
* 效能較有機地圖低
    _# Java 編寫而成_
離線地圖的好處，就是沒網路的荒山野地仍可用 (戰時斷網亦同)
平常情況下，不連網更省電、也更不怕個資被偷

---

### 懶人包
網頁版用 [OpenStreetMap](https://www.openstreetmap.org/#map=8/23.611/120.768) / [FacilMap](https://facilmap.org/)，你高興就好
至於手機 app：
一般用戶 / 極簡主義者 → [Organic Maps](https://organicmaps.app/) (有機地圖)
專業用戶 (例如越野車玩家) → [OsmAnd](https://osmand.net/)

---

這次比較簡短，因為地圖好選擇不多
不過這幾個替代品，就很夠用


