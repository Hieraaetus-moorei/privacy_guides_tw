# deGoogle - 密碼管理軟體  

> 用 Email 註冊，或以 Google 連動登入  

雖然那不是 Google 密碼管理軟體，但許多人用 Google 連動登入，無非就是圖個方便  
_# 慶幸的是， Google 密碼管理員，似乎沒什麼人用_  

好用的密碼管理工具，也能做到一鍵登入  
且不必冒著交出密碼的風險，尤其對象是 Google  
儲存帳密、連動登入，幾乎形同告訴 Google 你用哪些服務  
甚至把「備用鑰匙」交給它，及[躲藏在後](https://www.amnesty.org/en/latest/news/2025/02/global-googles-shameful-decision-to-reverse-its-ban-on-ai-for-weapons-and-surveillance-is-a-blow-for-human-rights/)的[美國國安局](https://epic.org/documents/epic-v-nsa-google-nsa-relationship/)  

進入正題前，得先解釋一下「密碼管理軟體」  
那是什麼、為什麼需要，已具背景知識者可略過  

---

### 密碼管理軟體  
#### 什麼是密碼管理軟體？  
很簡單，就是記錄帳密的軟體，類似密碼本  
好處是方便性高，登入時只需點擊按鈕  
很多人用瀏覽器記錄密碼，也有異曲同工之妙  
    瀏覽器記錄密碼較危險，因為：  
* 瀏覽器常綁定供應商帳號，例如 **Google** Chrome、**Apple** Safari  
    密碼管理工具多半獨立，且有主密碼、零知識端對端加密  
* 瀏覽器的密碼工具，僅有基本功能  
    密碼管理軟體多附帶密碼強弱檢查、高強度密碼生成、多身份驗證、保險庫分群...  
    _# 想不到高強度密碼，可用軟體幫你生_  
* 安全性低，只要瀏覽器被攻破，密碼就可能外洩  
    很多人瀏覽器裝滿外掛，往往沒先查過是否安全  
    攻擊面積太廣，甚至連怎麼被駭的都不知道  
    網站惡意腳本，也有機會入侵瀏覽器資訊  
    密碼管理軟體獨立分層，且靠主密碼隔離帳密  
    加密後哪怕瀏覽器真被攻破，也只是一堆亂碼  

何況有些瀏覽器，[設計上故意開後門](https://cybernews.com/security/microsoft-edge-loads-cleartext-passwords-to-memory/)，把你的密碼奉送給不肖人士  
_# 微軟 Edge 會把瀏覽器密碼[明文](https://www.forbes.com/sites/daveywinder/2026/05/06/microsoft-says-edge-password-security-vulnerability-is-by-design-is-it-time-to-switch-to-chrome/?streamIndex=0)存在記憶體裡，比 Chrome 還不安全呢！_  
想像瀏覽器是你家，為了正常活動，戒備通常不會太森嚴 (除非你是總統)  
把存摺、印章一起放桌上，只要被闖空門就會損失慘重  
密碼管理軟體就像保險箱，家門被入侵仍非常安全  

若不綁帳號，換瀏覽器或裝置時，就得大量匯出、匯入資料  
但密碼管理軟體可跨平台、跨瀏覽器使用，兼顧方便與安全  

#### 為什麼需要密碼管理軟體？  
除上述原因，密碼管理軟體對「資訊安全」有莫大幫助  
大眾喜歡用「懶人密碼」，也習慣「重複使用密碼」  
但以[資安角度](https://blog.trendmicro.com.tw/?p=81252)來看，那是非常[危險](https://specopssoft.com/blog/password-reuse-hidden-danger/)的行為  
因為：  
1. 進行破解、滲透行為時，駭客常會先用外流密碼表  
    各種常用密碼，如1234qwer (鍵盤左起第一、二排)、abcd1234 等當然都逃不掉  
2. 若重複使用密碼，當一處密碼外洩，你的所有帳號都可能被破解  
    更別提如果用懶人密碼，駭客甚至不必破解你任一帳號，就能直接非法存取  
    _# 密碼不必環保，請每次都用新的_  
3. 當然，拿生日、英文名當密碼，也很危險  
    危險的來源，主要是你的親友、知道你生日的人  
    ~~畢竟撿到朋友手機，當然是先猜生日、男 / 女友生日、英文名啊！~~  

既然那麼可怕、大眾也知道風險 (也許知道？)，為何許多人仍照做呢？  

因為「高強度密碼」很麻煩，而且多數人記不住啊！  
高強度密碼需要：**英文大小寫 + 數字 + 特殊符號 + 沒在外洩密碼表上**...  
設想當你辦帳號時，填了個超複雜密碼  

完美，對吧？  

那請問你辦其他帳號時，每次都會想一組高強度密碼、而且背起來嗎？  
別忘了重複使用，一樣很危險  
有些人怕忘記，會把密碼寫上便利貼、黏在螢幕或桌邊  

![shocked Barbie face](https://media.tenor.com/ijQ5N2nw640AAAAC/disgusted-disgusting.gif)  

此舉會讓同事、朋友、任何可物理性接觸你電腦的人，都能登入你的帳號  
那我寫進筆記本，隨身攜帶好好保護，總行了吧！  
那是個可行的做法，但有兩個缺點：  
1. 不方便  
    每次要登入，都得翻筆記本，而且萬一筆記本損毀，你的帳號就...  
2. 沒加密  
    如果被偷或遺失，別人可直接存取你的帳密  

所以密碼管理軟體就來啦！  

類似瀏覽器，能記住你的帳密  
需要時自動填入，非常方便  
因此用再難的密碼都行，反正不用你背  
_# 有些密碼管理軟體，還附帶「生成高強度密碼」功能_  
選擇開源、端對端加密者，就不怕特定公司掌握你帳密  
甚至能匯出密碼，換裝置時跟著連動，方便又安全  
密碼管理軟體就像手抄密碼本，只是多了安全、方便性  

若配合 2FA (雙因素驗證，Two Factor Authentication)，能提升更多安全性  
雙因素驗證指「除了密碼，還要再過一關」 (第二個因素)  
是 MFA (Multi-Factor Authentication，多因素驗證)的一種  
簡單說就是光密碼不夠，須更多條件才准登入，如同有兩道家門  
常見做法有 Email 認證信、簡訊驗證，和其他 app 驗證等  
_# 即使帳密被盜，對方沒你的手機 / 信箱 / 驗證 app，仍無法登入_  

---

背景知識介紹結束  
### 來看圖吧！  
[deGoogle password manager](image link)  
<sup>製圖者：只能是我</sup>  
<sup>FOSS 指免費開源軟體 (Free and Open Source Software)</sup>  
<sup>non-profit 指「不以營利為目的」</sup>  
應該不必多說，鑑於 Google 過去[作為](https://campaignsoftheworld.com/news/the-dark-side-of-google/)，只有傻子才把密碼給它管  

替代品來嘍！  
#### [KeePassXC](https://keepassxc.org/)  

---

講古：  
[KeePass](https://keepass.info/) 是密碼管理軟體專案，開源、由社群發起  
僅支援 Windows，且介面不太友善、運作緩慢  
_# Linux、MacOS 需安裝外掛_  
於是社群開發者分支出 KeePass/L (KeePass Linux 版)，後來又支援 Mac  
因為變成跨平台，不只 Linux，於是改名 [KeePassX](https://www.keepassx.org/)  
不過 KeePassX 開發緩慢，後來甚至不再更新  
等不下去的開發者，~~憤而~~再分支出 KeePassXC  
要知道最強的工程師，不在特定企業裡  
而是分布在世上各角落，活躍於社群中  
KeePassX 以 C++/Qt5 重構，比 C#/.net 寫成的 KeePass 高效許多  
而且原生支援多平臺，不需外掛  
KeePassXC 同樣為 C++ 專案，高效、跨平台特性都沒少  
使用者介面也較佳，因此迅速竄紅  

---

KeePassXC 可離線存放密碼，支援 AES 256、ChaCha20、Twofish 等加密演算法  
_# 不知道那些是什麼別緊張，裝作沒看到就好_  
Linux、Windows、MacOS 都能用，也有瀏覽器外掛  
開源、定期由第三方審查，內建 TOTP 功能  
_# Time-based One-Time Password, 有時效的一次性密碼_  
存取權受密碼保護，還需額外一層金鑰才能開  
官方建議將金鑰檔存在 USB 等可移除裝置上，不用時就拔掉  
_# 插上一個東西才能用，像特務片那樣，酷吧？_  

缺點：  
* 初次使用可能需摸索一下，詳見官方[說明](https://keepassxc.org/docs/KeePassXC_UserGuide)  

社群自發、開源，完全免錢、無隱藏費用  
想要功能強大、可自訂的密碼管理軟體，非此莫屬  

#### [Proton Pass](https://proton.me/pass)  
Proton 老面孔了，公司背景在 [Email 那篇](./deGoogle-email.md)介紹過  
主打開源、保障隱私，有各種常用線上服務  
_# [Email](./deGoogle-email.md)、[雲端硬碟](./deGoogle-drive-and-album.md)、[月曆](./deGoogle-calendar.md)... 都有_  
Proton Pass 開源、端對端加密，支援電腦、手機、瀏覽器  
瀏覽器外掛可獨立作業，不需先下載電腦端軟體  
線上、離線服務都行，還能多設一層密碼保護  
可儲存帳密、生成高強度密碼、自動填寫等  
亦可當 2FA 應用程式，讓你登入不必拿其他裝置  
還支援密碼金鑰 (passkey)，功能非常完備  

---

簡介 passkey：  
密碼金鑰是認裝置的唯一碼，只要裝置不離手就不怕被盜  
安全性的保障來自：**沒密碼就不怕偷** (Passkey ≠ Password)  
_# 只要你確定裝置安全_  
許多服務都可選密碼金鑰登入，比密碼更方便  
_# Google 用密碼金鑰就不必 2FA_  

Proton Pass 商業模式採訂閱制，但免費版非常夠用 (基本上不需訂閱)  
_# 若認同 Proton 的理念，訂閱是一種支持，就像買專輯一樣_  

缺點：  
* 從前速度很慢，但近期已大幅改善  

如有使用 Proton Mail，Proton Pass 還能幫你管理信箱別名 (Email Alias)  
喜歡整合生態系的使用者，不妨考慮看看  

#### [KeePassDX](https://www.keepassdx.com/)  
KeePassDX 同樣是 KeePass 系列，開源、免費享有多數功能  
_# 可購買 Pro 外觀、捐款贊助，但非強制_  
鑑於 KeePassXC 支援各大桌面平台，但行動版付之闕如  
[Kunzisoft](https://www.kunzisoft.com/) 便推出 KeePassDX，讓 Android 用戶也擁有 KeePass 服務  
iOS 用戶可選 [AuthPass](https://authpass.app/)、[KeePassium](https://keepassium.com/pricing/)，前者免費、與 KeePass 相容  
後者免費版功能受限，兩個都開源  
_# Strongbox 沒被推薦，是因為它閉源卻用開源行銷_  
KeePassDX 支援各種 KeePass 加密演算法，也支援生物辨識解鎖  
若你的手機能靠人臉、指紋解鎖，KeePassDX 就能用相同方式鎖定、解鎖  
_# 這樣就算滑手機時突然被搶，也不怕密碼外流_  

缺點：  
* 僅支援 Android  
    iOS 系列有相應替代品，但鑒於生態系閉鎖、強制綁蘋果商店、與 GPL 授權不相容  
    此處就不特別提，要怪請怪蘋果 (蘋果稅阻卻許多開發者)  
可從 Google Play、[F-Droid](https://f-droid.org/) 下載 (官方建議從 F-Droid)  
_# [F-Droid](https://f-droid.org/) 是免費開源軟體商店，本身也開源、去 Google 化，可見[這篇](./deGoogle-appStore.md)_  

#### [Bitwarden](https://bitwarden.com/)  
Bitwarden 是開源、知名的密碼管理軟體，訂閱制收費  
商用有不同方案，個人用則有免費版  
免費版功能齊全，和 Proton 的模式相似  
支援各大平台，包括電腦和手機  
也有瀏覽器外掛，一個軟體就能打天下  
最大的好處是，伺服器可自架  
同樣加密保護密碼，是廣受大眾喜愛的選擇  

缺點：  
* 美國公司  
    身在美國，受美國法律管束  
    好處是開源，至少能審核安全性  
    _# 相較之下，Proton 是瑞士公司，不受制於美國法律_  

#### [Spectre](https://spectre.app/)  
直翻幽靈，嚴格來說不算密碼管理軟體  

不是密碼管理軟體，放這幹嘛！？  

別急，就像[聯合國秘書長說的](https://www.un.org/sg/en/content/sg/speeches/2023-10-24/secretary-generals-remarks-the-security-council-the-middle-east%C2%A0)，事出必有因 (？)  
Spectre 是「密碼演算器」，可以做相似的事  
開發哲學是：「唯一不會被偷、勒索、遺忘的密碼，只有不存在的密碼」  
> The only password that can’t be lost, stolen, seized, ransomed or left on the bus, is a password that doesn’t exist.  

[原理](https://spectre.app/#algorithm)是透過密碼學[演算法](https://spectre.app/spectre-algorithm.pdf)，「生成」密碼：  
使用者只需填入姓名 (或暱稱)、固定秘密 (可想成主密碼)  
演算法會生成一把主鑰，碰到每個網站再依主鑰生成「唯一」、「不可逆推」的密碼  
如此一來，就算某個網站出事，其他帳號仍非常安全  
密碼不儲存在任何地方，就無法被偷  
_# 此做法稱為「無狀態 (Stateless)」密碼管理_  

---

講古：  
比利時裔[加拿大人](https://lhunath.com/)開發，專案[開源](https://gitlab.com/spectre.app/)、支援各大電腦與手機平台  
_# 作者專攻資安領域，自稱夢想家、理想主義者_  
原本名為「One Password」，因其只需一支密碼  
後更名為「Master Password」 (主密碼)，從 App Store 開始上架  
後來經過重構，程式邏輯優化、介面現代化，擴展到各平台  
品牌也重塑為 Spectre，至今已有十年歷史  

---

缺點：  
* 使用有些微門檻  
    * Windows 用戶須先下載 Java  
    * Mac 套件管理工具 [Homebrew](https://brew.sh/) 似乎不支援了，得由蘋果 App Store 下載  
* 主程式年久未維護，穩定與安全性堪慮  


#### [LessPass](https://lesspass.com/)  
原理和 Spectre 相似，都用「生成」取代「儲存」密碼  
一樣是[開源](https://github.com/lesspass/lesspass)、社群專案，支援手機平台、瀏覽器外掛  
_# Android 版在 [F-Droid](https://f-droid.org/) 也能下載_  
創建者是法國人 [Guillaume Vincent](https://github.com/guillaumevincent)，紅帽 (Red Hat)公司首席軟體工程師  
_# 熟悉開源的人鐵定不陌生，此紅帽即為 Linux 發行版那家公司_  
開發者自稱「開源成癮者」、人文主義者，應不會隨意背棄專案  
完全免費使用，沒有商業模式 (創立目的非賺錢)  
原先伺服器位於法國，但侵害隱私的[情報法案](https://www.amnesty.org/en/latest/news/2015/07/france-new-surveillance-law-a-major-blow-to-human-rights/)通過後，[伺服器遷至德國](https://medium.com/@guillaume20100/who-are-you-what-is-your-secret-where-are-you-going-60800e93f92)  
_# 可離線使用，此處指網頁伺服器_  

缺點：  
* 無桌面程式  

叫 'Less' 有種「少即是多」的意味，沒密碼就不用記密碼、不怕外洩  
而且還有在積極維護，選 LessPass 比 Spectre 更安全  

---

### 懶人包來啦！  
* ~~無腦~~一般使用者，想要「方便就好」→ [Proton Pass](https://proton.me/pass)  
* 樂意花時間設定：  
    * 桌面 → [KeePassXC](https://keepassxc.org/)  
    * 手機：  
        * Android → [KeePassDX](https://www.keepassdx.com/)  
        * iPhone → [AuthPass](https://authpass.app/)  
* 已在用 Bitwarden、可能需要中文社群支援 → [Bitwarden](https://bitwarden.com/)  
    _# Bitwarden 在台灣知名度不低，隨便搜都有很多文章_  
* 喜歡酷玩意 → [LessPass](https://lesspass.com/)  
    * 有技術能力、願意冒風險 → [Spectre](https://spectre.app/)  

---

其他隱私保障做再多，若密碼輕易被破解，帳號被盜、身份被竊一樣危險  
選一款喜歡的，就只需記住一組密碼 (密碼管理軟體的密碼)  
之後使用各大服務，都能暢行無阻又不失安全  
_# 或是你也可以跟我一樣，用腦記住一堆高強度密碼，但哪天忘記帳密別找我_  

**注意**：密碼管理軟體不防呆，把密碼貼在螢幕、桌上的，立刻給我撕掉！  

