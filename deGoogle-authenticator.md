# deGoogle - 兩步驟驗證器  

> 兩步驟驗證好煩，密碼打對了還要被擋  

好奇為什麼設計此擾人機制嗎？  

### 兩步驟驗證  
#### 那是什麼鬼？  
兩步驟驗證 (2-step ~~[from the hell](https://www.youtube.com/channel/UC3swwxiALG5c0Tvom83tPGg)~~ verification) = 雙因素驗證 (2-factor authentication)  
指「需要過兩關才能登入」，通常是密碼和簡訊 / app / 認證信等  
雖然有點麻煩，但其為安全而生  
設想以下情境：  
電郵地址通常是公開資訊，被人知道不奇怪  
而你貪圖方便，用懶人密碼`P@ssw0rd`  
某天駭客對郵件服務施展「密碼噴灑 (password spray)」，企圖竊取使用者身份  
「密碼噴灑」指嘗試用同一組密碼，對多個帳號進行登入  
通常密碼是外流、或常用的懶人款  
如果大眾都設懶人密碼，一次噴灑能獲得的帳號就很可觀  
重點是只嘗試一次，所以「三次失敗就鎖帳」機制擋不住  
於是，駭客輕鬆取得你的郵件，改個密碼你就無法登入了  

兩步驟驗證，能幫上什麼忙呢？  

假設你有開啟 2FA，駭客就會被擋在第二道門外  
當他用**正確帳密**登入，系統便跳出「請輸入 app 上顯示的 6 位數字」  
結果綁定的 app 在你手機裡，他什麼事也做不了  
_# 除非你手機被偷_  
好的服務還會寄信通知你，有人嘗試登入帳戶  
你可以改密碼、檢查問題、變換登入方式...  
兩步驟驗證，對資安有莫大助益  

---  

資安人士的苦衷：  
沒出事大眾總嫌麻煩，出事又怪系統不安全  
幫幫忙好嗎？  
疫苗不打、口罩不帶、衛生不顧，危險的事 (e.g. 重複、懶人密碼)一直做  
被感染又怪衛生單位沒做事，到底誰的問題？  

---  

兩步驟驗證常見做法，有簡訊認證碼、email 驗證信  
還有本次主角 - 應用程式一次性密碼 (One-Time Password, OTP)  
OTP 又分基於時間 (Time-based OTP, TOTP)、或雜湊函數 (Hash-based OTP, HOTP)  
#### TOTP  
原理：  
雙方先綁定時間戳記、約定密鑰，之後就可以離線  
每次登入時，系統基於當下時間 + 演算法，變換鎖孔形狀 (改變認證碼)  
神奇的是，鑰匙也會同步更新形狀，因為時間戳記和密鑰早就綁定了  
_# 有點像「雙方約好調整鎖鑰」，且每秒用固定方式共同變換_  
除了當初綁定者，其他人無法得知鎖鑰狀態  
尤其認證碼多半「每 30 秒」、「每分鐘」自動更換，非法入侵難度高  

#### HOTP  
嗯，得先解釋雜湊 (Hash)  

---  

雜湊簡單解釋 (其實不太簡單)：  
雜湊函數 (Hash function)是一類演算法，可將各種輸入轉成「固定長度」的輸出  
輸出稱為雜湊值 (hash value / hash)、摘要 (digest)、或雜湊碼 (hash code)  
因安全性高，常用於密碼轉換、儲存  
雜湊具以下特性：  
* 不論輸入多長，輸出長度都一樣  
    每個人密碼長度不同，但都用同樣 Hash 長度儲存  
    I.e. 無法從雜湊長度推測密碼位數，保護長度資訊  
* 快速計算  
    任何輸入都能高效產生雜湊值，避免運算時間暴露輸入性質  
    I.e. 密碼多長、多複雜，運算時間都差不多，保護密碼長度、複雜性  
* 抗碰撞性 (Collision resistance)  
    「兩種輸入產生同樣輸出」非常困難，通常以「機率極低」當標準  
    和安全性較無關，只是避免撞號  
    _# 此處「碰撞」可理解成「撞衫」，不同人碰巧用到一樣的值_  
* 抗篡改 / 微調 (又稱雪崩效應，Avalanche effect)  
    輸入稍改，輸出就會巨幅改變，如雪崩一般  
    I.e. 無法每次微調一點，觀察輸出變化來破解  
* 抗預像性 (Preimage resistance)  
    難以用雜湊值回推密碼，運算過程不可逆  
    I.e. 駭客取得雜湊值，也推不出你的密碼  

雖然身為函數，像是 h(x) = y  
不過雜湊函數很複雜，不是隨便手算可破解的  
_# 如果你手算破解了主流 Hash 演算法，請聯繫[阿貝爾獎](https://abelprize.no/) (Abel prize)_  
只要使用高強度密碼，暴力破解就會[曠日費時](https://specopssoft.com/blog/sha256-hashing-password-cracking/)  
_# 如 12 位數大小寫字母 + 數字 + 特殊符號，用 RTX 4090 得花近 20 **萬**年破解_  
鑑於高度安全性，Hash 幾乎被所有需要密碼的服務採用  
機構只儲存 Hash value，密碼留在用戶手上  

---  

HOTP 以雜湊為基礎，用「遞增計數」變換驗證碼  
雙方先約定密鑰，並共享計數器  
每次使用計數器就 + 1，演算後鎖孔、鑰匙跟著協變  
意思是，每次開鎖都會改變鎖鑰，適合用在手動觸發的情況  
_# 例如 API 驗證，開發者可能比較有感_  

<br/>  

知道那些要幹嘛？  

<br/>  

手機應用程式，能用來綁定 TOTP、HOTP  
多半本地儲存，資料不離手機  
有些會提供雲端備份，但加密與否各家殊異  
常見選擇有 Google、微軟 Authenticator，或 Twilio Authy  
知道我要說什麼了吧？  
沒錯，換掉那些東西！  

### 圖來囉！  
[deGoogle authenticator](image link)  
<sup>FOSS 指免費開源軟體 (Free and Open Source Software)</sup>  
<sup>non-profit 指就該品相而言，「不以營利為目的」</sup>  
<sup>e2ee syncing 指「提供端對端加密備份方式」</sup>  

### 欠換名單  
#### Google Authenticator  
不意外，先從 Google 開刀  
Google 驗證器從前無備份機制，所以手機壞掉、弄丟，就完蛋了  
_# 綁定的服務都會無法登入_  
2023 年[推出](https://security.googleblog.com/2023/04/google-authenticator-now-supports.html)雲端備份，登入 Google 就能同步各裝置、備份密鑰  
然而同年有研究員[指出](https://www.scworld.com/news/google-authenticators-syncing-security-concerns)，Google 備份**未**端對端加密  
換句話說，官方**能看到你的密鑰**  
Google 收到輿論壓力後[表示](https://www.malwarebytes.com/blog/news/2023/05/google-will-eventually-add-end-to-end-encryption-to-google-authenticator)，端對端加密在計劃中，準備好就會加上  

猜猜怎麼著？  
他們加了嗎？  

沒有！  
2023-2025，至截稿前都沒端對端加密  
這技術很難？  
才怪！有公版能照著走、也已有開源實作能參考，最好兩年做不出來  
Google 身為全球頂尖軟體公司，遲遲沒下文只有一個可能 - 
**不想做**，說不定還賭用戶們忘記此事了  
風頭一過就裝傻充愣，資料到手再說  
而且想用雲端備份，就得辦 Google 帳戶  
別忘記在 Google 生態系中，就算你選擇「關閉追蹤」，個資照樣被偷  
_# 今年 (2025)美國、法國才都[罰過](https://www.computerworld.com/article/4051435/google-hit-with-806m-in-penalties-from-us-and-french-authorities-over-privacy-issues.html)，熱騰騰的**八億美金**呢！_  
驗證器[隱私政策](https://sites.google.com/view/authenticator-privacy-policy/)又說明，蒐集超多個資、Metadata：  
* IP  
* Email  
* 地區  
* SIM 卡綁定的地區  
* 每次使用的時間  
* **廣告識別資料**  

除了優化服務，也明言會用於**個人化廣告**喔！  

如此危險，能不換嗎？  

#### Microsoft Authenticator  
微軟也不遑多讓，官方[明講](https://support.microsoft.com/en-us/account-billing/microsoft-authenticator-faqs-12d283d1-bcef-4875-9ae5-ac360e2945dd#:~:text=Authenticator%20collects%20your%20GPS%20information,to%20access%20the%20protected%20resource.)會蒐集：  
* GPS 地理位置  
* 微軟帳號資訊 (若你要備份)  
    _# 雲端備份**無**端對端加密 ([微軟能打開](https://techcommunity.microsoft.com/blog/microsoft-entra-blog/how-it-works-backup-and-restore-for-microsoft-authenticator/1006678)、看到內容)_  
* 生物辨識資訊 (如果用臉、指紋登入)  

個資除了優化服務，同樣也[用於](https://www.microsoft.com/en-us/privacy/privacystatement)推薦產品、**個人化廣告**  
更噁心的是微軟拿手絕活 - 綑綁行銷  
許多微軟服務如 Azure，[要求](https://learn.microsoft.com/en-us/answers/questions/5253276/i-am-being-forced-to-install-the-ms-authenticator)用戶使用微軟驗證器  
或許能用他牌軟體，但預設指引是微軟 (有多少人會去查呢？)  
很遺憾，不少深陷微軟體系的[公司](https://discuss.privacyguides.net/t/work-is-requiring-me-to-install-miscrosoft-authenticator/14769)，會[規定](https://www.reddit.com/r/privacy/comments/17vvaey/work_is_requiring_me_to_install_microsoft/)員工得用那些東西  
理論上因工所需，公司應提供「工作機」給你裝個資盜竊軟體  
個人手機應保持乾淨、安全，所以碰到這類情況請堅守立場  
要馬拒絕安裝，要馬索取工作機  
外國論壇都是一片倒，公司得提供手機或給予補償  
這才是正當應對，千萬別奴到交出權益！  

#### Twilio Authy  
Twilio 是美國公司，2015 年收購 Authy (兩步驟驗證軟體)  
雲端備份**有**端對端加密，且免費使用  
_# 每月有免費額度，超過要按次計費_  

聽起來不錯，為什麼要換呢？  

首先，非全免費、不開源  
再者，**安全性不足**  
而且，個資會用於[廣告推送](https://www.twilio.com/en-us/legal/privacy)  
不開源、廣告問題顯而易見  
安全性不足，則可從過往歷史推知：  

---  

2022 年被駭客攻擊，[部分帳號被竊取](https://www.twcert.org.tw/tw/cp-104-6471-26455-1.html)  
2024 年又被攻擊，用戶[個資外流](https://thehackernews.com/2024/07/twilios-authy-app-breach-exposes.html)，包括[三千三百萬人的門號](https://www.securityweek.com/twilio-confirms-data-breach-after-hackers-leak-33m-authy-user-phone-numbers/)  

---  

非開源的壞處，就是公正第三方無從審核  
宣稱安全、自詡隱私，只要沒被審查都能吹牛  
漏洞也無法預先察覺，被駭客滲透了才知道  
這也正好印證，資安、隱私的準則 - 不該拿的資料就別拿  
若未蒐集手機號碼、Email 等個資，就不會被偷  

#### Ravio OTP  
有在關注開源的人，應該會驚呼：「等等，那不是開源 iOS OTP 軟體嗎！？」  
抱歉，**不再**是了  
2023 年，法國公司 Mobime 買下開源專案 Ravio OTP  
調整[授權規範](https://github.com/raivo-otp/ios-application/blob/master/LICENSE.md)，僅「公開程式碼」而不「開源」  
且一次更新[刪光用戶資料](https://www.reddit.com/r/privacy/comments/1dcr5zn/raivo_otp_is_now_deleting_data_and_asking_for/)，付費才能取回 (根本勒索軟體)  
之後備份、匯出都要[訂閱](https://www.reddit.com/r/privacy/comments/1d3ha4f/raivootp_do_not_update/)，已完全商業化  
_# [社群解方](https://discuss.techlore.tech/t/i-lost-my-raivo-otp-passwords/8755)是先備份資料、再更新軟體；終極做法當然是**換掉**！_  
夠爛了嗎？  
還沒完，最惡劣的是**誤導行銷**  
上述內容可知，Ravio OTP 早已商業化、非開源  
但[官網](https://raivo-otp.com/)迄今仍自稱「非商業」、「開源」  
![Ravio OTP self-claimed non-commercial](ravio-commercial-scam.png)  
![Ravio OTP self-claimed as an OSS](ravio-open-scam.png)  
程式碼倉庫[宣稱](https://github.com/raivo-otp/ios-application?tab=readme-ov-file)不蒐集個資，但 Mobime [隱私政策](https://mobime.org/privacy/)說使用 Facebook、Google AdMod  
_# 個人化廣告追蹤器，會蒐集 IP 等資訊_  
問題頗大，不換不行  

---  

### 替代品們  
#### [2FAS](https://2fas.com/auth/)  
創立者為[美國人](https://www.linkedin.com/in/marcbpunk/)，不過比較像社群專案  
主要貢獻者是[波蘭人](https://github.com/GrzegorzZajac000)，其餘成員[來自各地](https://2fas.com/about-us/)  
免費、開源、資料存於地端 (e.g. 你手機)，無雲端伺服器  
_# 沒伺服器就不會拿資料_  
提供端對端加密備份，備份雲端依裝置而定  
iPhone 預設用 iCloud，Android 則是 Google Drive  
因為有加密，Google 和蘋果看不到內容 (當然，你也可以不備份)  
可設定生物辨識解鎖，增加方便性  
使用毋需帳號，不必信任特定機構  
匯入 / 匯出功能完善，可無痛從 Google 或 Twilio Authy 轉來、轉走  
還有出瀏覽器外掛，和手機 app 同步就不必手打驗證碼  
商業模式來自贊助，認同理念的話不妨打賞  

缺點：  
* 新版非立刻開源  
    官方[授權](https://raw.githubusercontent.com/twofas/2fas-pass-android/main/LICENSE-FAQ.md)寫明，推出後是「原始碼公開」，商用須申請  
    每版兩年後，才[自動流用](https://raw.githubusercontent.com/twofas/2fas-pass-android/main/LICENSE) GPL 3.0 (開源)  

支援 TOTP、HOTP，想要的功能基本上都有  

#### [FreeOTP](https://freeotp.github.io/)  
顧名思義，免費的 OTP 驗證軟體  
_# HOTP 和 TOTP 都支援_  
[Android](https://f-droid.org/packages/org.fedorahosted.freeotp/) 和 [iOS](https://apps.apple.com/us/app/freeotp-authenticator/id872559395) 皆可取得，完全離線使用  
由紅帽 ([Red Hat](https://www.redhat.com/)) 公司贊助開發，會長期、穩定維護  
_# 你沒看錯，此紅帽即 Red Hat Linux 那家公司_  
身為開源產品推動者，紅帽[不想走上](https://www.redhat.com/en/blog/identity-management-and-two-factor-authentication-using-one-time-passwords) Google 閉源道路  
於是贊助 FreeOTP 開發，旨在提供「免費」、「開源」、「跨平台」的選擇  
不蒐集任何個資、不需帳號，也不會連線到伺服器  
支援多數主流服務，可透過 QR code 或手動將 token 加入  
_# 白話文：可以掃碼或打字串綁定 2FA_  
雖然紅帽是營利企業，但此專案屬非營利性質  

缺點：  
* 紅帽為美國公司，近期有重大爭議  
Linux 是開源專案，但 Red Hat [限制](https://arstechnica.com/information-technology/2023/06/red-hats-new-source-code-policy-and-the-intense-pushback-explained/)大眾查看紅帽 Linux (RHEL)原始碼  
此舉有悖開源初衷，下游開源版 CentOS 甚至[被終止](https://www.redhat.com/en/topics/linux/centos-linux-eol)  
GPL 授權僅規範「取得二進制檔案者須可檢視原始碼」，非所有人  
紅帽的做法是：訂閱戶可看原始碼，但「重新分發」就會終止合約  
意思是，付錢才能看程式碼，一旦你要重製 (開源核心價值)就終止授權  
若終止你還分發，則屬違法侵權  
_# 很會鑽漏洞吧？法務堪比甲骨文公司_  
這種做法違反開源精神，因此招來社群反彈  
誰知道哪天，Red Hat 會不會對 FreeOTP 如法炮製呢？  
* 介面有點「復古」，至於美醜因人而異  
* 社群回報備份功能異常，似乎尚未修復  
    如果你沒備份需求，就不影響  

#### [Authman](https://authman.simular.co/)  
台灣公司夏木樂 (Simular)所開發，隸屬百岳國際集團  
開源、免費、跨平台的 OTP 軟體，可用於 TOTP 驗證  
_# Android、iOS、Window 和 Mac 都能用_  
可自選備份雲端，或用官方伺服器  
備份前資訊會先加密，伺服器看不到明碼  
_# I.e. 端對端加密_  
高度可客製化，字體、縮圖都能改  
同樣能輕鬆匯入 / 匯出 token，不綁死生態系  
官方說：  
> Authman is open, just export tokens for any purpose you want  

算有良心吧？  
也可用生物辨識解鎖，生物特徵僅存於本地  

缺點：  
* 須辦帳號  
* 幾乎形同沒文件，對開發者不友善  
* 疑似不支援 Linux  

無明顯商業模式，推測可能是內部使用  
只不過寫都寫了，就放開源給大眾共享  

#### [Proton Authenticator](https://proton.me/authenticator)  
老面孔 Proton，台裔瑞士物理學家創立  
開源、免費、跨平台，所有主流系統都能用  
_# Linux、Windows、Mac，手機 iOS、Android 皆可下載_  
不需帳號，支援 TOTP、HOTP  
提供端對端加密備份、同步，不過此功能需 Proton 帳號  
_# 免費帳號就行，畢竟沒登入誰知道你哪位_  
可掃碼、手動綁定 OTP 服務，功能基礎但充足  

缺點：  
* App 還很新，偶爾會有 bug、運作不穩定  

有趣的是， 明明已有 Proton Pass 能處理兩步驟驗證  
他們還出 Proton Authenticator，引發社群好奇討論  
此程式相對輕量，只有 2FA 相關功能  
且不需訂閱 Proton，完全免費  
_# Proton 訂閱方案「不包含」此產品，所以本篇歸為**非營利**_  

#### [Ente Auth](https://ente.io/auth/)  
即 [Ente Photo](https://ente.io/) 那家公司，背景可見[這篇](./deGoogle-drive-and-album.md)  
支援各大主流平台，手機電腦都行  
_# [Android](https://f-droid.org/packages/io.ente.auth/)、[iOS](https://apps.apple.com/us/app/ente-auth-2fa-authenticator/id6444121398)、[Linux](https://github.com/ente-io/ente/releases?q=tag%3Aauth-v4)、[Mac](https://github.com/ente-io/ente/releases/download/auth-v4.4.4/ente-auth-v4.4.4.dmg)、[Windows](https://github.com/ente-io/ente/releases/download/auth-v4.4.4/ente-auth-v4.4.4.dmg)_  
免費、[開源](https://github.com/ente-io/ente)、不需帳號，提供端對端加密的雲端備份  
_# 和 Proton Authenticator 一樣，雲端備份請辦帳號_  
此項目完全免費，無訂閱方案  
所以儘管 Ente 是商業公司，Ente Auth 仍算非營利項目  
Ente Auth 棲位與 Proton Authenticator 接近，但相對成熟  
支援 TOTP、HTOP，功能穩定、程式碼也積極維護  

缺點：  
* 美國公司開發、維護  
    _# 不過核心團隊、創辦者都是印度人_  

Ente Auth 廣獲社群好評，對新手也很友善  

#### [Aegis Authenticator](https://getaegis.app/)  
直翻神盾驗證器，支援 TOTP、HOTP  
[社群](https://github.com/beemdevelopment)發起的[開源](https://github.com/beemdevelopment/aegis)專案，[兩位](https://github.com/michaelschattgen)主要[開發者](https://github.com/alexbakker)都是荷蘭人  
可用生物辨識、密碼解鎖，也能自訂排序、圖示、有暗色主題  
從各種服務匯入 / 匯出都相容，可匯出明文 / 加密資訊  
掃碼、手動綁定服務都行，亦可開啟「專家模式」細緻調教  

缺點：  
* 僅在 Android 發行  
Google Play、[F-Droid](https://f-droid.org/packages/com.beemdevelopment.aegis/) 都能下載  

社群評價很高，Android 用戶發問幾乎都會被推薦 Aegis  

#### [Stratum](https://stratumauth.com/)  
層疊驗證器，免費、開源、社群發起  
_# [主要貢獻者](https://jmh.me/)為法國人_  
從前叫 Authenticator Pro，不需帳號、能離線使用  
支援 TOTP、HOTP 等，介面可客製化、有暗色模式  
匯出 / 匯入容易，且先加密才轉出，讓你安全放到喜歡的雲端  
_# 官方未提供雲端，請自選[適當服務](./deGoogle-drive-and-album.md)，謝謝_  
最特別之處，莫過於「穿戴式裝置相容」，是少數設計給穿戴裝置的驗證器  

缺點：  
* 僅在 Android 發行  

沒辦法，*某公司*就很愛鎖生態系  

---  

#### [Tofu](https://tofuauth.com/)  
社群的[開源](https://github.com/iKenndac/Tofu?tab=readme-ov-file)專案，免費、不需網路  
看到「豆腐 (Tofu)」，就以為是華人功勞嗎？  
不，[發起](https://github.com/calleluks)、[繼任者](https://github.com/iKenndac)都是瑞典人  
免帳號、支援 TOTP、HOTP，基礎功能都有  

缺點：  
* 僅發行 iOS 版 (Android 好像也不缺這個？)  
* 備份只能靠 iOS 機制，如 iCloud、iTune / Finder 連至 Mac  

機密存於 iOS keychain，是好是壞就看你對蘋果的信任度囉！  

#### [Mauth](https://github.com/X1nto/Mauth?tab=readme-ov-file)  
官方說唸做「Moth」，是社群發起的開源專案  
_# 開發者喬治亞人，喬治亞尚未入歐盟，所以不算 EU alternative_  
[作者說](https://github.com/X1nto/Mauth?tab=readme-ov-file#inspiration)既有產品介面不直觀，所以自己做一個  
主打功能多、好看、隱私，支援 HOTP 和 TOTP  
可用密碼或生物辨識解鎖，也能掃碼、手動、或輸入深度連結綁服務  
_# Deeplink 名字很炫，但其實只是「導向至特定頁面的超連結」_  
許多功能尚在開發中，上次維護是 7 個月前，可能要等很久  

缺點：  
* 僅有 [Android](https://f-droid.org/en/packages/com.xinto.mauth/) 版  
* 文件更新落後，已有的功能沒全寫上去  

介面高度可客製化，能調成喜歡的樣子  

---  

### 加碼！  
之前[介紹過](./deGoogle-pswd-manager.md)密碼管理軟體，此時派上用場啦！  
許多密碼管理軟體，也附帶 OTP 驗證功能  
例如 [KeePassXC](https://keepassxc.org/)、[Proton Pass](https://proton.me/pass)、Bitwarden  
_# KeePass 系列都有_  
已入坑密碼管理器的，可直接使用  

---  

### 懶人包~~在我身上~~  
同樣依照需求推薦：  
* 想要穩定、老牌服務 → [FreeOTP](https://freeotp.github.io/) / [2FAS](https://2fas.com/auth/)  
* 喜歡一個服務用到底，最好各平台都支援：  
    * 不~~爽~~想辦帳號 → [Proton Authenticator](https://proton.me/authenticator) / [Ente Auth](https://ente.io/auth/)  
    * 可接受辦帳號 → [Authman](https://authman.simular.co/)  
* 新手，什麼都不想懂，無腦入坑就好 → [Ente Auth](https://ente.io/auth/) / [Proton Authenticator](https://proton.me/authenticator)  
* 想要完備服務：  
    * Android 用戶 → [Aegis Authenticator](https://getaegis.app/) / [2FAS](https://2fas.com/auth/)  
        * 有穿戴裝置需求 → [Stratum](https://stratumauth.com/)  
    * iOS 用戶 → [2FAS](https://2fas.com/auth/)  
* 極簡主義者：  
    * iOS → [Tofu](https://tofuauth.com/)  
    * Android → [Mauth](https://github.com/X1nto/Mauth?tab=readme-ov-file)  
* 密碼管理軟體用戶：  
    * [KeePass](https://keepassxc.org/) 系列 → 請繼續用  
    * [Bitwarden](https://bitwarden.com/download/) → 裝手機應用程式即可  
    * [Proton Pass](https://proton.me/pass) → 繼續用吧！  

---  

### 遺珠之憾？  
#### Bitwarden Authenticator  
你或許會問，有介紹 Proton Authenticator，為何漏掉 Bitwarden Authenticator？  
答案很簡單，官方[不再維護](https://github.com/bitwarden/authenticator-ios) Bitwarden Authenticator 了  
_# 技術上來說，它已被[封存](https://github.com/bitwarden/authenticator-android?tab=readme-ov-file)_  
Bitwarden 將之[併入](https://github.com/bitwarden/ios)手機 app，二者直接[合一](https://github.com/bitwarden/android)  
免費、開源，歡迎自由取用  

#### [andOTP](https://github.com/andOTP/andOTP?tab=readme-ov-file)  
曾享負盛名的 andOTP，也已不再維護  
程式碼被封存，因為[作者](https://xdaforums.com/t/unmaintained-app-4-4-open-source-andotp-open-source-two-factor-authentication-for-android.3636993/post-87021655)大學畢業後，沒足夠時間無償付出  
身為 Android 開源驗證器先鋒，終止確實可惜  

#### [OVault](https://ovault.net/)  
iOS 的開源驗證器，使用 iOS keychain  
地端存放資料，不需連網  
免費使用、開發者為英國人  
他當初覺得 Authy 太複雜，決定自己做個簡單、方便的  
支援 TOTP、HOTP，能用 iCloud 同步、備份  

看起來不錯，為何沒介紹？  

因為沒特別好，且使用人數少  
用戶少的缺點，就是會跑去幫忙開發、審核的也少  
漏洞不易發現，維護進程也相對慢  
結論就是**無重大缺失**，你想用我也沒意見  
就當報給你知  

#### OTPAuth  
抱歉，此非遺珠之憾，而是刻意排除  
OTPAuth 是 iOS 平台的驗證器，「號稱」開源、免費  
問題是[作者程式碼倉庫](https://github.com/CooperRS)，**找不到原始碼！**  
還記得一路走來，最忌諱什麼嗎？  
謊言行銷，尤其假開源  
就算是良善 app，不開源就上不了推薦榜  
且蓄意誤導大眾，實在不可取  

---  

Apple Authenticator，為何沒在替換名單內？  
首先，它可離線使用  
且蘋果提供進階資料保護 (Advanced Data Protection)，能自行切換  
若開啟 ADP，蘋果驗證器即享端對端加密，可在雲端同步、備份  
雖然閉源，但尚無重大缺失  
所以不推薦，可是也不到替換標準  
果粉可以~~親吻對方~~歡呼了  


