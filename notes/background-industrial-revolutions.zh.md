# 工業革命：以電力化作為主線

*給喜歡深入理解的工程師看的參考資料。* 以下每個日期與數字都已對照一手資料或可信的二手資料；內文連結會指向來源，文末也有彙整的 **資料來源**。如果某個常見數字本身模糊或有爭議，文中會明確標出。

這篇之所以值得軟體工程師花時間讀，是因為科技史裡最有用的一個模式是：**general-purpose technology（GPT，泛用技術）通常在發明後數十年，才會真正出現在 productivity（生產力）統計裡。** 蒸汽機如此，電力更是戲劇性地如此，電腦也是如此；而 AI 現在很可能也正在重演這個過程。電力化是我們手上最清楚的案例，所以本文會用它作為貫穿全篇的主線。

---

## 0. 心智模型：泛用技術與滯後

所謂 *general-purpose technology*，是指一種技術會 (a) 擴散到整個經濟體，(b) 持續改善，且 (c) 催生互補創新。蒸汽、電力、內燃機、電腦，以及（很可能）AI，都符合這個定義。

反覆出現的轉折是**滯後**。你裝上新東西之後，很長一段時間裡，每工時產出幾乎不動，有時甚至下降。然後，通常要到數十年後，productivity 才突然起飛。這個想法有兩篇經典參考：

