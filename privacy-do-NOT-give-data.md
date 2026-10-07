# 不該拿的個資，就不要拿也不要給  

> 履歷幫我填一下，完整填寫才會進入正式面試喔！  

如果面試歐美外商，這段話會很令人困惑  
但如果是台商、尤其傳產，就會再熟悉不過  
要求照片、身分證號、性別年齡、甚至父母的資料，儼然身家調查  
問題是，面試又還沒錄取，要求那些東西做什麼？  
看長相決定是否錄取？還是靠性別、年齡篩選？  
再說就算錄取了，家人個資也不該拿  
**不必要的個資就不應索取**，因為索取了就可能外洩，而且也不尊重使用者、面試者  

---

### 沒有「不會被駭」的系統  
要知道，任何系統 / 機構 / 人都有可能被駭客攻破  
就算不是駭客，[官方](https://citizenlab.ca/research/privacy-in-the-wechat-ecosystem-full-report/)想偷資料、[不肖員工](https://www.vice.com/en/article/snapchat-employees-abused-data-access-spy-on-users-snaplion/)盜取個資、或[政府監控](https://www.aclu.org/news/national-security/nsa-continues-violate-americans-internet-privacy)都層出不窮  
你覺得什麼人 / 機構可能被駭或資料外洩呢？  
除了常見的[通訊軟體](https://www.cpomagazine.com/cyber-security/data-breach-on-the-largest-japanese-messaging-app-line-leaks-440k-records/)、[非營利機構](https://www.twreporter.org/a/personal-data-leaked-npo-donators)，其他對象也都難逃魔爪，例如：  
* 民營機構  
    * [104 人力銀行 ](https://finance.technews.tw/2026/10/06/104-corporation-hacked/) 
    * [7-11](https://cybernews.com/cybercrime/7-eleven-confirms-april-cyberattack-shinyhunters/)  
    * 還有本系列曾舉的一堆科技公司  
* 政府單位  
    * [FBI](https://www.npr.org/2026/09/30/nx-s1-5985202/fbi-hack-shinyhunters) (是的，情報單位也會被駭)  
    * [五角大廈](https://cybersecuritynews.com/pentagon-data-breach/)，即美國政府 (還好啦，被偷 **200 多萬人**個資而已)  
    * [歐盟理事會](https://cybernews.com/news/european-commission-aws-cloud-breach-stolen-data/)  
* 駭客，e.g. [TeamPCP](https://www.secureinseconds.com/blog/2026-08-27-teampcp-arrest-deanonymization-defense)  
    你沒看錯，駭客不會自動免疫，執法單位也可以反過來用相似手段抓人  
    至於為什麼有些駭客很難抓，就是因為他們有做好匿名化，妥善保護自己  

---

遇到請求時該先想想，哪些個資並非必要，非必要就不要亂給  
例如辦會員要生日、地址、手機號碼等，結果你此生不會再去那家店  
_# 這種情況就不要辦會員_  
許多商家都想要你下載 App，但 App 會在你手機上做什麼呢？  
來看看[全家便利商店](https://reports.exodus-privacy.eu.org/en/reports/grasea.familife/latest/)的 Android App：  
* 有多個第三方追蹤器  
    包括 Google AdMob、Google Analytics、Google Firebase Analytics、Insider  
    _# 第一個是廣告，後面幾個是分析用遙測，但分析也可以助長個人化廣告_  
* 索取過量權限  
    拿 53 個權限，且包含機敏、非必要項目，例如：  
    * 精確位置 (好吧，可以藉口說要推薦最近的全家)  
    * 聯絡人  
        請問便利商店 app 要知道你聯絡人做什麼？  
        這就是為什麼不能亂給別人電話號碼，不然對方把你加進通訊錄、又亂下載 app，你的門號就會被許多陌生人取得  
    * 寫入**外部**檔案  
        代表它可以在你手機裡存東西  
    * 修改設定  
        這樣就算你沒手動給權限，app 也能自己來  
    * ...  

這只是其中一個案例，主流商家的應用程式幾乎都有類似問題  
如果不想一一確認，就不要亂下載 app，因為那形同「提供蒐集個資的管道」  
用瀏覽器裝成 PWA、或者都用瀏覽器造訪網站，至少還安全一點  
_# PWA 指 Progressive Web App，有點像裝在瀏覽器裡、但體驗接近原生的 App_  

---

**不會被偷的資料，只有不存在的資料**  
如果你怕詐團、路邊變態、駭客知道哪些事，就不要把那些東西輕易交出去  
心態請從「他要個資，所以我給」，改成「為什麼要這些、不給會怎樣？」  
預設不要亂給，索取者需自證必要性  
雖然不是完美，但會減少很多破口  


