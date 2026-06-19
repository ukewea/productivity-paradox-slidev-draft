# Why The 1920s TFP Surge Can Be Linked To Electrification, But Not Fully Attributed To It

This note stores the evidence behind the Q&A answer:

> Why can we say the 1920s manufacturing TFP surge is related to electrification if earlier TFP growth cannot be attributed to electrification?

The short version:

> Do not say the 1920s TFP surge was entirely caused by electrification. The safer claim is that the 1920s manufacturing TFP acceleration lines up with electrification much better than the 1880s does, because by then factory electric drive had diffused, unit drive was spreading, and David found a positive cross-industry relationship between secondary motor growth and TFP acceleration.

## Three Layers Of Evidence

### 1. Diffusion timing

In the 1880s, factory electrification was essentially absent. In David 1989 Table 3, factory drive electrified was only `0.3%` in 1889.

By contrast, the 1920s were the decade when electric drive was already central to manufacturing:

| Year | Factory drive electrified | Secondary motor penetration |
|---:|---:|---:|
| 1919 | 53.1% | 32.6% |
| 1929 | 78.4% | 56.4% |

So the 1920s are not just a random decade after invention. They are the decade when factory electrification was already deep enough to plausibly matter.

### 2. Mechanism

Devine's `From Shafts to Wires` explains why unit drive could increase productivity:

- power no longer had to move through long shafts and belts;
- less energy was wasted rotating shafts when machines were idle;
- machines could be arranged by workflow instead of shaft geometry;
- material handling improved because clear headroom allowed cranes and better flow;
- one machine's failure no longer stopped a whole shaft line;
- machine control improved;
- factories became cleaner, safer, brighter, and easier to ventilate.

This is why the deck says the payoff was not merely "more electricity." The key mechanism is that electricity removed old constraints and enabled factory redesign.

### 3. Cross-industry evidence

David 1989 did not rely only on a time coincidence. He compared industries.

His Table 5 and related regression look at whether industries with larger increases in secondary electric motor capacity also had stronger acceleration in adjusted TFP growth during the 1920s. The relationship was positive and statistically significant in the sample he used.

David's interpretation is careful:

- the relationship can explain only part of the aggregate acceleration;
- his rough calculation says secondary motor capacity accounts for about `2.42` percentage points of a `5.12` percentage-point TFP acceleration, i.e. somewhat less than half;
- he explicitly warns against attributing everything in 1920s manufacturing productivity to this one technical change.

David and Wright 1999 sharpen the wording: the 1920s productivity surge reflected a confluence of electrification, complementary technologies, factory organization, continuous-process manufacturing, shift-work, and labor-market changes. Electrification was a key part of the story, not the whole story.

## Q&A Phrasing

> 我不會說 1920s 的 TFP 提升全部都是電氣化造成的。比較準確是說:1920s 的 manufacturing TFP acceleration 有相當大一部分跟工廠電氣化有關。
>
> 差別在於, 1880s 的時候電動馬達在工廠動力裡幾乎還不存在, 所以那段 TFP growth 很難歸因於 electrification。
>
> 但到 1920s, 工廠動力電氣化已經過半, secondary motor / unit-drive proxy 也快速上升, 工廠 layout、material handling、machine control 開始重設計。而且 David 有做跨產業比較: secondary motor capacity 增加比較多的產業, TFP acceleration 也比較明顯。
>
> 所以我們不是只靠時間巧合, 而是有三層證據: diffusion timing、mechanism、cross-industry correlation。但還是要補一句:它不是唯一原因, David 自己也說大概最多解釋一半左右。

## Sources

- Paul A. David, "Computer and Dynamo: The Modern Productivity Paradox in a Not-Too-Distant Mirror," Warwick Economic Research Paper No. 339, 1989, Tables 2, 3, and 5. <https://warwick.ac.uk/fac/soc/economics/research/workingpapers/1989-1994/twerp339.pdf>
- Paul A. David and Gavin Wright, "Early Twentieth Century Productivity Growth Dynamics: An Inquiry into the Economic History of 'Our Ignorance'," 1999, especially the sections on 1920s manufacturing, secondary motor capacity, and the confluence of electrification and labor/organizational change. <https://www.nuffield.ox.ac.uk/Economics/History/Paper33/33david4.pdf>
- Warren D. Devine Jr., "From Shafts to Wires: Historical Perspective on Electrification," *Journal of Economic History*, 1983. <https://gwern.net/doc/economics/automation/1983-devine.pdf>
- Chart asset in this repo: `assets/electrification-secondary-motor-vs-tfp.svg`.