- **Paul David (1990)**，*"The Dynamo and the Computer: An Historical Perspective on the Modern Productivity Paradox"*，用電力化來解釋為什麼 1980 年代的電腦會像 Robert Solow 的妙語所說，到處都看得到，唯獨在 productivity statistics 裡看不到。([American Economic Review / AEA](https://www.aeaweb.org/articles?id=10.1257/aer.80.2.355), [PDF via academia.edu](https://www.academia.edu/11211365/The_Dynamo_and_the_Computer_An_Historical_Perspective_on_the_Modern_Productivity_Paradox))
- **Brynjolfsson, Rock & Syverson (2018/2021)**，*"The Productivity J-Curve: How Intangibles Complement General Purpose Technologies"*，把背後機制形式化：新的 GPT 需要大量、難以衡量的**無形**投資（流程重新設計、新商業模式、人力資本）。一開始，產出與 productivity 會被*低估*（你正在花錢打造統計沒有計入的無形資產）；後來，當那些無形資產開始回收，productivity 看起來就會暴衝。曲線會先下探再上升，也就是一個「J」。([NBER w25148](https://www.nber.org/papers/w25148), [AEA AEJ:Macro](https://www.aeaweb.org/articles?id=10.1257%2Fmac.20180386))

先把這個模型放在腦中。下面每一段都是它的實例。

---

## 1. 標準分期

歷史學家與經濟學家通常把工業化分成三到四次「革命」。邊界並不銳利，標籤（尤其是第四次）也有爭議，但這個基本架構被廣泛採用。

### 第一次工業革命（約 **1760** 到 **1840**）

> **GPT：蒸汽機。** 另外還包括：水力、機械化紡織、鐵，以及真正的制度性發明：工廠系統。

**因 → 果。** 英國有便宜的煤、昂貴的勞動力、深厚的資本市場，以及專利制度。這個組合讓機械化變得值得投資。突破性的裝置是 James Watt 的**分離式冷凝器**，在 **1769 年 1 月 5 日**以 *"A New Method of Lessening the Consumption of Steam and Fuel in Fire-Engines"* 為題取得專利。它讓 Newcomen 蒸汽機的煤耗大約下降三分之二，也就是讓蒸汽終於不只適合在煤礦區抽水，而能在遠離煤田的地方、甚至工廠內部，變得經濟可行。([Science Museum](https://blog.sciencemuseum.org.uk/james-watt-and-the-separate-condenser/), [Britannica: James Watt](https://www.britannica.com/biography/James-Watt))

**誰／什麼／在哪裡。** 英國，大約從 1760 年開始，到了約 1840 年擴散到歐洲大陸與美國。([Wikipedia: Industrial Revolution](https://en.wikipedia.org/wiki/Industrial_Revolution))

**具體例子。**
- **紡織：** Hargreaves 的珍妮紡紗機（約 1764）、Arkwright 的水力紡紗機、Crompton 的 mule（走錠精紡機）、Cartwright 的動力織布機：紡紗、接著織布，從家庭手工業轉向機械作業。([World History Encyclopedia: Steam Engine in the IR](https://www.worldhistory.org/article/2166/the-steam-engine-in-the-british-industrial-revolut/))
- **鐵：** 焦炭煉鐵與攪煉法擴大了廉價鐵的供給，可用於機器、鐵軌與建築結構。
- **工廠本身：** 真正新的「技術」是組織方式：把工人與機器集中在單一原動機（水車，後來是蒸汽機）周圍。

![晚期 Watt 雙作用樑式蒸汽機（D. Napier & Son，倫敦，1832），保存於馬德里高等工業工程技術學校](https://upload.wikimedia.org/wikipedia/commons/thumb/9/9e/Maquina_vapor_Watt_ETSIIM.jpg/640px-Maquina_vapor_Watt_ETSIIM.jpg)
*保存至今的 Watt 型雙作用蒸汽機。來源：[Wikimedia Commons — Maquina_vapor_Watt_ETSIIM.jpg](https://commons.wikimedia.org/wiki/File:Maquina_vapor_Watt_ETSIIM.jpg)*

注意這裡的動力架構：**一台大型引擎**轉動傳動軸與皮帶，驅動*所有東西*。先記住這點，因為電力化最大的回報，就是把這整套配置拆掉。

### 第二次工業革命（約 **1870** 到 **1914**）

> **GPT：電力化。** 這是本文的核心。圍繞它的還有：廉價鋼鐵（Bessemer 轉爐／平爐法）、工業化學、內燃機、電報／電話，以及大量生產。

**因 → 果。** 一群以科學為基礎的技術幾乎同時成熟，並彼此強化。廉價鋼鐵讓更大的機器、鐵軌與建築成為可能；電力提供乾淨、可分割、可傳輸的動力形式；電報與電話壓縮了通訊時間；可互換零件加上移動式生產線，帶來大量生產。這段時間通常被定為 **1870 到 1914 年**（以第一次世界大戰作為終點）。([Wikipedia: Second Industrial Revolution](https://en.wikipedia.org/wiki/Second_Industrial_Revolution), [Joel Mokyr, "The Second Industrial Revolution, 1870–1914"](https://faculty.wcas.northwestern.edu/jmokyr/castronovo.pdf))

**為什麼電力是核心。** 它是這個時代教科書級的 GPT：一個底層技術組合（發電 + 輸電 + 電動馬達），重新改造了照明、工廠、交通、通訊，最後也改造家庭。它完整的弧線會在下一節單獨展開。

**具體例子。**
- **鋼鐵：** Henry Bessemer 的轉爐（1850 年代取得專利）把空氣吹入熔融生鐵以燃燒掉碳，大幅降低鋼鐵成本，讓鋼取代熟鐵，用在鐵軌、橋梁、船舶與摩天大樓。([Lumen: Steel Production](https://courses.lumenlearning.com/suny-hccc-worldhistory2/chapter/steel-production/))
- **大量生產：** Ford 的移動式裝配線（1913，下文會提到）是最具代表性的案例。
- **通訊／化學／ICE：** 電話（Bell，1876）、合成染料與肥料，以及內燃機（ICE）都在這個窗口成熟。

![Bessemer 轉爐示意圖，這個裝置讓廉價大量鋼鐵成為可能](https://upload.wikimedia.org/wikipedia/commons/thumb/6/61/Bessemer_converter.jpg/512px-Bessemer_converter.jpg)
*Bessemer 轉爐。來源：[Wikimedia Commons — Bessemer_converter.jpg](https://commons.wikimedia.org/wiki/File:Bessemer_converter.jpg)*

### 第三次工業革命／數位革命（約 **1950 年代**到 **2000 年代**）

> **GPT：半導體／數位邏輯**（電晶體 → 積體電路 → 微處理器），催生電腦與網際網路。

**因 → 果。** 核心轉變是從機械式與類比電子，轉向**數位**電子：MOSFET、積體電路、微處理器，以及封包交換網路。這是一個資訊變成可處理、可移動，而且邊際成本近乎為零的時代。([Wikipedia: Digital Revolution](https://en.wikipedia.org/wiki/Digital_Revolution); 「第三次工業革命」這個標籤也與 Jeremy Rifkin 2011 年的書有關：[Wikipedia](https://en.wikipedia.org/wiki/The_Third_Industrial_Revolution))

**誰／什麼／在哪裡。** 美國與全球；Bell Labs、矽谷的 Fairchild/Intel、ARPANET 到 Internet、PC，最後到 Web。

**具體例子。**
- **ENIAC**（賓州大學 Moore School）：第一台通用電子數位電腦，於 **1946 年 2 月 14 日**公開亮相。([Penn Engineering](https://www.seas.upenn.edu/about/history-heritage/eniac/), [Wikipedia: ENIAC](https://en.wikipedia.org/wiki/ENIAC))
- **微處理器**（Intel 4004，1971）把 CPU 放到單一晶片上。
- **Internet / Web**：從 ARPANET（1969）到 TCP/IP（1983），再到 World Wide Web（1989 到 1991）。

![賓州大學 Moore School 的 ENIAC 面板與函數表](https://upload.wikimedia.org/wikipedia/commons/thumb/6/6c/ENIAC_Penn1.jpg/640px-ENIAC_Penn1.jpg)
*ENIAC，第一台通用電子數位電腦。照片 © Paul W. Shaffer, University of Pennsylvania，採 CC BY-SA 3.0 / GFDL 授權。來源：[Wikimedia Commons — ENIAC_Penn1.jpg](https://commons.wikimedia.org/wiki/File:ENIAC_Penn1.jpg)*

### 第四次工業革命／「工業 4.0」（約 **2010 年代**至今）－*有爭議*

> **被主張為 GPT 的技術：cyber-physical systems（CPS，資訊物理系統）、AI、IoT、robotics**，融合實體、數位與生物領域。

**標籤的來源。** 「The Fourth Industrial Revolution」由世界經濟論壇（WEF）創辦人 **Klaus Schwab** 透過 2016 年 1 月的書與當年 Davos 會議主題推廣開來。（「Industrie 4.0」則稍早源自德國製造業策略用語。）Schwab 的主張是，這些變化與第三次工業革命相比，在*規模、範圍與複雜度*上都不同。([WEF: "The Fourth Industrial Revolution: what it means" (2016)](https://www.weforum.org/stories/2016/01/the-fourth-industrial-revolution-what-it-means-and-how-to-respond/), [WEF press release, Jan 2016](https://www.weforum.org/press/2016/01/shaping-the-fourth-industrial-revolution-to-benefit-all-new-book-by-professor-schwab/))

**為什麼有爭議。** 不少經濟學家與歷史學家會說，這*不是*一場獨立的新革命，而是數位革命的延續：同一個 GPT（數位運算／半導體）正在成熟，而不是新的泛用技術誕生。「4IR」這套說法是 WEF/Schwab 在政策與顧問圈流行起來的框架；引用時應把它當成一個*品牌化*主張，而不只是歷史分期。

**具體例子（不論你怎麼稱呼這個時代）。** 深度學習與大型語言模型；雲端規模的資料中心；工業 IoT 與「智慧工廠」；自主系統與機器人。

![BalticServers 資料中心內的伺服器機櫃](https://upload.wikimedia.org/wikipedia/commons/5/5d/BalticServers_data_center.jpg)
*現代資料中心，也就是數位／AI 時代耗電量驚人的「工廠現場」。照片採 CC BY-SA 3.0 / GFDL 授權。來源：[Wikimedia Commons — BalticServers_data_center.jpg](https://commons.wikimedia.org/wiki/File:BalticServers_data_center.jpg)*

---

## 2. 電力化的完整弧線

這是本文主線，也是 GPT 從實驗室裡的好奇物，變成看不見的基礎設施，以及從發明到回報之間存在數十年滯後的最清楚案例。

### 2.1 發明與第一批中央電站（1879 到 1882）

- **1879**：Thomas Edison（美國）與 Joseph Swan（英國）各自展示實用、壽命夠長的**白熾燈泡**。燈泡是創造分散式用電需求的「killer app」。
- **1882 年 1 月 12 日**：Edison 位於倫敦的 **Holborn Viaduct** 電站開始運轉，這是世界第一座燃煤公共發電站。([Wikipedia: Holborn Viaduct power station](https://en.wikipedia.org/wiki/Holborn_Viaduct_power_station))
- **1882 年 9 月 4 日**：Edison 位於曼哈頓 Pearl Street 257 號的 **Pearl Street Station** 開始供電給「First District」的客戶。它是所有中央發電站的先驅，也是第一座*永久性*中央電站：直流、低電壓，服務半徑勉強一英里左右。([IEEE/ETHW: Milestones — Pearl Street Station, 1882](https://ethw.org/Milestones:Pearl_Street_Station,_1882), [Wikipedia: Pearl Street Station](https://en.wikipedia.org/wiki/Pearl_Street_Station))

![Edison 的 Pearl Street Station，紐約（1882）素描](https://upload.wikimedia.org/wikipedia/commons/5/58/PearlStreetStation.jpg)
*Pearl Street Station，第一座永久性中央電站（DC），1882。來源：[Wikimedia Commons — PearlStreetStation.jpg](https://commons.wikimedia.org/wiki/File:PearlStreetStation.jpg)*

### 2.2 電流戰爭與交流勝出（1880 年代到 1896）

Edison 押注**直流（DC）**。DC 不容易升壓到高電壓，因此輸電損失讓它的範圍被限制在約 1 英里，也就是幾乎每個街區都需要一座電廠。**George Westinghouse** 與 **Nikola Tesla** 支持**交流（AC）**，因為 AC 可以透過變壓器升壓做長距離輸電，再降壓供使用端使用。

- **1893**：Westinghouse 拿下 **Chicago World's Columbian Exposition** 的照明合約，以 AC 點亮會場，公開展示它的安全性與規模化能力。([History.com: War of the Currents](https://www.history.com/articles/what-was-the-war-of-the-currents))
- **1895 年 4 月 15 日**：**Niagara Falls**（Edward Dean Adams）水力發電廠的第一部大型發電機完成測試。
- **1896 年 11 月 16 日**：Niagara 開始把 AC 電力送到**約 26 英里外的 Buffalo, NY**。這是 DC 在物理上幾乎做不到的成就，也成為 AC 勝出的決定性證明。([Big Think: Tesla at Niagara](https://bigthink.com/surprising-science/why-nikola-teslas-greatest-achievement-may-be-in-niagara-falls/), [Legal Legacy: Nov 16, 1896](https://legallegacy.wordpress.com/2020/11/16/november-16-1896-niagara-falls-hydroelectric-power-plant-begins-operation/))

![Niagara Falls 的 Adams 水力發電廠](https://upload.wikimedia.org/wikipedia/commons/thumb/6/6f/AdamsPowerPlant_DateUnknown_HABS_15_GeneralViewFromSoutheast_cropped.jpg/640px-AdamsPowerPlant_DateUnknown_HABS_15_GeneralViewFromSoutheast_cropped.jpg)
*Niagara Falls 的 Edward Dean Adams Station：大規模 AC 水力發電，讓電流戰爭塵埃落定。來源：[Wikimedia Commons — Adams Power Plant](https://commons.wikimedia.org/wiki/File:AdamsPowerPlant_DateUnknown_HABS_15_GeneralViewFromSoutheast_cropped.jpg)*

AC + 變壓器 + 中央電站，就是我們今天仍在使用的電網架構。當你能便宜地遠距離輸電，發電的經濟邏輯就會從「每家工廠自己蓋引擎」翻轉成「向電力公司買電」。

### 2.3 工廠改造：從傳動軸到單機驅動

這是 Paul David 論點的核心，也是整個故事裡與工程師最相關的部分。

**舊作法（group drive / line-shaft）：** 一個原動機（水車或蒸汽機）帶動貫穿整棟建築的中央傳動軸；皮帶從頭頂的「line shafts」垂下來，驅動每一台機器。整棟建築的配置都被動力傳輸的機械結構決定：機器擠在傳動軸旁、皮帶到處都是、單點故障，而且想移動一台機器，就得重拉皮帶與傳動機構。

![傳動軸工廠：機器由頭頂傳動軸垂下的皮帶驅動（Leipzig，約 1925）](https://upload.wikimedia.org/wikipedia/commons/thumb/e/eb/AHW_Kammgarnspinnerei_Pfaffendorf_Leipzig_um_1925.jpg/640px-AHW_Kammgarnspinnerei_Pfaffendorf_Leipzig_um_1925.jpg)
*由頭頂傳動軸垂下的皮帶驅動的毛紡機器，也就是電力化後來取代的「group drive」架構。來源：[Wikimedia Commons — line-shaft spinning mill](https://commons.wikimedia.org/wiki/File:AHW_Kammgarnspinnerei_Pfaffendorf_Leipzig_um_1925.jpg)*

**第一波（失敗的）電力化：** 管理者只是把蒸汽機換成一台大型電動馬達，然後保留傳動軸與皮帶。這就是 David 強調的陷阱：*把新技術套在舊系統上。* 你得到比較乾淨一點的動力來源，但 productivity 幾乎沒有提升。([Paul David, "The Dynamo and the Computer," 1990](https://www.academia.edu/11211365/The_Dynamo_and_the_Computer_An_Historical_Perspective_on_the_Modern_Productivity_Paradox))

**真正的革命（unit drive）：** 在*每一台機器上裝一顆小馬達*。於是動力變成可分割、按需使用：閒置機器不耗電，沒有會讓整條線停擺的中央傳動軸，更關鍵的是，**廠房布局終於不再受傳動軸幾何限制。** 你可以依*製程順序*（也就是工作流）安排機器，裝設天車，建造採光良好的單層廠房，並加入電動物料搬運。productivity 來自這種重新設計，而不是馬達本身。

電力驅動的擴散情況（Warren Devine 的經典研究 *"From Shafts to Wires,"* 1983，以及其他來源佐證）：

- **1899：** 電動馬達提供的馬力占美國製造業已安裝機械驅動馬力的 **<5%**。
- **約 1914：** 約 **40%**。
- **約 1919：** 約 **55%**。
- **約 1929 到 1930：** 約 **78 到 80%**。

([Devine, "From Shafts to Wires," J. Econ. History (1983)](https://www.cambridge.org/core/journals/journal-of-economic-history/article/abs/from-shafts-to-wires-historical-perspective-on-electrification/500078D9B4764BA1109A7967437CF226); 工業占比數字也由 [Construction Physics, "The Birth of the Grid"](https://www.construction-physics.com/p/the-birth-of-the-grid) 佐證)

美國製造業 productivity 的大幅躍升出現在 **1920 年代**，大約是 Pearl Street 之後**四十年**，也就是 unit-drive 重新設計大規模普及之後。這四十年的落差，就是整個重點。

![Ford 的移動式裝配線，Highland Park，1913](https://upload.wikimedia.org/wikipedia/commons/thumb/e/e8/Ford_assembly_line_-_1913_%28restored%29.jpg/640px-Ford_assembly_line_-_1913_%28restored%29.jpg)
*Ford 的 Highland Park 移動式裝配線，始於 1913 年 10 月 7 日：這種依流程配置、由電力驅動的廠房，是 line-shaft 工廠不可能做到的。它把 Model T 底盤組裝時間從約 12.5 小時降到約 93 分鐘。來源：[Wikimedia Commons — Ford assembly line 1913](https://commons.wikimedia.org/wiki/File:Ford_assembly_line_-_1913_(restored).jpg)；組裝時間數字：[History.com](https://www.history.com/this-day-in-history/october-7/moving-assembly-line-at-ford), [Library of Congress](https://guides.loc.gov/this-month-in-business-history/October/Ford)*

![工業電動馬達，類似 unit drive 下用來驅動個別機器的設備](https://upload.wikimedia.org/wikipedia/commons/thumb/5/53/VEM_motor_Wernigerode.png/512px-VEM_motor_Wernigerode.png)
*工業電動馬達。每台機器各自配備的「unit drive」馬達，讓工廠配置擺脫中央傳動軸。來源：[Wikimedia Commons — VEM_motor_Wernigerode.png](https://commons.wikimedia.org/wiki/File:VEM_motor_Wernigerode.png)*

### 2.4 家庭與農村擴散（1899 到約 1960）

照明與工廠先到；*家庭*慢了一步，*農場*則慢得多。

- **約 1899 到 1907：** 家戶電力化比例從低個位數到約 **8%**。（常被引用的「1899 年約 3% 美國家庭有電」大致可信，也符合趨勢，但我**無法**把它追到單一權威一手來源；文獻比較扎實的錨點是 **1907 年美國家庭約 8% 有電**。）([Construction Physics](https://www.construction-physics.com/p/the-birth-of-the-grid))
- **約 1910：** 約 **10%** 美國家庭有電。([Construction Physics](https://www.construction-physics.com/p/the-birth-of-the-grid))
- **1920 年代初：** 約 **30 到 35%** 美國家庭。
- **約 1925：** 大約**一半**。
- **約 1929 到 1930：** 約 **68 到 70%**，但這個接近普及的數字主要是*城市*；美國農村大多仍然沒有電。([Coolidge Foundation: "A Misunderstood Decade"](https://coolidgefoundation.org/blog/a-misunderstood-decade/); [Smithsonian NMAH](https://www.americanhistory.si.edu/explore/stories/power-people-rural-electrification-brought-more-lights))
- **1934：** 只有約 **11%** 的美國*農場*有電。民營電力公司不願以負擔得起的價格，把電線拉到人口稀疏的鄉間。
- **1935/1936：** **Rural Electrification Administration**（1935 年以行政命令成立；**Rural Electrification Act** 於 **1936** 年通過）提供融資，讓農民持有的合作社興建農村電線。([Living New Deal: REA](https://livingnewdeal.org/glossary/rural-electrification-administration-rea-1935/); [Wikipedia: Rural Electrification Act](https://en.wikipedia.org/wiki/Rural_Electrification_Act))
- **1945：** 約 **50%** 農場有電；**1950：** 約 **80%**；**1960：** 約 **97%**，幾乎普及。([Richmond Fed: "Electrifying Rural America"](https://www.richmondfed.org/publications/research/econ_focus/2020/q1/economic_history))

所以整條弧線，從 Edison 的燈泡（1879）到美國電力化幾乎普及（約 1960），大約跨越 **80 年**。

### 2.5 為什麼花了約四十年才回收（David 的論點）

Paul David 對這段滯後的解釋，也可以推廣到每一種 GPT：

1. **關鍵是互補投資，不只是裝置本身。** 一顆馬達很便宜；圍繞它重新設計工廠並不便宜。價值在*系統*裡，而系統必須被重建。
2. **重組勝過替換。** 把馬達裝在原本蒸汽機的位置（替換）沒有什麼用；把整座工廠依製程順序重新配置（重組），才會讓每位工人的產出跳升。
3. **資本汰換很慢。** 你不會報廢一座還能運作的工廠。電力驅動配置主要是在舊廠磨損淘汰、*新廠*從零開始用電力化方式興建時擴散，而這需要一個世代。
4. **投入價格下降才會打開採用。** 實質電價大幅下跌（有估計認為 **1890 到 1920 年間實質下降超過 80%**），採用曲線也大致在這時轉折。([Construction Physics](https://www.construction-physics.com/p/the-birth-of-the-grid))
5. **技能與 know-how 也會滯後。** 工程師、電工與管理者都必須學會如何*為電力而設計*。這種人力資本本身就是緩慢的無形投資。

第 1 點與第 5 點，正是 Brynjolfsson 等人後來形式化為 productivity **J-curve** 成因的那些**無形資產**。([NBER w25148](https://www.nber.org/papers/w25148))

---

## 3. 各次革命中的共同模式

同樣的形狀反覆出現：

| GPT | 發明／首次部署 | 廣泛 productivity 回報 | 約略滯後 |
|---|---|---|---|
| **蒸汽** | Watt 分離式冷凝器，**1769** | 19 世紀中期的工廠 productivity | 約 50 到 80 年 |
| **電力** | Edison 燈泡 **1879** / Pearl Street **1882** | 美國製造業暴衝，**1920 年代** | 約 **40 年** |
| **計算** | ENIAC **1946** / 微處理器 **1971** | 美國 productivity 加速，**1990 年代中期到 2000 年代** | 數十年 |
| **AI**（被主張為 GPT） | 深度學習時代 **2010 年代** | TBD | TBD |

Paul David 1990 年的論文把這個類比講得很明確：1990 年的電腦，就像 1900 年的發電機，到處都看得到，唯獨統計裡看不到。Brynjolfsson, Rock & Syverson（2018）補上機制，也就是由被低估的無形／互補投資所驅動的 **productivity J-curve**；他們甚至估計，若調整軟體無形資產，美國 total-factor productivity（TFP，全要素生產力）在 2017 年底會比官方數字高約 **15.9%**。([NBER w25148](https://www.nber.org/papers/w25148))

給工程師的重點是：**當一個新的 GPT 看起來令人失望時，在判定技術被過度炒作之前，先懷疑它還在 J-curve 前段。** 滯後不代表技術沒有兌現價值；它代表周邊系統需要時間重建，包含組織圖、工作流程、技能、資本存量。電力不是在工廠被*接上電*的那一刻改造工廠，而是在工廠被重新*設計成適合電力*之後，才真正改造工廠。

---

## 摘要時間線

| 日期 | 事件 | 意義 |
|---|---|---|
| **1769** | Watt 取得分離式冷凝器專利 | 讓蒸汽在工廠中變得經濟可行 |
| **約 1760 到 1840** | 第一次工業革命 | 蒸汽、紡織、鐵、工廠系統 |
| **1850 年代** | Bessemer 製鋼法（取得專利） | 廉價大量鋼鐵 |
| **1870 到 1914** | 第二次工業革命 | **電力化**、鋼鐵、化學、ICE、電報／電話、大量生產 |
| **1879** | Edison 與 Swan 的白熾燈泡 | 電力的「killer app」 |
| **1882 年 1 月 12 日** | Holborn Viaduct 電站（倫敦） | 第一座燃煤公共發電站 |
| **1882 年 9 月 4 日** | Pearl Street Station（NYC） | 第一座*永久性*中央電站（DC） |
| **1893** | Chicago World's Fair 以 AC 點亮 | AC 的公開勝利 |
| **1895 到 1896** | Niagara Falls AC；1896 年 11 月 16 日送電 26 英里到 Buffalo | AC 決定性贏得電流戰爭 |
| **1899** | 電動馬達占工廠驅動馬力 <5% | 工業電力化才剛開始 |
| **1907** | 約 8% 美國家庭有電 | 家庭擴散滯後 |
| **1913** | Ford 移動式裝配線（10 月 7 日） | 大量生產；每個底盤 12.5 小時 → 93 分鐘 |
| **1920 年代** | 美國製造業 productivity 躍升 | 約 40 年後的電力化回報（unit drive） |
| **約 1929 到 1930** | 約 78 到 80% 工廠驅動已電力化；約 68 到 70%（城市）家庭有電 | 電力化成為主流 |
| **1935/1936** | Rural Electrification Administration / Act | 資助農村合作社 |
| **1946** | ENIAC 公開亮相（2 月 14 日） | 第一台通用電子電腦 |
| **約 1950 年代到 2000 年代** | 第三次／數位革命 | 半導體、電腦、網際網路 |
| **約 1960** | 約 97% 美國農場有電 | 電力化幾乎普及 |
| **1971** | Intel 4004 微處理器 | CPU on a chip |
| **1990** | Paul David, "The Dynamo and the Computer" | 點出滯後模式 |
| **2010 年代至今** | 「第四次工業革命」（Schwab/WEF）－*有爭議* | AI、IoT、cyber-physical systems |
| **2018** | Brynjolfsson et al., "Productivity J-Curve" | 形式化滯後機制 |

---

## 資料來源

- Paul A. David, *"The Dynamo and the Computer: An Historical Perspective on the Modern Productivity Paradox,"* American Economic Review 80(2), 1990：[AEA](https://www.aeaweb.org/articles?id=10.1257/aer.80.2.355) · [PDF](https://www.academia.edu/11211365/The_Dynamo_and_the_Computer_An_Historical_Perspective_on_the_Modern_Productivity_Paradox)
- Brynjolfsson, Rock & Syverson, *"The Productivity J-Curve,"* NBER w25148 (2018) / AEJ:Macro (2021)：[NBER](https://www.nber.org/papers/w25148) · [AEA](https://www.aeaweb.org/articles?id=10.1257%2Fmac.20180386)
- Warren D. Devine, *"From Shafts to Wires: Historical Perspective on Electrification,"* Journal of Economic History 43(2), 1983：[Cambridge Core](https://www.cambridge.org/core/journals/journal-of-economic-history/article/abs/from-shafts-to-wires-historical-perspective-on-electrification/500078D9B4764BA1109A7967437CF226)
- Joel Mokyr, *"The Second Industrial Revolution, 1870–1914"*：[PDF](https://faculty.wcas.northwestern.edu/jmokyr/castronovo.pdf)
- Wikipedia：[Industrial Revolution](https://en.wikipedia.org/wiki/Industrial_Revolution) · [Second Industrial Revolution](https://en.wikipedia.org/wiki/Second_Industrial_Revolution) · [Digital Revolution](https://en.wikipedia.org/wiki/Digital_Revolution) · [The Third Industrial Revolution (Rifkin)](https://en.wikipedia.org/wiki/The_Third_Industrial_Revolution) · [Pearl Street Station](https://en.wikipedia.org/wiki/Pearl_Street_Station) · [Holborn Viaduct power station](https://en.wikipedia.org/wiki/Holborn_Viaduct_power_station) · [War of the currents](https://en.wikipedia.org/wiki/War_of_the_currents) · [ENIAC](https://en.wikipedia.org/wiki/ENIAC) · [Rural Electrification Act](https://en.wikipedia.org/wiki/Rural_Electrification_Act)
- James Watt 分離式冷凝器，1769：[Science Museum](https://blog.sciencemuseum.org.uk/james-watt-and-the-separate-condenser/) · [Britannica](https://www.britannica.com/biography/James-Watt)
- 工業革命中的蒸汽機：[World History Encyclopedia](https://www.worldhistory.org/article/2166/the-steam-engine-in-the-british-industrial-revolut/)
- Bessemer／鋼鐵：[Lumen Learning](https://courses.lumenlearning.com/suny-hccc-worldhistory2/chapter/steel-production/)
- Pearl Street Station 里程碑：[IEEE/ETHW](https://ethw.org/Milestones:Pearl_Street_Station,_1882)
- 電流戰爭／Niagara：[History.com](https://www.history.com/articles/what-was-the-war-of-the-currents) · [Big Think](https://bigthink.com/surprising-science/why-nikola-teslas-greatest-achievement-may-be-in-niagara-falls/) · [Legal Legacy (Nov 16, 1896)](https://legallegacy.wordpress.com/2020/11/16/november-16-1896-niagara-falls-hydroelectric-power-plant-begins-operation/)
- Ford 移動式裝配線，1913：[History.com](https://www.history.com/this-day-in-history/october-7/moving-assembly-line-at-ford) · [Library of Congress](https://guides.loc.gov/this-month-in-business-history/October/Ford)
- 家庭與工業電力化數字：[Construction Physics, "The Birth of the Grid"](https://www.construction-physics.com/p/the-birth-of-the-grid) · [Coolidge Foundation](https://coolidgefoundation.org/blog/a-misunderstood-decade/)
- 農村電力化：[Smithsonian NMAH](https://www.americanhistory.si.edu/explore/stories/power-people-rural-electrification-brought-more-lights) · [Richmond Fed](https://www.richmondfed.org/publications/research/econ_focus/2020/q1/economic_history) · [Living New Deal](https://livingnewdeal.org/glossary/rural-electrification-administration-rea-1935/)
- 第四次工業革命（Schwab/WEF, 2016）：[WEF essay](https://www.weforum.org/stories/2016/01/the-fourth-industrial-revolution-what-it-means-and-how-to-respond/) · [WEF press release](https://www.weforum.org/press/2016/01/shaping-the-fourth-industrial-revolution-to-benefit-all-new-book-by-professor-schwab/)

*圖片檔案（皆來自 Wikimedia Commons；授權細節請點各圖片說明中的連結）：* Watt 蒸汽機、Bessemer 轉爐、Pearl Street Station、Adams/Niagara 發電廠、line-shaft 紡織廠、Ford 裝配線（1913）、工業電動馬達、ENIAC（CC BY-SA 3.0/GFDL）、BalticServers 資料中心（CC BY-SA 3.0/GFDL）。
