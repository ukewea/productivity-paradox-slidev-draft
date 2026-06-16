# The Industrial Revolutions, With Electrification as the Throughline

*A reference for engineers who like depth.* Every date and figure below was checked against primary or reputable secondary sources; inline links point to them, and a consolidated **Sources** list sits at the bottom. Where a popular figure is fuzzy or contested, it is flagged explicitly.

The reason this is worth your time as a software engineer: the single most useful pattern in the history of technology is that **a general-purpose technology (GPT) is invented decades before it shows up in the productivity statistics.** It happened with the steam engine, it happened *spectacularly* with electricity, it happened with the computer, and it is — arguably — happening right now with AI. The electrification story is the cleanest case study we have, so it runs as a throughline through the whole article.

---

## 0. The mental model: general-purpose technologies and the lag

A *general-purpose technology* is one that (a) spreads across the whole economy, (b) keeps improving, and (c) spawns complementary innovations. Steam, electricity, the internal-combustion engine, the computer, and (plausibly) AI all qualify.

The recurring twist is the **lag**. You install the new thing, and for a long time output per hour barely moves — sometimes it falls. Then, often decades later, productivity takes off. The two canonical references for this idea:

- **Paul David (1990)**, *"The Dynamo and the Computer: An Historical Perspective on the Modern Productivity Paradox"*, used electrification to explain why 1980s computers were, in Robert Solow's quip, visible "everywhere but in the productivity statistics." ([American Economic Review / AEA](https://www.aeaweb.org/articles?id=10.1257/aer.80.2.355), [PDF via academia.edu](https://www.academia.edu/11211365/The_Dynamo_and_the_Computer_An_Historical_Perspective_on_the_Modern_Productivity_Paradox))
- **Brynjolfsson, Rock & Syverson (2018/2021)**, *"The Productivity J-Curve: How Intangibles Complement General Purpose Technologies"*, formalized why: a new GPT requires large, hard-to-measure **intangible** investments (process redesign, new business models, human capital). Early on, output and productivity are *under*-measured (you're paying to build intangibles nobody counts); later, when those intangibles pay off, productivity appears to surge. The curve dips before it rises — a "J." ([NBER w25148](https://www.nber.org/papers/w25148), [AEA AEJ:Macro](https://www.aeaweb.org/articles?id=10.1257%2Fmac.20180386))

Keep this in your head. Everything below is an instance of it.

---

## 1. The standard periodization

Historians and economists conventionally split industrialization into three-to-four "revolutions." The boundaries are soft and the labels (especially the fourth) are debated, but the scaffolding is widely shared.

### First Industrial Revolution (~**1760**–**1840**)

> **GPT: the steam engine.** Also: water power, mechanized textiles, iron, and — the real institutional invention — the factory system.

**Cause → effect.** Britain had cheap coal, expensive labor, deep capital markets, and a patent system. That combination made it worth mechanizing. The breakthrough device was James Watt's **separate condenser**, patented **5 January 1769** under the title *"A New Method of Lessening the Consumption of Steam and Fuel in Fire-Engines."* It cut the Newcomen engine's coal consumption by roughly two-thirds, which is what finally made steam economical away from coalfields and inside factories rather than just pumping water out of mines. ([Science Museum](https://blog.sciencemuseum.org.uk/james-watt-and-the-separate-condenser/), [Britannica: James Watt](https://www.britannica.com/biography/James-Watt))

**Who / what / where.** Britain, c. 1760 onward, spreading to continental Europe and the US by ~1840. ([Wikipedia: Industrial Revolution](https://en.wikipedia.org/wiki/Industrial_Revolution))

**Concrete examples.**
- **Textiles:** Hargreaves' spinning jenny (~1764), Arkwright's water frame, Crompton's mule, Cartwright's power loom — spinning and then weaving go from cottage handcraft to machine work. ([World History Encyclopedia: Steam Engine in the IR](https://www.worldhistory.org/article/2166/the-steam-engine-in-the-british-industrial-revolut/))
- **Iron:** coke smelting and puddling scale up cheap iron for machines, rails, and structures.
- **The factory itself:** the genuinely new "technology" is organizational — concentrating workers and machines around a single prime mover (a waterwheel, then a steam engine).

![A late Watt double-acting beam steam engine (D. Napier & Son, London, 1832), preserved at the Higher Technical School of Industrial Engineers, Madrid](https://upload.wikimedia.org/wikipedia/commons/thumb/9/9e/Maquina_vapor_Watt_ETSIIM.jpg/640px-Maquina_vapor_Watt_ETSIIM.jpg)
*A preserved Watt-type double-acting steam engine. Source: [Wikimedia Commons — Maquina_vapor_Watt_ETSIIM.jpg](https://commons.wikimedia.org/wiki/File:Maquina_vapor_Watt_ETSIIM.jpg)*

Note the architecture of power here: **one big engine** turns shafts and belts that drive *everything*. Hold that thought — electrification's biggest payoff was tearing this exact arrangement out.

### Second Industrial Revolution (~**1870**–**1914**)

> **GPT: ELECTRIFICATION.** This is the centerpiece. Surrounding it: cheap steel (Bessemer/open-hearth), industrial chemicals, the internal-combustion engine, the telegraph/telephone, and mass production.

**Cause → effect.** A cluster of science-driven technologies arrived close together and reinforced each other. Cheap steel made bigger machines, rails, and buildings possible; electricity gave a clean, divisible, transmittable form of power; the telegraph and telephone collapsed communication time; interchangeable parts plus the moving line gave mass production. The dating is conventionally **1870–1914** (ending at WWI). ([Wikipedia: Second Industrial Revolution](https://en.wikipedia.org/wiki/Second_Industrial_Revolution), [Joel Mokyr, "The Second Industrial Revolution, 1870–1914"](https://faculty.wcas.northwestern.edu/jmokyr/castronovo.pdf))

**Why electricity is the centerpiece.** It is the textbook GPT of this era: a single underlying technology (generation + transmission + the electric motor) that re-tooled lighting, factories, transit, communication, and eventually the home. Its full arc gets its own section below.

**Concrete examples.**
- **Steel:** Henry Bessemer's converter (patented in the 1850s) blew air through molten pig iron to burn off carbon, collapsing the cost of steel and letting it replace wrought iron in rails, bridges, ships, and skyscrapers. ([Lumen: Steel Production](https://courses.lumenlearning.com/suny-hccc-worldhistory2/chapter/steel-production/))
- **Mass production:** Ford's moving assembly line (1913, below) is the iconic instance.
- **Communication / chemicals / ICE:** the telephone (Bell, 1876), synthetic dyes and fertilizers, and the internal-combustion engine all mature in this window.

![Schematic of a Bessemer converter, the device that made cheap bulk steel](https://upload.wikimedia.org/wikipedia/commons/thumb/6/61/Bessemer_converter.jpg/512px-Bessemer_converter.jpg)
*A Bessemer converter. Source: [Wikimedia Commons — Bessemer_converter.jpg](https://commons.wikimedia.org/wiki/File:Bessemer_converter.jpg)*

### Third Industrial Revolution / Digital Revolution (~**1950s**–**2000s**)

> **GPT: the semiconductor / digital logic** (transistor → integrated circuit → microprocessor), giving rise to the computer and the internet.

**Cause → effect.** The shift from mechanical and analog electronics to **digital** electronics: the MOSFET, the integrated circuit, the microprocessor, and packet-switched networking. This is the era when information becomes the thing you process and move at near-zero marginal cost. ([Wikipedia: Digital Revolution](https://en.wikipedia.org/wiki/Digital_Revolution); the "Third Industrial Revolution" label is also associated with Jeremy Rifkin's 2011 book — [Wikipedia](https://en.wikipedia.org/wiki/The_Third_Industrial_Revolution))

**Who / what / where.** US/global; Bell Labs, Fairchild/Intel in Silicon Valley, ARPANET → the Internet, the PC, and eventually the Web.

**Concrete examples.**
- **ENIAC** (Moore School, University of Pennsylvania) — the first general-purpose electronic digital computer, publicly unveiled **14 February 1946**. ([Penn Engineering](https://www.seas.upenn.edu/about/history-heritage/eniac/), [Wikipedia: ENIAC](https://en.wikipedia.org/wiki/ENIAC))
- **The microprocessor** (Intel 4004, 1971) puts a CPU on one chip.
- **The Internet / Web** — ARPANET (1969) to TCP/IP (1983) to the World Wide Web (1989–91).

![ENIAC panels and a function table at the Moore School, University of Pennsylvania](https://upload.wikimedia.org/wikipedia/commons/thumb/6/6c/ENIAC_Penn1.jpg/640px-ENIAC_Penn1.jpg)
*ENIAC, the first general-purpose electronic digital computer. Photo © Paul W. Shaffer, University of Pennsylvania, licensed CC BY-SA 3.0 / GFDL. Source: [Wikimedia Commons — ENIAC_Penn1.jpg](https://commons.wikimedia.org/wiki/File:ENIAC_Penn1.jpg)*

### Fourth Industrial Revolution / "Industry 4.0" (~**2010s**–) — *contested*

> **Claimed GPT(s): cyber-physical systems, AI, IoT, robotics**, fusing physical, digital, and biological domains.

**Origin of the label.** "The Fourth Industrial Revolution" was popularized by **Klaus Schwab**, founder of the World Economic Forum, in a January 2016 book and as the theme of that year's Davos meeting. ("Industrie 4.0" originated slightly earlier as a German manufacturing-strategy term.) Schwab's claim is that the changes differ from the Third in *scale, scope, and complexity*. ([WEF: "The Fourth Industrial Revolution: what it means" (2016)](https://www.weforum.org/stories/2016/01/the-fourth-industrial-revolution-what-it-means-and-how-to-respond/), [WEF press release, Jan 2016](https://www.weforum.org/press/2016/01/shaping-the-fourth-industrial-revolution-to-benefit-all-new-book-by-professor-schwab/))

**Why it's contested.** Plenty of economists and historians argue this is *not* a distinct revolution but a continuation of the digital one — the same GPT (digital computing/semiconductors) maturing, not a new general-purpose technology. The "4IR" framing is a WEF/Schwab coinage popular in policy and consulting circles, and you should treat it as a *branding* claim as much as a historical one. Flag it as such when you cite it.

**Concrete examples (whatever you call the era).** Deep learning and large language models; cloud-scale data centers; industrial IoT and "smart factories"; autonomous systems and robotics.

![Server racks in the BalticServers data center](https://upload.wikimedia.org/wikipedia/commons/5/5d/BalticServers_data_center.jpg)
*A modern data center — the power-hungry "factory floor" of the digital/AI era. Photo licensed CC BY-SA 3.0 / GFDL. Source: [Wikimedia Commons — BalticServers_data_center.jpg](https://commons.wikimedia.org/wiki/File:BalticServers_data_center.jpg)*

---

## 2. The complete arc of electrification

This is the throughline — the cleanest example of a GPT going from lab curiosity to invisible infrastructure, and of the multi-decade lag between invention and payoff.

### 2.1 Invention and the first central stations (1879–1882)

- **1879** — Thomas Edison (US) and Joseph Swan (UK) independently demonstrate practical, long-lived **incandescent lamps**. The lamp is the "killer app" that creates demand for distributed electricity.
- **12 January 1882** — Edison's **Holborn Viaduct** station in London begins running: the world's first coal-fired public power station. ([Wikipedia: Holborn Viaduct power station](https://en.wikipedia.org/wiki/Holborn_Viaduct_power_station))
- **4 September 1882** — Edison's **Pearl Street Station** at 257 Pearl Street, Manhattan begins supplying customers in the "First District." It is the forerunner of all central generating stations and the first *permanent* one — DC, low voltage, serving a radius of barely a mile. ([IEEE/ETHW: Milestones — Pearl Street Station, 1882](https://ethw.org/Milestones:Pearl_Street_Station,_1882), [Wikipedia: Pearl Street Station](https://en.wikipedia.org/wiki/Pearl_Street_Station))

![Sketch of Edison's Pearl Street Station, New York (1882)](https://upload.wikimedia.org/wikipedia/commons/5/58/PearlStreetStation.jpg)
*Pearl Street Station, the first permanent central power station (DC), 1882. Source: [Wikimedia Commons — PearlStreetStation.jpg](https://commons.wikimedia.org/wiki/File:PearlStreetStation.jpg)*

### 2.2 The War of the Currents and the triumph of AC (1880s–1896)

Edison bet on **direct current (DC)**. DC can't be easily stepped up to high voltage, so transmission losses limited it to ~1 mile — meaning a power plant on nearly every block. **George Westinghouse** and **Nikola Tesla** backed **alternating current (AC)**, which transformers can step up for long-distance transmission and back down for use.

- **1893** — Westinghouse wins the contract to light the **Chicago World's Columbian Exposition** with AC, a very public demonstration of its safety and scale. ([History.com: War of the Currents](https://www.history.com/articles/what-was-the-war-of-the-currents))
- **15 April 1895** — the first large generator at the **Niagara Falls** (Edward Dean Adams) hydroelectric plant is tested.
- **16 November 1896** — Niagara begins transmitting AC power **~26 miles to Buffalo, NY** — a feat physically impossible for DC, and the decisive proof that AC had won. ([Big Think: Tesla at Niagara](https://bigthink.com/surprising-science/why-nikola-teslas-greatest-achievement-may-be-in-niagara-falls/), [Legal Legacy: Nov 16, 1896](https://legallegacy.wordpress.com/2020/11/16/november-16-1896-niagara-falls-hydroelectric-power-plant-begins-operation/))

![The Adams hydroelectric power plant at Niagara Falls](https://upload.wikimedia.org/wikipedia/commons/thumb/6/6f/AdamsPowerPlant_DateUnknown_HABS_15_GeneralViewFromSoutheast_cropped.jpg/640px-AdamsPowerPlant_DateUnknown_HABS_15_GeneralViewFromSoutheast_cropped.jpg)
*The Edward Dean Adams Station at Niagara Falls — large-scale AC hydroelectric generation that settled the War of the Currents. Source: [Wikimedia Commons — Adams Power Plant](https://commons.wikimedia.org/wiki/File:AdamsPowerPlant_DateUnknown_HABS_15_GeneralViewFromSoutheast_cropped.jpg)*

AC + transformers + central stations is the architecture of the grid we still use. Once you can transmit power cheaply over distance, the economics of generation flip from "every factory builds its own engine" to "buy power from a utility."

### 2.3 The factory transformation: from line shafts to unit drive

This is the heart of Paul David's argument and the most engineer-relevant part of the story.

**The old way (group drive / line-shaft):** one prime mover (waterwheel or steam engine) spins a central shaft running the length of the building; leather belts drop from overhead "line shafts" to each machine. The whole building's layout is dictated by the mechanics of power transmission — machines crammed near the shaft, belts everywhere, a single point of failure, and you can't move a machine without re-rigging the belts.

![Line-shaft factory: machines driven by belts from an overhead shaft (Leipzig, ~1925)](https://upload.wikimedia.org/wikipedia/commons/thumb/e/eb/AHW_Kammgarnspinnerei_Pfaffendorf_Leipzig_um_1925.jpg/640px-AHW_Kammgarnspinnerei_Pfaffendorf_Leipzig_um_1925.jpg)
*Wool-spinning machines driven by belts from an overhead line shaft — the "group drive" architecture electrification eventually replaced. Source: [Wikimedia Commons — line-shaft spinning mill](https://commons.wikimedia.org/wiki/File:AHW_Kammgarnspinnerei_Pfaffendorf_Leipzig_um_1925.jpg)*

**The first (failed) wave of electrification:** managers simply swapped the steam engine for one big electric motor and kept the shafts and belts. This is the trap David emphasizes — *overlaying a new technology on an old system.* You get a marginally cleaner power source and almost no productivity gain. ([Paul David, "The Dynamo and the Computer," 1990](https://www.academia.edu/11211365/The_Dynamo_and_the_Computer_An_Historical_Perspective_on_the_Modern_Productivity_Paradox))

**The real revolution (unit drive):** put a *small motor on each machine.* Now power is divisible and on-demand — idle machines draw nothing, there's no central shaft to fail, and crucially **the factory floor is freed from the geometry of the shaft.** You can lay machines out in *process order* (i.e., the flow of the work), put in overhead cranes, build single-story plants with natural light, and add electric materials handling. That redesign — not the motor itself — is where the productivity came from.

The diffusion of electric drive (Warren Devine's classic study, *"From Shafts to Wires,"* 1983, and corroborating sources):

- **1899:** electric motors supplied **<5%** of installed mechanical drive horsepower in US manufacturing.
- **~1914:** roughly **40%**.
- **~1919:** roughly **55%**.
- **~1929–1930:** roughly **78–80%**.

([Devine, "From Shafts to Wires," J. Econ. History (1983)](https://www.cambridge.org/core/journals/journal-of-economic-history/article/abs/from-shafts-to-wires-historical-perspective-on-electrification/500078D9B4764BA1109A7967437CF226); industrial-share figures corroborated by [Construction Physics, "The Birth of the Grid"](https://www.construction-physics.com/p/the-birth-of-the-grid))

The big US manufacturing-productivity surge shows up in the **1920s** — roughly **four decades after** Pearl Street — once the unit-drive redesign was widespread. That four-decade gap is the whole point.

![Ford's moving assembly line, Highland Park, 1913](https://upload.wikimedia.org/wikipedia/commons/thumb/e/e8/Ford_assembly_line_-_1913_%28restored%29.jpg/640px-Ford_assembly_line_-_1913_%28restored%29.jpg)
*Ford's Highland Park moving assembly line, begun 7 October 1913 — the kind of flow-based, electrically powered plant layout that line-shaft factories could never achieve. It cut Model T chassis assembly from ~12.5 hours to ~93 minutes. Source: [Wikimedia Commons — Ford assembly line 1913](https://commons.wikimedia.org/wiki/File:Ford_assembly_line_-_1913_(restored).jpg); assembly-time figures: [History.com](https://www.history.com/this-day-in-history/october-7/moving-assembly-line-at-ford), [Library of Congress](https://guides.loc.gov/this-month-in-business-history/October/Ford)*

![An industrial electric motor of the kind that powered individual machines under "unit drive"](https://upload.wikimedia.org/wikipedia/commons/thumb/5/53/VEM_motor_Wernigerode.png/512px-VEM_motor_Wernigerode.png)
*An industrial electric motor. Per-machine "unit drive" motors freed factory layout from the central line shaft. Source: [Wikimedia Commons — VEM_motor_Wernigerode.png](https://commons.wikimedia.org/wiki/File:VEM_motor_Wernigerode.png)*

### 2.4 Household and rural diffusion (1899 → ~1960)

Lighting and factories came first; the *home* lagged, and the *farm* lagged much more.

- **~1899–1907:** household electrification is in the low single digits to ~**8%**. (The frequently quoted "~3% of US homes in 1899" is plausible and consistent with the trend, but I could **not** pin it to a single authoritative primary source; the well-documented anchor is **~8% of US homes by 1907**.) ([Construction Physics](https://www.construction-physics.com/p/the-birth-of-the-grid))
- **~1910:** roughly **10%** of US homes. ([Construction Physics](https://www.construction-physics.com/p/the-birth-of-the-grid))
- **Early 1920s:** ~**30–35%** of US households.
- **~1925:** about **half**.
- **~1929–1930:** roughly **68–70%** — but this near-universal figure was *urban*; rural America was still mostly dark. ([Coolidge Foundation: "A Misunderstood Decade"](https://coolidgefoundation.org/blog/a-misunderstood-decade/); [Smithsonian NMAH](https://www.americanhistory.si.edu/explore/stories/power-people-rural-electrification-brought-more-lights))
- **1934:** only **~11%** of US *farms* had electricity. Private utilities wouldn't string lines across sparse countryside at affordable rates.
- **1935/1936:** the **Rural Electrification Administration** (created by executive order **1935**; the **Rural Electrification Act** passed **1936**) financed farmer-owned cooperatives to build rural lines. ([Living New Deal: REA](https://livingnewdeal.org/glossary/rural-electrification-administration-rea-1935/); [Wikipedia: Rural Electrification Act](https://en.wikipedia.org/wiki/Rural_Electrification_Act))
- **1945:** ~**50%** of farms; **1950:** ~**80%**; **1960:** ~**97%** — near-universal. ([Richmond Fed: "Electrifying Rural America"](https://www.richmondfed.org/publications/research/econ_focus/2020/q1/economic_history))

So the full arc — from Edison's lamp (1879) to near-universal US electrification (~1960) — spans about **80 years**.

### 2.5 Why it took ~four decades to pay off (the David thesis)

Paul David's explanation for the lag, which generalizes to every GPT:

1. **Complementary investment, not just the device.** A motor is cheap; redesigning the factory around it is not. The value is in the *system*, and the system has to be rebuilt.
2. **Reorganization beats substitution.** Bolting a motor where the steam engine used to be (substitution) does nothing; re-laying the whole plant in process order (reorganization) is where output per worker jumps.
3. **Capital replacement is slow.** You don't scrap a working factory. Electric-drive layouts spread mostly as old plants wore out and *new* ones were built electrified from scratch — which takes a generation.
4. **Falling input prices unlock adoption.** Real electricity prices fell sharply (one estimate: **>80% in real terms, 1890–1920**), and that's roughly when adoption inflected. ([Construction Physics](https://www.construction-physics.com/p/the-birth-of-the-grid))
5. **Skills and know-how lag.** Engineers, electricians, and managers had to learn how to design *for* electricity. That human capital is itself a slow, intangible investment.

Points 1 and 5 are exactly the **intangibles** Brynjolfsson et al. later formalized as the cause of the productivity **J-curve**. ([NBER w25148](https://www.nber.org/papers/w25148))

---

## 3. The pattern across revolutions

The same shape recurs:

| GPT | Invention / first deployment | Broad productivity payoff | Approx. lag |
|---|---|---|---|
| **Steam** | Watt separate condenser, **1769** | mid-19th-century factory productivity | ~50–80 yrs |
| **Electricity** | Edison lamp **1879** / Pearl Street **1882** | US manufacturing surge, **1920s** | ~**40 yrs** |
| **Computing** | ENIAC **1946** / microprocessor **1971** | US productivity acceleration, **mid-1990s–2000s** | decades |
| **AI** (claimed) | deep-learning era **2010s** | TBD | TBD |

Paul David's 1990 paper made the analogy explicit: in 1990, computers were the dynamo of 1900 — everywhere except in the statistics. Brynjolfsson, Rock & Syverson (2018) supplied the mechanism — the **productivity J-curve**, driven by under-measured intangible/complementary investment — and even estimated that adjusting for software intangibles, US total-factor productivity was about **15.9% higher** than the official measure at the end of 2017. ([NBER w25148](https://www.nber.org/papers/w25148))

The engineer's takeaway: **when a new GPT seems disappointing, suspect the J-curve before you conclude the technology is overhyped.** The lag is not the technology failing to deliver; it's the time it takes to rebuild the surrounding system — the org charts, the workflows, the skills, the capital stock — around it. Electricity didn't transform the factory until factories were *redesigned* for it, not merely *connected* to it.

---

## Summary timeline

| Date | Event | Significance |
|---|---|---|
| **1769** | Watt patents the separate condenser | Makes steam economical for factories |
| **~1760–1840** | First Industrial Revolution | Steam, textiles, iron, the factory system |
| **1850s** | Bessemer process (patented) | Cheap bulk steel |
| **1870–1914** | Second Industrial Revolution | **Electrification**, steel, chemicals, ICE, telegraph/telephone, mass production |
| **1879** | Edison & Swan incandescent lamps | The "killer app" for electricity |
| **12 Jan 1882** | Holborn Viaduct station (London) | First coal-fired public power station |
| **4 Sep 1882** | Pearl Street Station (NYC) | First *permanent* central station (DC) |
| **1893** | Chicago World's Fair lit with AC | Public win for AC |
| **1895–1896** | Niagara Falls AC; 26 mi to Buffalo (Nov 16, 1896) | AC decisively wins the War of the Currents |
| **1899** | Electric motors <5% of factory drive HP | Electrification barely begun in industry |
| **1907** | ~8% of US homes electrified | Household lag |
| **1913** | Ford moving assembly line (Oct 7) | Mass production; 12.5 hr → 93 min per chassis |
| **1920s** | US manufacturing productivity surge | The ~40-yr electrification payoff (unit drive) |
| **~1929–30** | ~78–80% of factory drive electric; ~68–70% of (urban) homes | Electrification mainstream |
| **1935/1936** | Rural Electrification Administration / Act | Finances rural co-ops |
| **1946** | ENIAC unveiled (Feb 14) | First general-purpose electronic computer |
| **~1950s–2000s** | Third / Digital Revolution | Semiconductors, computers, internet |
| **~1960** | ~97% of US farms electrified | Electrification near-universal |
| **1971** | Intel 4004 microprocessor | CPU on a chip |
| **1990** | Paul David, "The Dynamo and the Computer" | Names the lag pattern |
| **2010s–** | "Fourth Industrial Revolution" (Schwab/WEF) — *contested* | AI, IoT, cyber-physical systems |
| **2018** | Brynjolfsson et al., "Productivity J-Curve" | Formalizes the lag mechanism |

---

## Sources

- Paul A. David, *"The Dynamo and the Computer: An Historical Perspective on the Modern Productivity Paradox,"* American Economic Review 80(2), 1990 — [AEA](https://www.aeaweb.org/articles?id=10.1257/aer.80.2.355) · [PDF](https://www.academia.edu/11211365/The_Dynamo_and_the_Computer_An_Historical_Perspective_on_the_Modern_Productivity_Paradox)
- Brynjolfsson, Rock & Syverson, *"The Productivity J-Curve,"* NBER w25148 (2018) / AEJ:Macro (2021) — [NBER](https://www.nber.org/papers/w25148) · [AEA](https://www.aeaweb.org/articles?id=10.1257%2Fmac.20180386)
- Warren D. Devine, *"From Shafts to Wires: Historical Perspective on Electrification,"* Journal of Economic History 43(2), 1983 — [Cambridge Core](https://www.cambridge.org/core/journals/journal-of-economic-history/article/abs/from-shafts-to-wires-historical-perspective-on-electrification/500078D9B4764BA1109A7967437CF226)
- Joel Mokyr, *"The Second Industrial Revolution, 1870–1914"* — [PDF](https://faculty.wcas.northwestern.edu/jmokyr/castronovo.pdf)
- Wikipedia: [Industrial Revolution](https://en.wikipedia.org/wiki/Industrial_Revolution) · [Second Industrial Revolution](https://en.wikipedia.org/wiki/Second_Industrial_Revolution) · [Digital Revolution](https://en.wikipedia.org/wiki/Digital_Revolution) · [The Third Industrial Revolution (Rifkin)](https://en.wikipedia.org/wiki/The_Third_Industrial_Revolution) · [Pearl Street Station](https://en.wikipedia.org/wiki/Pearl_Street_Station) · [Holborn Viaduct power station](https://en.wikipedia.org/wiki/Holborn_Viaduct_power_station) · [War of the currents](https://en.wikipedia.org/wiki/War_of_the_currents) · [ENIAC](https://en.wikipedia.org/wiki/ENIAC) · [Rural Electrification Act](https://en.wikipedia.org/wiki/Rural_Electrification_Act)
- James Watt separate condenser, 1769 — [Science Museum](https://blog.sciencemuseum.org.uk/james-watt-and-the-separate-condenser/) · [Britannica](https://www.britannica.com/biography/James-Watt)
- Steam engine in the Industrial Revolution — [World History Encyclopedia](https://www.worldhistory.org/article/2166/the-steam-engine-in-the-british-industrial-revolut/)
- Bessemer / steel — [Lumen Learning](https://courses.lumenlearning.com/suny-hccc-worldhistory2/chapter/steel-production/)
- Pearl Street Station milestone — [IEEE/ETHW](https://ethw.org/Milestones:Pearl_Street_Station,_1882)
- War of the Currents / Niagara — [History.com](https://www.history.com/articles/what-was-the-war-of-the-currents) · [Big Think](https://bigthink.com/surprising-science/why-nikola-teslas-greatest-achievement-may-be-in-niagara-falls/) · [Legal Legacy (Nov 16, 1896)](https://legallegacy.wordpress.com/2020/11/16/november-16-1896-niagara-falls-hydroelectric-power-plant-begins-operation/)
- Ford moving assembly line, 1913 — [History.com](https://www.history.com/this-day-in-history/october-7/moving-assembly-line-at-ford) · [Library of Congress](https://guides.loc.gov/this-month-in-business-history/October/Ford)
- Household & industrial electrification figures — [Construction Physics, "The Birth of the Grid"](https://www.construction-physics.com/p/the-birth-of-the-grid) · [Coolidge Foundation](https://coolidgefoundation.org/blog/a-misunderstood-decade/)
- Rural electrification — [Smithsonian NMAH](https://www.americanhistory.si.edu/explore/stories/power-people-rural-electrification-brought-more-lights) · [Richmond Fed](https://www.richmondfed.org/publications/research/econ_focus/2020/q1/economic_history) · [Living New Deal](https://livingnewdeal.org/glossary/rural-electrification-administration-rea-1935/)
- Fourth Industrial Revolution (Schwab/WEF, 2016) — [WEF essay](https://www.weforum.org/stories/2016/01/the-fourth-industrial-revolution-what-it-means-and-how-to-respond/) · [WEF press release](https://www.weforum.org/press/2016/01/shaping-the-fourth-industrial-revolution-to-benefit-all-new-book-by-professor-schwab/)

*Image files (all from Wikimedia Commons; click each caption link for license details):* Watt engine, Bessemer converter, Pearl Street Station, Adams/Niagara plant, line-shaft mill, Ford assembly line (1913), industrial electric motor, ENIAC (CC BY-SA 3.0/GFDL), BalticServers data center (CC BY-SA 3.0/GFDL).
