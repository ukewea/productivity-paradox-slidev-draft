# Source Notes And Caveats

## Core Sources

- Paul A. David, "The Dynamo and the Computer: An Historical Perspective on the Modern Productivity Paradox," *AEA Papers and Proceedings*, 1990. Local PDF: `/Users/eanu/Downloads/1990-david.pdf`.
- Paul A. David, "Computer and Dynamo: The Modern Productivity Paradox in a Not-Too-Distant Mirror," 1989 working paper. Public PDF: <https://warwick.ac.uk/fac/soc/economics/research/workingpapers/1989-1994/twerp339.pdf>
- Warren D. Devine Jr., "From Shafts to Wires: Historical Perspective on Electrification," *Journal of Economic History*, 1983.
- Martin N. Baily and Robert J. Gordon, "The Productivity Slowdown, Measurement Issues, and the Explosion of Computer Power," *Brookings Papers on Economic Activity*, 1988.
- Stephen D. Oliner and Daniel E. Sichel, "The Resurgence of Growth in the Late 1990s: Is Information Technology the Story?", *Journal of Economic Perspectives*, 2000. <https://www.aeaweb.org/articles?id=10.1257/jep.14.4.3>
- Dale W. Jorgenson, Mun S. Ho, and Kevin J. Stiroh, "A Retrospective Look at the U.S. Productivity Growth Resurgence," *Journal of Economic Perspectives*, 2008. <https://www.aeaweb.org/articles?id=10.1257/jep.22.1.3>
- Chad Syverson, "Challenges to Mismeasurement Explanations for the U.S. Productivity Slowdown," *Journal of Economic Perspectives*, 2017. <https://www.aeaweb.org/articles?id=10.1257/jep.31.2.165>
- Erik Brynjolfsson, Daniel Rock, and Chad Syverson, "The Productivity J-Curve," 2021. <https://www.aeaweb.org/articles?id=10.1257/mac.20180386>
- Erik Brynjolfsson, Danielle Li, and Lindsey R. Raymond, "Generative AI at Work," *Quarterly Journal of Economics*, 2025. <https://academic.oup.com/qje/article/140/2/889/7990658>
- U.S. Bureau of Labor Statistics via FRED, `OPHNFB`, Nonfarm Business Sector Labor Productivity. <https://fred.stlouisfed.org/series/OPHNFB>
- John Fernald et al., "Productivity During and Since the Pandemic," FRBSF Economic Letter, 2024. <https://www.frbsf.org/research-and-insights/publications/economic-letter/2024/11/productivity-during-and-since-pandemic/>
- Mary C. Daly, "The AI Moment? Possibilities, Productivity, and Policy," FRBSF Economic Letter, 2026. <https://www.frbsf.org/research-and-insights/publications/economic-letter/2026/02/ai-moment-possibilities-productivity-policy/>
- Nida Cakir Melek and Sydney Miller, "A New U.S. Productivity Chapter? What Industry Data Say About AI," Federal Reserve Bank of Kansas City Economic Bulletin, 2026. <https://www.kansascityfed.org/research/economic-bulletin/a-new-us-productivity-chapter-what-industry-data-say-about-ai/>

## Factual Guardrails

- David's `dynamo` is best treated as shorthand for the broader electrification regime. It is not the electric motor itself.
- The factory productivity mechanism runs through electric motors, factory electrification, and especially the shift from `group drive` to `unit drive`.
- The phrase "dynamos everywhere but in productivity statistics" is David's rhetorical counterfactual, not a famous 1900 quote.
- TFP/MFP is not a clean direct measurement of "technology." It is a residual-like productivity measure that can include measurement error, organization, scale effects, and uncounted inputs.
- Do not say David proved AI will succeed. The paper provides a lens and historical analogy, not a prophecy.
- Do not say Paul David did not live to see the later computer productivity story. He died in 2023.
- Use cautious wording for AI: task-level and some firm-level gains exist, but aggregate productivity causality is still early and contested in 2026.

## David 1990 Numbers Used In Deck

- In 1899, U.S. electric lighting was used in about 3% of all residences and about 8% of urban dwellings.
- In 1899, installed horsepower capacity of primary and secondary electric motors in U.S. manufacturing was less than 5% of factory mechanical drive.
- Factory mechanical drive electrified moved from 4.8% in 1899 to 53.1% in 1919 in David 1989 Table 3.
- Factory electrification gained real momentum after 1914-17, with lower electricity rates relative to the general price level and the rise of central-station generation.
- David 1990 p.359 says the rise in secondary electric motor capacity statistically accounts for approximately half of the 1919-29 acceleration in aggregate U.S. manufacturing TFP growth. Do not present unit drive as the only cause.

## Secondary Electric Motor

- David 1989 Table 3 includes two factory electrification measures:
  - Primary and secondary electric motor horsepower as a share of total mechanical drive in manufacturing.
  - Secondary electric motor horsepower as a share of non-electric direct-drive horsepower plus secondary electric motor horsepower.
- A simple talk-level explanation: in the Census/Duboff power statistics, primary electric motors typically belong to purchased-electricity/rented-power categories, while secondary electric motors are powered by electricity generated inside the plant and tracked separately to avoid double-counting the prime mover.
- David treats rising secondary electric motor penetration as a proxy for deeper factory electrification and the unit-drive transition. Do not explain it as a literal count of "second motors" or as precise one-machine-one-motor adoption.
- In the main deck, use only the broader and more intuitive `factory mechanical drive electrified` line.

## David 1989 Table 3 Data Used For Chart

