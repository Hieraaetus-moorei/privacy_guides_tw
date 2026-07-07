# 開源等於隨便用嗎？

![cc by nc nd logo](https://images.unsplash.com/photo-1562412692-26406e1bf600?crop=entropy&cs=srgb&fm=jpg&ixid=M3wyNTY4N3wwfDF8c2VhcmNofDF8fGNvcHlyaWdodHxlbnwwfHx8fDE3NTQ0NTQxMzB8MA&ixlib=rb-4.1.0&q=85)

> 在軟體、AI界，常聽到「開源」一詞，但開源究竟是什麼？
> 是隨便用的意思嗎？

開源 (open source)一詞，相對於專有 (proprietary)、或閉源 (closed source)
專有軟體需獲得授權才能使用，通常：
1. 程式碼不公開 (可能是商業機密)
2. 不能自由分發 (否則侵權)
3. 要錢 (很貴)
4. 背景運作細節不明 (含「主要功能以外」的東西，可能藏在同意條款中，也可能偷偷來)

例如：你買了 Windows 電腦，只是希望有個「即開即用」的體驗
首先，大部分 Windows 的程式碼都不公開，所以你不知道裡面有些什麼
再來，你不能任意拷貝 Windows 系統，安裝給其他電腦 (或許你做得到，但此行為就是「**盜版**」)
第三，買 Windows 電腦要錢
你可能會說，我花的是硬體的錢，但軟體費早就包含在零售商的電腦價格中了，你實質上「付了硬體和軟體的錢」
第四，很多人可能沒關注，微軟的 [Windows Recall](https://brave.com/privacy-updates/35-block-recall/) 每幾秒就會進行螢幕截圖，號稱是為了 AI 體驗，但鑑於微軟過去的[惡形惡狀](https://www.justice.gov/archives/opa/pr/microsoft-agrees-pay-20-million-civil-penalty-alleged-violations-children-s-privacy-laws)，你的個資、機密早已不是你的
所以不少開發者，倡議、帶頭實行「開源」，也就是公開原始碼，任何人都看得到
而且不只公開原始碼，更允許多種形式的取用
例如直接使用、修改內容再推出新品 (有點像你買了衣服，改個配色就賣出，還說那是自己的)、甚至允許商用
開源的好處，不只讓大眾享受免費、安心的軟體，還能避免其他開發者「重複造輪」
也就是輪子 (有某功能的程式)已被發明，其他人不必浪費數小時甚至數天，再做出一模一樣的輪子
開源可促進互相學習 (東西已經有了，可參考他人之作再行創新)、刺激良性競爭 (你有的東西大家都有，不繼續前進就等著被超車)、易於推廣作品 (要錢、不透明的產品 vs 免費、透明，多數人應該會選後者)

---

### 開源定義
對於開源，不同人可能有不同定義
廣為接受的開源共識，至少需符合以下特性：
* 可自由重新分發
    即取用、複製該作品不應受限制，且不得要求付費
* 開放原始碼 (廢話，不然哪叫開源？)
    程式碼要公開，讓大家都能看到
* 允許修改、產出衍生作品，且允許衍生作品開源

若每個人分發軟體都要寫一份授權書，可能定義會因人而異 (每個人表達方式不同)，使用者每次都得讀長文，實在很困擾
因此許多機構紛紛推出開源「定型化契約」，也就是公定版開源授權書
開發者僅需複製貼上、使用者看授權書名就知道，很方便吧？

---

### 常見的開源授權條款
* General Public Licence, [GPL](https://www.gnu.org/licenses/gpl-3.0.en.html)
    此系列起源甚早，有各種變體
    特徵就是條款超長，且有感染性 (infectious 或稱 viral effect)，因為其規定衍生作品、有引用「任何一行程式碼」者，也**須用相同方式授權**
    其中最嚴厲者 [AGPL](https://www.gnu.org/licenses/agpl-3.0.en.html) 更要求，「用於網路分發、架設線上服務」的程式碼，也得跟著開源
    _身為極端開源信徒，我超愛這東西！_
* [Apache licence](https://www.apache.org/licenses/LICENSE-2.0)
    由 Apache 基金會制定，相較 GPL 快十頁 A4 的條款，「只有」一兩頁 A4 寫滿
    且不要求衍生作品開源與否，僅須載明修改了什麼、附上原始授權聲明就行
* Berkeley Software Distribution Licence, [BSD](https://opensource.org/license/bsd-3-clause) Licence
    加州大學柏克萊分校推出的，非常簡明
    幾乎可說是只要求開源基本定義、附上著作權聲明，其他隨便
* [MIT](https://opensource.org/license/mit) Licence
    _# 此 MIT 是麻省理工學院，不是台灣製造_
    條文同樣非常短，和 BSD 有 87% 像，除了著作權聲明也要求附上副本，同樣很寬鬆
    兩者都一頁 A4 不到，就算全讀完也花不了幾秒鐘
* Creative Common, [CC](https://creativecommons.org/licenses/by/4.0/)，即大名鼎鼎的[創用 CC](https://creativecommons.org/licenses/by/4.0/legalcode.zh-hant)
    CC 系列常用於藝文創作，較少用於軟體、AI 模型，常有「程式碼 MIT 授權、文章 CC-BY 4.0」此類混血
    但有幾家公司特立獨行，喜歡用 CC 條款授權 AI 模型，例如加拿大 [Cohere](https://huggingface.co/CohereLabs/command-a-vision-07-2025)、美國 [Nvidia](https://huggingface.co/nvidia/OpenMath-Nemotron-14B)
    常用的版本有 [CC0](https://creativecommons.org/publicdomain/zero/1.0/deed.en)，即公領域授權 (public domain)，白話文就是**放棄著作權 (no right reserved)**，誰愛用、愛怎麼用都行
    還有 [CC-BY](https://creativecommons.org/licenses/by/4.0/)，要求標示作者姓名；[CC-BY-SA](https://creativecommons.org/licenses/by-sa/4.0/deed.en) 要求衍生作品用相同方式分發 (和 GPL 「感染性」有異曲同工之妙)；[CC-BY-NC](https://creativecommons.org/licenses/by-nc/4.0/) 不可商用等
    基本上 CC 是本體，其他 BY (by attribution)、NC (NonCommercial)、SA (Share Alike)等裝備可任意搭配，作者爽就好

---

### AI 產業的開源
AI 產業和傳統軟體開發，對「開源」的詮釋略有不同
傳統開源，往往授權整個專案
但 AI 模型則常常只開源一小部分，甚至非真開源，就以開源名號做行銷
訓練一個 AI 模型，重要的成分有：
* 模型權重 (weight, 即模型本身)
* 訓練資料 (training dataset)
* 訓練 / 部署用程式碼 (training / deployment code)

各位常聽到的 Meta Llama、Stable Diffusion 模型，就是權重、程式碼開源，但訓練資料不公開的經典案例 (Black Forest Labs 比較誠實，說旗下的 [Flux](https://huggingface.co/black-forest-labs/FLUX.1-dev) 是「[開放權重](https://bfl.ai/blog/flux-1-kontext-dev)」模型)
DeepSeek 旗下的 Janus 系列製圖模型，則是僅開放模型權重，其他都不給看
[Nvidia](https://huggingface.co/nvidia/OpenMath-Nemotron-14B)、[TII](https://huggingface.co/datasets/tiiuae/falcon-refinedweb) 則部分模型有公開訓練資料、權重、程式碼、甚至訓練細節，是少見的慷慨做法

---

### 趣聞
大家耳熟能詳的 Stable Diffusion、Llama 系列模型，向來享有「開源」美譽
然而，就算不計入訓練資料，他們仍**非**真開源
前面提到，開源必須允許衍生作品、自由分發，但 Stable Diffusion 與 Llama、DeepSeek V3、阿里巴巴[部分 Qwen 模型](https://huggingface.co/Qwen/Qwen2.5-3B-Instruct)，都有限制使用範圍
有的規定「獲利」、「每月活躍使用者」超過門檻，就必須另行申請授權 (當然不會免費)
簡言之就是賺錢的企業會變標靶，他們也要分一杯羹
Llama 的限制更多，除了賺太多要分潤外，還要求微調後的模型需冠名，所以才有不少模型叫 llama-ooxx-@#%^，例如聯發科的 [Breeze](https://huggingface.co/MediaTek-Research/Llama-Breeze2-8B-Instruct)、Nous research 的 [Hermes](https://huggingface.co/NousResearch/Hermes-3-Llama-3.1-405B)
從前只有 GPT 的時代，開源語言模型很少，大家想客製化自己的模型，就只能接受 Meta 的假開源條款
_# 註：GPT 的公司 OpenAI 雖然名字裡有 Open，但知名模型全都閉源，因此被諷為「CloseAI」。直至截稿日前才開源[一組](https://huggingface.co/openai/gpt-oss-120b) GPT 模型_
但後來開源模型如雨後春筍般冒出，有更好、更寬鬆的模型能用，很多人就不理 Meta 了

---

總之，看到軟體、模型寫「開源」時，不代表能恣意亂用
記得先看是什麼授權條款，多數真開源也不代表「拿去用不必註明出處」，多半是需要給作者榮譽標註的喔！



