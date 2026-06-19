# Early Manufacturing TFP Growth Was Not Necessarily Electrification

This note stores the evidence behind the Q&A answer for the visible `1879-1889` TFP bar in the deck.

The short version:

> The chart does not say there was no manufacturing productivity growth before the 1920s. There clearly was. The safer claim is narrower: the `1879-1889` manufacturing TFP growth should not be read as the factory-electrification payoff, because electric drive was essentially absent from U.S. manufacturing at that time.

## What The TFP Data Show

David 1989 Table 2 reports Kendrick-based U.S. manufacturing TFP growth rates. The deck uses the geometric-weighted Kendrick-based series:

| Period | Manufacturing TFP growth, %/yr |
|---|---:|
| 1869-1879 | 0.31 |
| 1879-1889 | 1.23 |
| 1889-1899 | 0.86 |
| 1899-1909 | 0.50 |
| 1909-1919 | 0.17 |
| 1919-1929 | 5.29 |

So yes: the 1880s bar is visibly higher than the 1870s, 1890s, 1900s, and 1910s.

## Why It Should Not Be Attributed To Factory Electrification

David 1989 Table 3 says factory electrification was still tiny:

| Year | Factory drive electrified | Secondary motor penetration |
|---:|---:|---:|
| 1889 | 0.3% | 0.3% |
| 1899 | 4.8% | 3.0% |
| 1919 | 53.1% | 32.6% |
| 1929 | 78.4% | 56.4% |

This makes the attribution problem straightforward: if factory electric drive was only around `0.3%` in 1889, the `1879-1889` manufacturing TFP growth cannot plausibly be explained mainly by electrification of factory motive power.

Field's Gilded Age paper makes this point directly. He argues that pre-World War I TFP growth was robust, but that much of it fits the broader Gilded Age story: railroads, telegraphs, modern business enterprise, scale, distribution, steel, petroleum refining, meatpacking, cigarettes, and other organizational or steam-era improvements. He also says it is unlikely that much prewar TFP growth can be attributed to industrial electrification, at least for motive power.

## Safer Explanation For The 1880s Bar

Treat the `1879-1889` bar as a reminder that manufacturing productivity had other sources:

- railroad and telegraph networks lowered coordination costs;
- modern business enterprise spread into railroads, telegraphs, distribution, and parts of manufacturing;
- scale-intensive sectors such as steel, petroleum refining, meatpacking, and cigarettes expanded;
- steam-era machinery and business organization continued improving;
- the Second Industrial Revolution was a cluster, not a single technology.

The Q&A phrasing:

> 1879-1889 也有 TFP growth, 這點完全沒錯。但那時候工廠電氣化幾乎還沒進場, 1889 年 factory drive electrified 只有約 0.3%。所以那根 bar 比較像 Gilded Age 其他力量的結果:鐵路、電報、現代企業組織、規模化、鋼鐵、石油、肉品加工等。它提醒我們不要把所有 productivity growth 都塞給電氣化。

## Sources

- Paul A. David, "Computer and Dynamo: The Modern Productivity Paradox in a Not-Too-Distant Mirror," Warwick Economic Research Paper No. 339, 1989, Tables 2 and 3. <https://warwick.ac.uk/fac/soc/economics/research/workingpapers/1989-1994/twerp339.pdf>
- Alexander J. Field, "US Economic Growth in the Gilded Age," 2007 draft. <https://eml.berkeley.edu/~webfac/eichengreen/e211_fa06/field_GildedAge.pdf>
- Data used in this repo: `data/manufacturing-tfp-david1989.csv` and `data/electrification-diffusion.csv`.