| Year | Factory drive electrified | Secondary electric motor penetration |
|---:|---:|---:|
| 1899 | 4.8% | 3.0% |
| 1904 | 11.5% | 8.5% |
| 1909 | 24.7% | 17.3% |
| 1914 | 37.6% | 25.2% |
| 1919 | 53.1% | 32.6% |
| 1924 | 67.1% | 45.0% |
| 1929 | 78.4% | 56.4% |

## David 1989 Table 2 TFP Data Used For Appendix Chart

- Source: Paul A. David, "Computer and Dynamo: The Modern Productivity Paradox in a Not-Too-Distant Mirror," Warwick Economic Research Paper No. 339, 1989, Table 2.
- Data file in this repo: `data/manufacturing-tfp-david1989.csv`.
- Chart asset in this repo: `assets/manufacturing-tfp-electrification-era.svg`.
- Measure used: Kendrick-based U.S. manufacturing total factor productivity growth rate, geometric weighting (`Ag` in David's Table 2).
- These are period-average annual growth rates, not annual observations.

| Period | Manufacturing TFP growth, %/yr |
|---|---:|
| 1869-1879 | 0.31 |
| 1879-1889 | 1.23 |
| 1889-1899 | 0.86 |
| 1899-1909 | 0.50 |
| 1909-1919 | 0.17 |
| 1919-1929 | 5.29 |
| 1929-1937 | 1.96 |
| 1937-1948 | 1.56 |

- Talk-safe interpretation: the diffusion curve proves slow adoption; this TFP chart is the backup evidence for the measured productivity surge.
- David 1990 p.359 links roughly half of the 1919-1929 TFP acceleration, relative to 1909-1919, to growth in secondary electric motor capacity. Keep the "roughly half" wording and do not imply electrification explains the entire 1920s productivity surge.

## Image Sources

- `assets/line-shaft.jpg`: Wikimedia Commons `File:Line shaft.jpg`, sourced from Library of Congress / HAER CA-179-45. Public domain as U.S. National Park Service / HAER work. <https://commons.wikimedia.org/wiki/File:Line_shaft.jpg>
- `assets/kammgarnspinnerei-pfaffendorf-1925.jpg`: user-provided image copied from `/Users/eanu/Downloads/AHW_Kammgarnspinnerei_Pfaffendorf_Leipzig_um_1925.jpg`. Use as the main group-drive visual: overhead shafts and belts in Kammgarnspinnerei Pfaffendorf, Leipzig, c. 1925.
- `assets/marconi-individual-driving-motors.jpg`: Wikimedia Commons / NARA `Industries of War - Machinery - Engines - Doing war work in plant of Marconi Wireless Telephone Co., Aldene, New Jersey. Screw machine department. Note the individual driving motors - NARA - 45486522.jpg`. Public domain / no copyright in the United States. <https://commons.wikimedia.org/wiki/File:Industries_of_War_-_Machinery_-_Engines_-_Doing_war_work_in_plant_of_Marconi_Wireless_Telephone_Co.,_Aldene,_New_Jersey._Screw_machine_department._Note_the_individual_driving_motors_-_NARA_-_45486522.jpg>
- `assets/ibm-704-edp.jpg`: Wikimedia Commons `File:IBM Electronic Data Processing Machine - GPN-2000-001881.jpg`, NASA Langley photo, public domain as U.S. government work. <https://commons.wikimedia.org/wiki/File:IBM_Electronic_Data_Processing_Machine_-_GPN-2000-001881.jpg>

## Optional Public-Domain Visual Sources

- Library of Congress line shaft / group drive reference: <https://www.loc.gov/pictures/item/ne0071.photos.346105p/>
- Wikimedia line shaft file: <https://commons.wikimedia.org/wiki/File:Line_shaft.jpg>
- Steam-to-shaft reference, Library of Congress: <https://www.loc.gov/pictures/resource/hhh.pa3690.photos.142916p/>
- `assets/ford-assembly-line-1913.jpg`: Wikimedia Commons `File:Ford assembly line - 1913.jpg`, public domain in the United States. Useful only as a workflow-redesign visual, not as evidence of individual motors. <https://commons.wikimedia.org/wiki/File:Ford_assembly_line_-_1913.jpg>

## IT And AI Productivity Claims

- For the IT payoff slide, use cautious wording: after 1995, U.S. nonfarm-business productivity accelerated sharply; growth-accounting studies attribute a large share of the late-1990s speed-up, and a meaningful but smaller post-2000 share, to IT production and IT capital deepening.
- Avoid saying IT alone explains the whole 1995-2004 economy. Oliner and Sichel's strongest claim is about the 1990s acceleration, not a universal explanation for every later productivity movement.
- For the computer "unit drive" analogy, avoid saying "documents became digital." A stronger mechanism is operational redesign around live databases, ERP, supply-chain systems, real-time inventory, CAD/CAM, networked ordering, electronic payments, search, routing, and self-service.
- Plausible productivity channels: less re-keying and reconciliation, fewer errors, lower inventories, better capacity utilization, faster design cycles, shorter lead times, and new operating models across firms.
- For the slowdown, prefer `2005-2019` or `after the mid-2000s`, because the post-pandemic and post-2022 data are volatile and still being interpreted.
- For AI, the strongest evidence is task- or firm-level: Brynjolfsson, Li, and Raymond find 15% more issues resolved per hour in one customer-support setting, and the authors caution that the study is not designed to identify aggregate employment or wage effects.
- As of 2026, macro evidence for a durable AI-driven aggregate productivity regime change remains limited. The safe talk line is: "AI can clearly help in specific settings; economy-wide productivity causality is not yet settled."
