# deGoogle - 雲端硬碟與相簿

> 檔案太大了，用 Google drive 連結分享給我

個資，也順便分享給 Google 了
不僅 [Google](https://www.techradar.com/pro/security/gemini-ai-platform-caught-scanning-google-drive-files-without-user-permission)、[Dropbox](https://proton.me/blog/dropbox-security-issues)、[百度](https://gbhackers.com/chinas-baidu-compromised-in-data-leak/)...，主流中美企業個資爭議不斷
畢竟從架構到商業模式，都不是為隱私設計
免費方案看似慷慨，其實是個人資料換來的
賺到服務，卻賣了自己

鑑於性質相似，本篇將一併介紹雲端相簿、檔案分享服務
如果還在用預設相簿且開啟備份，勸你三思

### 來人，上圖！
[deGoogle drive and album](image link)
雲端硬碟替代方案
^製圖：我^
^FOSS^ ^指^ ^Free^ ^and^ ^Open^ ^Source^ ^Software^^，即免費開源軟體^
^端對端加密^ ^(^^End-to-end^ ^encryption^^)^^，僅你、獲授權者才能看到內容，公司也不知你傳了什麼^
* Google 雲端硬碟 / 相簿
    不只對外[安全性問題](https://www.technice.com.tw/techmanage/infosecurity/187175/)，Google 更能[掃描](https://proton.me/blog/is-google-drive-secure)你的雲端硬碟內容
    Android 手機預設的 Google 相簿，也有[照片被拿去練 AI](https://proton.me/blog/is-google-photos-safe#ai-training)、烏龍[指控兒少性犯罪](https://www.nytimes.com/2022/08/21/technology/google-surveillance-toddler-photo.html?unlocked_article_code=1.80w.nigh.XohWLd4Vrdgd)及其他隱私疑慮
* Dropbox 
    隱私政策[疑點重重](https://proton.me/blog/dropbox-privacy)，不只聲明「受法律要求時，他們會基於自身判斷是否提供資料」 (別忘了，[PRISM](https://techcrunch.com/2014/10/11/edward-snowden-new-yorker-festival/) 計劃是美國國安局主導，他們會說不嗎？)
    還和不少機構分享資料，又閉源、非端對端加密
    而且過往實在[不怎麼光彩](https://www.theguardian.com/technology/2014/apr/11/dropbox-condoleezza-rice-privacy-surveillance)，自然在更換名單內
* OneDrive / SharePoint
OneDrive 從[設計](https://www.infosecurity-magazine.com/news/microsoft-onedrive-flaw-exposes/)上就[不安全](https://www.proofpoint.com/us/blog/cloud-security/proofpoint-discovers-potentially-dangerous-microsoft-office-365-functionality)，且微軟也保留檔案存取權
SharePoint 可分享、協作、儲存檔案，還有多種管理、自動化工具
可架設企業內網、充當整合工具平台
然而，SharePoint 和 OnDrive 同樣有安全性問題
今年才[被駭客利用](https://www.forbes.com/sites/siladityaray/2025/07/21/hackers-exploit-microsoft-software-vulnerability-to-reportedly-target-governments-and-businesses-what-to-know/)，造成[核子機構](https://socradar.io/toolshell-sharepoint-zero-day-cve-2025-53770/)、[研究單位](https://www.washingtonpost.com/technology/2025/07/23/sharepoint-microsoft-hack-nih-nnsa/)等[諸多受害者](https://www.securityweek.com/toolshell-attacks-hit-400-sharepoint-servers-us-government-victims-named/)淪陷
微軟出了不少修補，但也建議使用者改用他家線上平台，變相廣告
_# 就不安全了，還付錢用你雲端？_
* 其餘市占率較低的危險雲端，如[百度網盤](https://tw.stock.yahoo.com/news/%E5%9C%8B%E5%AE%89%E5%B1%80-%E5%B0%8F%E7%B4%85%E6%9B%B8-%E5%BE%AE%E5%8D%9A-%E6%8A%96%E9%9F%B3-%E5%BE%AE%E4%BF%A1-030600240.html)、[Yandex Disk](https://www.cloudwards.net/review/yandex-disk/) 等恕不一一詳述

開始換吧！

#### [Proton Drive](https://proton.me/drive)
在 [Email 那篇](https://vocus.cc/article/6895c735fd89780001176a4a)提過，Proton 是保障隱私的瑞士公司，[台裔科學家](https://proton.me/blog/author/andy-yen)創立
他們率先提供「端對端加密」、「開源」、保障隱私的雲端儲存服務
因為端對端加密，只有你、你授權的人能存取
**Proton 也看不到你的檔案內容**，所以請牢記密碼、備份金鑰
_# 否則一旦忘記密碼，沒人能幫你救回檔案_
雲端硬碟和自家文件、郵件整合，類似 Google 雲端的概念
無廣告、不出售個資，採訂閱制 (且為防特定政權封鎖，接受虛擬貨幣付款)
缺點：
* 手機版 app 偶爾會出狀況
* 免費版容量小，不過訂閱能享有整個 Proton 生態系的服務
    月費數百台幣，可等黑色星期五、特定節日再下大單，多半有驚天折扣 (e.g. 三折)
* 若想當相簿用，介面可能不太方便 (畢竟產品定位是雲端硬碟)

#### [Filen](https://filen.io/)
Filen 是德國公司，提供端對端加密的雲端空間，程式碼開源、支援各大平台
曾有加密[安全性不足](https://github.com/privacyguides/privacyguides.org/pull/345)問題，例如使用 RSA 演算法
儘管未公開回應，但更新的程式碼已[改善](https://filen.io/hub/)此類問題
訂閱制，免費帳戶給 10GB 儲存空間
不定期推出終身方案，可一次買足
_# 注意：若公司倒閉，終身方案仍形同白搭_

缺點：
* 免費帳戶三個月沒用，資料就會被刪除
    付費帳戶三年沒用，才會被刪資料
    _# 付錢又不使用，對商家不是很划算嗎？為何要停權？_
* 定位是雲端硬碟，不太適合當相簿
* 曾出過檔案傳輸中斷等 bug，雖已修復但使用上需小心

#### [Nextcloud](https://nextcloud.com/)
Nextcloud 也是德國公司，產品 100% 開源，主張去中心化整合雲端
產品很像 Google 雲端，各種工具整合在一個服務中
人人皆可自行架設，且企業版和一般版「**沒有差別**」
主要靠提供企業、政府解決方案來獲利，例如資安認證、客服、穩定版本維護
簡單說就是賣服務，所以散戶不必擔心隱藏費用
你可以自行架設雲端，和家人朋友共用
_# 自行架設相對隱私，因為只有你可以偷自己的個資_
支援端對端加密，雖然自有雲端不見得需要
純粹儲存、分享檔案外，亦享有整合工具服務
官方也有合作者事先架好服務，付費即可直接使用
_# 但你得信任服務架設者_
缺點：
* 有技術門檻
* 需自行維運相關設備

#### [Syncthing](https://syncthing.net/)
此為檔案傳輸軟體，非雲端硬碟
使用對等網路 (peer-to-peer, p2p)，意思是不經中央伺服器
由你和檔案接收者，直接對傳檔案
所以儘管只靠 TLS 加密，仍達成**端對端加密**

---

白話文解釋：
你想分享檔案給朋友，於是你們下載 [Syncthing](https://syncthing.net/downloads/)、保持在線
接著你上傳檔案、他接收檔案，結束
只有你本人、該朋友可取得檔案，沒第三人
有點像搭建一個直通滑道，然後把包裹滑至對方家
沒有物流公司、撿貨員，參與者只有你們倆

---

Syncthing 開源、免費、去中心化，支援各大桌面平台
Android 有[非官方 app](https://github.com/Catfriend1/syncthing-android)，但也開源
缺點：
* 傳輸時須保持在線
* 檔案在收發裝置上沒加密，若駭客入侵有機會取得明文
    _# 簡單說：若你或朋友的電腦中毒，就可能不安全_
* iOS 尚不支援

#### [OnionShare](https://onionshare.org/)
同樣是檔案傳輸用，很像 Syncthing
OnionShare 直翻「洋蔥共享」，用洋蔥路由傳輸資料

---

洋蔥路由 (The Onion Router, Tor)
洋蔥路由連線皆經多層加密 (通常是三層)，無單一伺服器可解析使用者活動
伺服器群靠志願者、機構架設，分佈於全球各地，不受特定政府管轄
Tor 專案由非營利組織維運，不必擔心隱藏費用

---

開源、端對端加密，支援所有主流平台
Linux、Windows、MacOS、Android、iOS 都能用
_# 行動版由守望者計劃 ([Guardian project](https://guardianproject.info/))開發_
除了檔案分享，OnionShare 還提供「架設暗網網站」、「聊天」功能
沒什麼技術門檻，下載軟體、按指示做即可
_# 若真不會用，也可參考[教學影片](https://odysee.com/@techlore:3/onionshare-for-private-file-sharing,:7)_
缺點：
* 速度較慢，畢竟要多層加密
* 傳輸檔案時，須保持在線上

#### [Immich](https://immich.app/)
Immich 為 Google 相簿替代品，開源、可自架伺服器
由社群自主開發，非盈利項目
可處理照片、影片，介面人性化
因伺服器自行架設，就沒端對端加密
缺點：
* 需自備硬體，稍有技術門檻

#### [Cryptomator](https://cryptomator.org/)
德國公司 [Skymatic](https://skymatic.de/) 開發、維護，是開源、免費軟體
Cryptomator 本身非雲端、相簿、或檔案共享軟體
而是相容於各大雲端的**客戶端加密**軟體，可搭配 Dropbox、Google drive、OneDrive...
功能：把檔案先加密，再傳上任一雲端硬碟
如此一來，雲端供應商只會看到亂碼，不知檔案內容
程式和各雲端無縫整合，[操作非常簡單](https://techlore.tv/w/9KQBtSMJNNwXCaSxRZwT5f?start=1s)
**幾乎等同使用你習慣的雲端，只是把它變安全了**
有此軟體，任何雲端都能當加密雲端
缺點：
* 比純用特定雲端慢，因為檔案收發須加解密
    不過相較其他端對端加密服務，就無明顯速度差
用 [VeraCrypt](https://veracrypt.io/en/Home.html) 手動加密每個檔案也行，但 Cryptomator 和雲端整合，方便許多
_# VeraCrypt 是硬碟加密軟體，日後**可能**會提_

#### [Ente Photo](https://ente.io/)
簡稱 Ente，是 Google Photos 替代品

---

講古：
從前從前，有個[印度人](https://ente.io/blog/ama-with-ente-ceo/)在瑞士 Google 工作
他發現主流相片軟體不保障隱私，卻沒平易近人的替代選項
於是返回印度後，他開發了相片管理軟體
也成立公司，提供雲端服務
公司註冊在美國上市，但主要研發總部在阿姆斯特丹 (荷蘭)、邦加羅爾 (印度)
資料存於[歐盟](https://ente.io/help/photos/faq/security-and-privacy#data-encryption-and-storage) (德國法蘭克福、法國巴黎、荷蘭阿姆斯特丹)，受歐盟隱私法規庇護
「Ente」源於馬拉雅拉姆語 (Malayalam, 創辦人母語)，意為「我的」
所以產品指「[我的相片](https://ente.io/help/#origin-of-the-name)」

---

Ente 軟體**全**[開源](https://github.com/ente-io)，支援所有主流平台
資料端對端加密，metadata (相片的資料)也加密
app [功能](https://ente.io/features/)非常多，體驗甚至好過 Google 相簿
_# 可鎖 app、隱藏相簿、無廣告、本地運作的 AI 功能..._
採訂閱制，免費帳戶 10GB 雲端備份空間，自架空間則視你硬體而定
也可以不用雲端備份，純粹當本地相簿軟體
那容量就視你裝置而定，且可離線使用
缺點：
* 公司登記在美國
* 過去曾有下載慢、功能少的問題，但很快就解決
    _# 開發團隊效率高，或許算種優點？_

#### [Mega](https://mega.io/)
紐西蘭公司，母公司登記在香港
_# 別急！創辦人[說過](https://www.businessinsider.com/kim-dotcom-data-not-safe-filing-sharing-site-mega-2015-7)，中資、美資併購 Mega 的事，都是[假訊息](https://www.zdnet.com/article/mega-denies-claims-by-kim-dotcom-of-nz-government-control-of-company/)_
端對端加密，且提供線上會議功能
客戶端程式碼公開，但非開源
I.e. 可檢視程式碼，但不授權各種使用
_# 即使是廣義開源，仍非程式碼公開就算，可參考[本篇](./open-source-intro.md)_
最大的優點是，免費帳戶就有 20GB
_# [據說](https://www.zdnet.com/article/review-what-to-expect-from-megas-free-50gb-of-cloud-storage/)從前免費帳戶有 50GB，但 20GB 也算慷慨了_
缺點：
* 中資疑慮 (畢竟香港被強硬接管了)
    至少只有母公司在香港，且客戶端加密、公開程式碼 (否則不會入列)

---

### 其他
#### [Firefox Send](https://github.com/mozilla/send)
熟悉開源的人可能好奇，為何沒提 Firefox Send？
Firefox Send 是 Mozilla 的開源專案，為端對端加密檔案傳輸軟體
用戶上傳檔案到伺服器、分享連結給別人以供下載
且可設定下載多少次、或某個期限後，自動焚毀檔案
更棒的是，伺服器可自架！

如此美妙，為何不提？

因為 2020 年官方已[停止維護](https://support.mozilla.org/en-US/kb/what-happened-firefox-send)，僅剩社群支援
且[社群服務點](https://github.com/timvisee/send-instances/)需信任第三方，存在安全風險
_#  若不介意仍可使用，**出事不負責**_
好消息是，Mozilla 說 Thundermail 會復刻、改良 Firefox Send
讓我們拭目以待

### 果粉可能會問，那 iCloud 呢？
尚可接受，因其有[端對端加密](https://support.apple.com/en-us/102651)
但除此之外，就沒什麼可提
缺點：
* 閉源，程式碼不公開
    所以無從檢核是否落實加密、偷埋後門
* 美國公司，又曾參與稜鏡 (PRISM)[監聽計劃](https://www.theguardian.com/world/2013/jun/06/us-tech-giants-nsa-data)
    _# 何況不開源，如何相信他們呢？_
* 綁蘋果生態系、免費儲存空間少
* 需開啟[進階資料保護](https://support.apple.com/en-us/102651#advanced) (ADP)，預設[標準保護](https://support.apple.com/en-us/102651#standard)沒端對端加密
    _# 蘋果稱其為「標準」，可見不認為用戶需要太多隱私_
* 蘋果曾在[英國政府要求](https://www.theregister.com/2025/02/24/apple_adp_replacements_e2ee/)下，取消端對端加密

光前兩點，就不推薦 iCloud 了
但相較其他美企，又稍微好一點
於是沒在欠換名單內

#### pCloud
說來話長，簡言之不推薦
pCloud 外宣自己是[瑞士公司](https://www.pcloud.com/company/about.html)、有跨平台服務、[客戶端加密](https://www.pcloud.com/Europe)
且最獨特的行銷，就是「終身方案」
I.e. 付一次錢，享有終身儲存空間

聽起來不賴，為何不推薦呢？

因為：
* 公司[不透明](https://www.experte.com/cloud-storage/pcloud)，許多資訊無從得知
* 閉源，程式碼未公開
* 營運團隊主要在[保加利亞](https://www.reddit.com/r/pcloud/comments/11kbyjd/some_concerns/)，資料儲存在盧森堡、**美國**
    主打「瑞士公司」有誤導之虞，保加利亞和瑞士法規差異甚大
    資料存在美國，更要擔心**美國政府**，莫忘 [NSA 稜鏡計劃](https://epic.org/documents/epic-v-doj-prism/)
    _# 善意提醒，保加利亞親俄_
* 免費帳戶有置入廣告，想當然爾追蹤器們...
    _# 而且只有 5GB，還不如選 Proton Drive_
* 加密功能須另購，不是訂閱、購買就享有
* **帳戶停權爭議**：
[許多](https://www.reddit.com/r/DataHoarder/comments/n9shfp/pcloud_subscribers_accounts_terminated_with_no/)用戶[反映](https://www.reddit.com/r/pcloud/comments/rhbw4p/lost_720_to_pcloud_black_friday_deal_account_just/)，買了終身方案且添購加密服務
    * 有人被無預警停權，沒任何通知
        且保證退費期內解約，仍未退費
    * 有人被警告，上傳內容侵害版權，因而停權
        首先，客戶端加密，他們何以得知侵權？打自己臉？
        _# 要碼 pCloud 羅織罪名，要碼加密是假的、有後門_
其次，有人上傳「公領域文件 (沒版權)」、「合法購買內容」，卻仍遭停權
意見反映無效，其他檔案也被刪
    _# 顯然編造藉口，只是想停你權_

    從前有人好奇，「終身方案」如何永續經營？
    畢竟那像老鼠會，若無新人加入，遲早會垮
    現在知道了，他們收錢、停權，近乎當強盜
    所以提供終身制，仍可持續獲利，畢竟拿錢不做事

劣跡斑斑的公司，自然不值得推薦
你當然能碰運氣，說不定停權沒停到你
但爭議多、誤導行銷、閉源...，至少我不信任 pCloud

---

#### 懶人包
* 雲端先來：
    * 願意付費、喜歡整合服務 → [Proton Drive](https://proton.me/drive)
    * 開發者想自架 → [Nextcloud](https://nextcloud.com/)
    * 免費仔、有習慣雲端者 → [Cryptomator](https://cryptomator.org/) + 你原本的雲端
        或選 [Filen](https://filen.io/) / [Proton Drive](https://proton.me/drive)
    * 蕭貪免費仔 (？) → [Mega](https://mega.io/)
* 檔案分享：
    * 高風險人士 → 不用想，就是 [OnionShare](https://onionshare.org/)
    * 一般人 → [Syncthing](https://syncthing.net/)
        甘冒風險者，[Firefox Send](https://github.com/mozilla/send) 也行
* 相片軟體：
    * 開發者想自架 → [Immich](https://immich.app/)
    * 想簡單換 Google 相簿、免費仔、願意訂閱者 → [Ente Photo](https://ente.io/)

---

不想被大企業偷窺，早點替換才是王道

