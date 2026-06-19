---
theme: default
title: "The Productivity Paradox"
info: |
  A rough internal sharing deck on Paul A. David's 1990 essay
  "The Dynamo and the Computer" and delayed productivity payoffs.
class: text-slate-800
drawings:
  persist: false
transition: none
mdc: true
fonts:
  sans: "Inter"
  serif: "Source Serif 4"
  mono: "JetBrains Mono"
---

<style>
:root {
  --slidev-theme-primary: #0f766e;
}
.slidev-layout {
  background: #f8fafc;
  color: #0f172a;
  font-size: 19px;
}
.slidev-layout h1 {
  color: #0f172a;
  font-size: 35px;
  line-height: 1.05;
  letter-spacing: 0;
}
.slidev-layout h2 {
  color: #0f172a;
  font-size: 28px;
  line-height: 1.12;
  letter-spacing: 0;
}
.kicker {
  color: #0f766e;
  font-size: 12px;
  font-weight: 800;
  letter-spacing: .10em;
  text-transform: uppercase;
  margin-bottom: 10px;
}
.muted { color: #64748b; }
.source {
  position: absolute;
  left: 48px;
  right: 48px;
  bottom: 12px;
  font-size: 9px;
  line-height: 1.15;
  color: #64748b;
}
.quote {
  font-family: Georgia, "Times New Roman", serif;
  font-size: 34px;
  line-height: 1.12;
  color: #0f172a;
}
.claim {
  font-size: 24px;
  line-height: 1.18;
  font-weight: 760;
}
.subclaim {
  font-size: 20px;
  line-height: 1.25;
  color: #334155;
}
.twocol {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 28px;
  align-items: center;
}
.threecol {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 16px;
}
.box {
  border: 1px solid #cbd5e1;
  background: #fff;
  border-radius: 8px;
  padding: 16px 18px;
}
.soft {
  background: #f1f5f9;
  border: 1px solid #dbe4ee;
  border-radius: 8px;
  padding: 16px 18px;
}
.small {
  font-size: 14px;
  line-height: 1.3;
}
.tiny {
  font-size: 11px;
  line-height: 1.35;
}
ul {
  line-height: 1.25;
}
.diagram {
  width: 100%;
  max-height: 390px;
  object-fit: contain;
}
.photo-pair {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 18px;
  margin-top: 8px;
}
.photo-panel {
  overflow: hidden;
  background: #fff;
  border: 1px solid #cbd5e1;
  border-radius: 8px;
}
.photo-panel img {
  display: block;
  width: 100%;
  height: 212px;
  object-fit: cover;
  filter: grayscale(100%) contrast(1.05);
}
.photo-panel .label {
  padding: 8px 12px 9px;
  font-size: 18px;
  font-weight: 820;
  line-height: 1.15;
}
.photo-panel .caption {
  padding: 0 12px 10px;
  color: #64748b;
  font-size: 10px;
  line-height: 1.25;
}
.edp-photo {
  width: 100%;
  height: 232px;
  object-fit: cover;
  filter: grayscale(100%) contrast(1.05);
  border-radius: 8px;
  border: 1px solid #cbd5e1;
}
.metric {
  border-left: 5px solid #0f766e;
  padding: 13px 16px;
  background: #fff;
  border-radius: 0 8px 8px 0;
}
.metric .number {
  font-size: 32px;
  font-weight: 840;
  line-height: 1;
  color: #0f766e;
}
.slidev-layout .text-5xl {
  font-size: 40px !important;
  line-height: 1 !important;
}
.slidev-layout .text-2xl {
  font-size: 19px !important;
  line-height: 1.2 !important;
}
.slidev-layout .text-xl {
  font-size: 16px !important;
  line-height: 1.25 !important;
}
.slidev-layout.end h1 {
  color: #f8fafc;
}
.slidev-layout.end .text-2xl {
  color: #cbd5e1;
}
/* Hide only Slidev chrome that is noisy in screenshots/presentation previews. */
#slide-container > nav,
#slidev-goto-dialog {
  display: none !important;
}
</style>

<div class="kicker">Productivity Paradox</div>

# The Productivity Paradox

<div class="mt-7 claim">
Why new technologies often pay off late
</div>

<div class="quote mt-10">
"We see the computers everywhere but in the productivity statistics."
</div>

<div class="mt-4 text-xl text-slate-400">電腦到處都看得到,就是在生產力的統計數字裡看不到。</div>

<div class="mt-5 text-xl text-slate-500">Robert Solow, quoted in Paul A. David (1990)</div>

<div class="source">Draft v3 | English slides | Paul A. David, "The Dynamo and the Computer"</div>

<!--
(Open cold. Say the quote first, before any throat-clearing.)

"We see the computers everywhere but in the productivity statistics."

中文大意:電腦到處都看得到,就是在生產力的統計數字裡看不到。經濟學家 Robert Solow 在 1980 年代末講的。投資很重、大家天天用、人人都覺得它重要,但攤開總體生產力的數字,卻幾乎沒有動。

(Beat.) He said that about computers, almost forty years ago. The same sentence is being said about AI today — "we see LLMs everywhere but not in the productivity statistics." A short 1990 economics paper tells us whether that should worry us.

The paper is Paul David's "The Dynamo and the Computer." The main story is not AI. It is a historical puzzle about computers, and David's way of using electrification to understand it.

That gap — visible everywhere, invisible in the numbers — is the productivity paradox. Near the end I will come back to AI; the foundation is the older paradox: computers were everywhere, yet the productivity statistics looked disappointing.
-->

---

<div class="kicker">Definition</div>

# Visible adoption, unclear payoff

<div class="mt-14 claim text-3xl text-center">
Real value — <span class="text-teal-700">not yet</span> real productivity.
</div>

<div class="threecol mt-14 text-center">
  <div class="soft" v-click>
    <div class="text-2xl font-bold">Tools show up</div>
  </div>
  <div class="soft" v-click>
    <div class="text-2xl font-bold">Numbers lag</div>
  </div>
  <div class="soft" v-click>
    <div class="text-2xl font-bold">Why? — unclear</div>
  </div>
</div>

<div class="source">Keep TFP/MFP for Q&A. In the talk, say "productivity numbers."</div>

<!--
Skip the TFP formula. For this room, an example is enough.

Concrete version first: your team adopts Copilot. Everyone uses it every day. Nobody can point to the sprint that actually got faster. That gap is the paradox.

(Optional show of hands.) Who here would say AI has measurably sped up your team's delivery? Now — who uses it every day? The gap between those two shows of hands is basically the whole talk.

The important point: the paradox does not mean "the tool has no value." It means the value is not yet visible as system-level productivity.

Two separate reasons the numbers lag, and David leans on both: (1) real — the work has not been redesigned around the tool yet; (2) measurement — the official statistics are partly blind, missing quality gains and whole new categories of output, so real gains show up late and understated. Keep the measurement point; it returns on the payoff slide.
-->

---

<div class="kicker">David's Move</div>

# David used electrification as a mirror for the computer age

<div class="twocol mt-7">
  <div class="soft">
    <div class="text-5xl font-bold text-teal-700">1900</div>
    <div class="mt-3 text-2xl font-bold">Electrical Age</div>
    <div class="mt-3 small">Light · motors · generators — everywhere. Payoff: not yet.</div>
  </div>
  <div class="soft">
    <div class="text-5xl font-bold text-blue-700">1990</div>
    <div class="mt-3 text-2xl font-bold">Computer Age</div>
    <div class="mt-3 small">Microprocessors · business computers — everywhere. Numbers: still flat.</div>
  </div>
</div>

<div class="mt-7 subclaim font-bold">
His question: why do general-purpose technologies (electricity, computers… maybe AI) often pay off late?
</div>

<div class="mt-3 small muted">Long, variable, not guaranteed — visible technology first, measured payoff later.</div>

<div class="source">David 1990, p.355-356.</div>

<!--
David's move is not "computers are literally dynamos."

He uses electrification as a historical mirror. Around 1900, the electrical age was visible. Around 1990, the computer age was visible. In both cases, the visible technology was ahead of the measured productivity payoff.

If someone asks why these two moments are being compared: each is a long interval after the enabling breakthrough — but the interval varies and is NOT a fixed clock. Edison and Swan's incandescent lamp and early central stations appear around 1879-1881, yet diffusion into factory drive was still only around half by 1919. Intel's memory chip and microprocessor appear around 1969-1970; the computer payoff shows up much later. Resist any "neat twenty-year rule" — the point is lag and contingency, not a constant.

Vocabulary: "general-purpose technology" = a technology that spreads across the whole economy (electricity, the computer, maybe AI); that breadth is why the payoff is slow. And in David's title, "dynamo" = the electric generator, his shorthand for the whole electrification regime.
-->

---

<div class="kicker">Diffusion Lag</div>

# Diffusion is not the payoff

<div class="mt-3">
  <img src="/assets/electrification-diffusion.svg" class="diagram" style="max-height:330px;" />
</div>

<div class="mt-2 subclaim font-bold">
This chart proves delay, not productivity. Productivity is a separate claim.
</div>

<div class="source">David 1990 p.356; David 1989 Table 3. Lighting note in speaker notes.</div>

<!--
Lead with the punch number: about twenty years after the lightbulb, in 1899, only about 3% of U.S. residences had electric light — 8% even in urban dwellings — and electric motors were less than 5% of factory mechanical drive.

The chart is one line: factory mechanical drive electrified. David says these aggregate measures took roughly another two decades to reach about 50% diffusion.

Do not claim the 1920s slope suddenly "surges"; visually, the point is safer and stronger: diffusion was slow. Also do not claim this diffusion chart proves productivity. The chart proves only that electricity took a long time to enter the factory core.

(Beat, then the lesson — the spine of the talk.) Invention is not diffusion. Diffusion is not redesign. Redesign — rebuilding how the work is done around the tool — is what eventually moves productivity. The productivity evidence is a separate claim. For the main talk, keep the mechanism simple: diffusion was slow, and only redesign can turn a technology into measured productivity.

(Appendix / only if asked.) The original table also has a "secondary electric motor" series. In David/DuBoff's usage, primary motors ran on purchased electricity from utilities; secondary motors ran on electricity generated inside the plant. Treat secondary-motor penetration as a proxy for deeper factory electrification and unit-drive diffusion, not as a literal motor type. Q&A material — do not spend main-talk time on it.
-->

---

<div class="kicker">Mechanism · 1 of 2</div>

# Group drive: one shaft drives the whole floor

<div class="photo-pair mt-2">
  <div class="photo-panel">
    <img src="/assets/kammgarnspinnerei-pfaffendorf-1925.jpg" style="object-position:50% 40%;" />
    <div class="label">The real thing (1925)</div>
    <div class="caption">Kammgarnspinnerei Pfaffendorf, Leipzig.</div>
  </div>
  <div class="photo-panel">
    <img src="/assets/line-shaft-group-drive.svg" style="object-fit:contain;filter:none;background:#fff;" />
    <div class="label">Same idea, simplified</div>
    <div class="caption">Even with an electric motor: one motor → shaft → belts → every machine</div>
  </div>
</div>

<div class="mt-3 subclaim font-bold">Swap the steam engine for a motor on the same shaft → barely helps. The constraint is the shaft, not the engine.</div>

<div class="source">David 1990 p.357-358; Devine 1983. Photo: user-provided Pfaffendorf image. Schematic: Claude.</div>

<!--
Centerpiece, part 1. Old factories ran group drive: one big steam engine turned a long overhead line shaft, and belts dropped power to each machine — every machine chained to that one spinning shaft. The historical photo (left) is hard to parse, so I had Claude draw the simplified schematic (right). The point the schematic makes: even if you swap the steam engine for an ELECTRIC MOTOR, as long as it still drives the same shaft, it is STILL group drive — and it barely helps. The constraint was never the engine; it was the shaft: the whole line spins all day even for one machine (friction/waste), machines must sit in a row near the shaft (not by workflow), they can't run at independent speeds, and one breakdown stops everyone.
-->

---

<div class="kicker">Mechanism · 2 of 2</div>

# Retrofit vs redesign: group drive → unit drive

<div class="photo-pair mt-2">
  <div class="photo-panel">
    <img src="/assets/kammgarnspinnerei-pfaffendorf-1925.jpg" style="object-position:50% 40%;" />
    <div class="label">Group drive: shafts + belts</div>
    <div class="caption">Kammgarnspinnerei Pfaffendorf, Leipzig, c. 1925.</div>
  </div>
  <div class="photo-panel">
    <img src="/assets/marconi-individual-driving-motors.jpg" style="object-position:50% 48%;" />
    <div class="label">Unit drive: motors at machines</div>
    <div class="caption">Screw-machine dept. with individual driving motors, Marconi, 1917-18.</div>
  </div>
</div>

<div class="mt-3 subclaim font-bold">Remove the shaft → redesign the floor. The productivity jump comes from the redesign, not the motor.</div>

<div class="mt-2 small muted">Main line: electrification enabled unit-drive redesign; redesign is what moves productivity.</div>

<div class="source">David 1990 p.357-358 (mechanism), p.359 (TFP decomposition); Devine 1983. Photos: user-provided Pfaffendorf image; NARA/Wikimedia Commons PD-US.</div>

<!--
Centerpiece, part 2 — the side-by-side. Left = group drive (shafts + belts), right = unit drive (a motor on each machine). The point: once you remove the shaft, you can redesign the whole floor — machines run on demand, laid out by workflow, independent speeds, isolated breakdowns, single-story plants with cranes and daylight. Productivity jumps from the REDESIGN the motor allowed, not from the motor itself. (Marconi photo is 1917-18 — unit drive beginning to appear, not the whole 1920s story.)

Carry-forward line for the rest of the talk: bolting a motor onto the old shaft is the same move as bolting a chatbot onto an unchanged workflow — you change the engine, not the constraints.

(Bridge.) The "why exactly the 1920s?" story is good Q&A material: power prices, replacement timing, design know-how, and capital all had to line up. For the main talk, skip that detour and move straight to computers: the pattern repeated.

(Appendix / if asked.) David's 1920s story is not only unit drive: secondary motor capacity explains about half of the 1919-1929 manufacturing TFP acceleration (p.359); continuous-process production, shift-work, instrumentation, process heat also matter.
-->

---

<div class="kicker">35 Years On</div>

# David was mostly right: payoff came late

<div class="threecol mt-8">
  <div class="box" v-click>
    <div class="text-2xl font-bold text-slate-500">Early 1990s</div>
    <div class="mt-3 small">Computers everywhere; productivity still weak.</div>
  </div>
  <div class="box" style="border-color:#5eead4;" v-click>
    <div class="text-2xl font-bold text-teal-700">1995–2004</div>
    <div class="mt-3 small">U.S. productivity accelerated; IT explained a large share.</div>
  </div>
  <div class="box" v-click>
    <div class="text-2xl font-bold text-slate-500">After 2005</div>
    <div class="mt-3 small">The boom faded; delayed does not mean guaranteed or permanent.</div>
  </div>
</div>

<div class="mt-7 claim">
Same shape as the dynamo: adoption first, payoff later. Patience, but not faith.
</div>

<div class="source">Oliner & Sichel 2000 (Table 2; pp.11–12); Jorgenson, Ho & Stiroh 2008; Syverson 2017; BLS.</div>

<!--
This is the "35 years on" layer. Keep it short in the talk: David was mostly right, but not in the simple "buy computers and productivity rises immediately" way.

The lag, in hard data: through the early 1990s, computer-hardware stock grew ~17%/yr and investment more than quadrupled after 1995, yet computers added only ~¼ point/yr to growth (still a tiny share of the capital stock). Adoption everywhere, payoff missing — David's electrification curve repeated.

Then it landed: Oliner & Sichel find nonfarm-business labor productivity accelerated from ~1.6%/yr (first half of the 1990s) to ~2.7%/yr (second half). IT capital deepening ≈ half the step-up; computer hardware's own contribution rose from ~¼ to ~0.6 point/yr; IT plus computer production ≈ two-thirds of the acceleration.

But it did not simply continue. From 2005 to 2019 growth slowed again despite internet, smartphones, and cloud. Frame the fade carefully: it was the redesign stalling, not the technology being exhausted — the complementary reorganization ran its course, not the silicon. (Post-2022 pickup in some series; attribution to AI is too young to call.)

The lesson is two words: patience, but not faith. The payoff can be delayed, partial, or temporary — and contingent, not permanent. Not a guarantee that arrives if you just wait.
-->

---

<div class="kicker">AI Extension</div>

# AI: old shaft or redesigned workflow?

<div class="twocol mt-5">
  <div class="box" style="background:#fff7ed;border-color:#fdba74;" v-click>
    <div class="text-2xl font-bold" style="color:#b45309;">Bolt-on (retrofit)</div>
    <div class="mt-3 small">opencode helps write / edit / test<br/>same repo · PR · review · "done"</div>
    <div class="mt-3 small" style="color:#b45309;font-weight:700;">You type less. The work is still shaped the same.</div>
  </div>
  <div class="box" style="background:#ecfdf5;border-color:#5eead4;" v-click>
    <div class="text-2xl font-bold" style="color:#0f766e;">Re-architect (redesign)</div>
    <div class="mt-3 small">agent owns a small ticket<br/>tests / CI = the gate<br/>humans review requirements, risk, responsibility</div>
    <div class="mt-3 small" style="color:#0f766e;font-weight:700;">"Done" changes. Accountability changes.</div>
  </div>
</div>

<div class="mt-4 claim">Self-check (not a scorecard): has it changed our org chart or our "definition of done" yet?</div>

<div class="source">AI analogy as a design question, not a forecast. Q&A: task-level evidence, private learning loops, Klarna. David 1990 p.360: "Computers are not dynamos."</div>

<!--
Now apply the lens to AI. Put a sharp claim on the table — as a provocation, not a verdict, because we are standing inside the transition and cannot yet measure it.

Make it about us — gently; this is a sharing, not a report card. We run opencode against our own on-prem model, and like almost everyone right now, we're mostly in the bolt-on phase: the agent writes and edits code faster, but it still flows through the same repo, pull request, review, and definition of "done." That's real, useful, and exactly where you'd expect to start. It's step one, not a mistake. The point isn't that we're doing it wrong; it's that there's a further step worth getting excited about.

But honor David's caution: from inside a transition you genuinely cannot tell early redesign from retrofit — the 1917 photo of motors-on-every-machine looked like nothing in the aggregate at the time. So "most AI is bolt-on" is a question to hold against your own work, not a confident diagnosis. It does not prove AI has failed, and it does not prove it will succeed. The evidence today is strongest at the task or firm level — real, measured gains in specific writing and customer-support settings. What we cannot yet say, in 2026, is that AI has caused a durable, economy-wide productivity regime change.

So: what would AI's re-architect moment look like for us? Keep only one strong contrast in the main talk — bolt-on AI means the old PR/review/done workflow stays intact; redesigned AI means the agent can own a bounded ticket, tests and CI become the gate, and humans move up to requirements, risk, and accountability. Save private learning loops, evals, tuning, and Klarna for Q&A.

One concrete shape of the re-architect version: a support org that does not just drop a bot beside its agents, but rebuilds the whole tier-one queue around an AI agent — defined escalation paths, a measured deflection rate, humans re-scoped to handle only what the agent hands up. That is a workflow-and-org redesign, not a tool bolted on. Most "we added an AI assistant" projects are not that.

The structural warning — David's own sharpest point. Factories got redesigned partly because the old ones physically wore out and had to be replaced; that replacement moment forced the redesign. Information systems and workflows do not wear out. A 2009 process can run untouched for fifteen years. Nothing forces the AI rewrite — so AI's re-architect moment may be structurally slower than electricity's, because decay will not do the work for us.

(Optional interaction.) Ask the room: name one thing your team does differently because of AI — not faster, differently. The silence, or the rare good answer, is the most persuasive evidence in this whole talk.
-->

---

<div class="kicker">Takeaway</div>

# Redesign the work, don't just add the tool

<div class="threecol mt-8">
  <div class="box">
    <div class="text-2xl font-bold">Do not over-celebrate</div>
    <div class="mt-3 small">A technology does not automatically become productivity.</div>
  </div>
  <div class="box">
    <div class="text-2xl font-bold">Do not over-dismiss</div>
    <div class="mt-3 small">Early statistics alone may be too impatient.</div>
  </div>
  <div class="box">
    <div class="text-2xl font-bold">Ask the design question</div>
    <div class="mt-3 small">Are we retrofitting, or redesigning the system?</div>
  </div>
</div>

<div class="mt-8 subclaim font-bold">
Factories got redesigned because the old ones fell apart. Your codebase won't — nothing forces the AI rewrite except you.
</div>

<div class="quote mt-7">
Are we bolting new tools onto old shafts,<br/>
or redesigning the factory?
</div>

<div class="source">Closing thesis: analogy as a thinking tool, not a forecast.</div>

<!--
The close is conservative, but it should still have teeth.

David is not saying "wait long enough and every new technology will save us." He is saying: do not judge a general-purpose technology too quickly from early productivity numbers. The electricity story was never about the generator alone — it was about redesigning factories. The computer story was never about buying computers — it was about becoming digital-native.

So for AI the question is not only "is the technology good enough?" It is "can we redesign work around it?" — and then the sharper version: factories got redesigned because the old ones fell apart; your codebase won't. Nothing will force the AI rewrite except you, so the only question that matters is whether you will do it on purpose.

(Land the line, then stop.) Are we bolting new tools onto old shafts, or redesigning the factory?
-->

---
layout: end
---

# Q&A

<div class="mt-8 text-2xl">Appendix candidates: why the 1920s | TFP surge chart | TFP 101 | Solow | electrification timeline (primary vs. secondary motors, p.359) | the banking & ATM case | "Computers are not dynamos" (p.360) | Why info systems never wear out | how economists disagree (Acemoglu ↔ Goldman) | private learning loops / Nadella | Klarna</div>

---

<div class="kicker">Appendix · Why The 1920s?</div>

# The payoff needed several conditions to line up

<div class="grid grid-cols-2 gap-5 mt-10">
  <div class="box">
    <div class="text-2xl font-bold">Cheaper, reliable power</div>
  </div>
  <div class="box">
    <div class="text-2xl font-bold">A replacement moment</div>
  </div>
  <div class="box">
    <div class="text-2xl font-bold">Design know-how</div>
  </div>
  <div class="box">
    <div class="text-2xl font-bold">Capital to build</div>
  </div>
</div>

<div class="mt-6 subclaim font-bold">
This is "historically contingent": the conditions had to line up — and they might not have.
</div>

<div class="source">David 1990 p.356-358.</div>

<!--
Why did the payoff become visible in the 1920s? Several conditions lined up — and each has a software parallel, so this is good Q&A material.

Cheaper, reliable power → the tool got cheap and trustworthy enough to build on (our GPT-4-class moment). Capital replacement moments → we redesign during a rewrite or migration, not mid-flight. Design know-how → someone has to actually learn the new architecture; it is a skill, not a switch. Investment climate → leadership has to fund the redesign.

This is what "historically contingent" means in plain English: the technology did not automatically produce productivity — it needed prices, capital-replacement moments, skills, and macro conditions to align, and they might not have. There was no guarantee; a different macro climate could have deferred the payoff for years. Use this only if someone asks why the payoff appeared in the 1920s specifically.
-->

---

<div class="kicker">Appendix · Productivity Evidence</div>

# Backup: the TFP surge is visible in the 1920s

<div class="mt-4">
  <img src="/assets/manufacturing-tfp-electrification-era.svg" class="diagram" style="max-height:360px;" />
</div>

<div class="source">David 1989, "Computer and Dynamo," Table 2, Kendrick-based U.S. manufacturing TFP growth rates, geometric weighting. See also David 1990 p.359.</div>

<!--
Use this only if someone asks: "If the diffusion curve doesn't prove productivity, where is the productivity evidence?"

Answer: not in the diffusion curve. David's longer 1989 paper reports period-average manufacturing TFP growth. The geometric-weighted Kendrick-based measure is 0.17% per year in 1909-1919 and 5.29% per year in 1919-1929. That is the productivity surge. David 1990 then connects roughly half of the acceleration statistically to the growth of secondary electric motor capacity, while warning that unit drive was not the whole story.

Important caveat: this is not an annual time series. The bars are period averages. Do not read this as exact year-by-year timing; read it as the historical evidence that the 1920s claim is about measured productivity, not a kink in the adoption curve.
-->

---

<div class="kicker">Appendix · Origins & dating</div>

# Why 1879 — and why David pairs "1900" with "1990"

<div class="twocol mt-6">
  <div class="soft">
    <div class="text-2xl font-bold">1879 → 1882: device → system</div>
    <div class="mt-3 small">1879: Edison's (and Swan's) practical incandescent lamp — a better <b>device</b>. 1882: Pearl Street Station, NYC — the first commercial <b>central station</b>: generation + distribution + metering + tariffs as one system. Electricity became <b>infrastructure</b>, not a product — the generality that makes it a general-purpose technology, and why the payoff came a generation later.</div>
  </div>
  <div class="soft">
    <div class="text-2xl font-bold">Why 1900 ≈ 1990</div>
    <div class="mt-3 small">David writes in 1990 — about two decades after the 1969–71 chip. So he stands at the matching electrical vantage: ~1900, about two decades after the 1880s dynamo. Both are <b>"we see it everywhere but not in the statistics"</b> diagnosis moments — <b>not</b> the payoff dates. The electrical payoff itself came later, in the 1920s.</div>
  </div>
</div>

<div class="mt-5 subclaim font-bold">1900 and 1990 are paired vantage points, not paired payoffs.</div>

<div class="source">David 1990 p.355-356; Pearl Street: IEEE ETHW. Rhetorical symmetry, not a fixed lag.</div>

---

<div class="kicker">Appendix · Data</div>

# Backup: electricity prices fell after 1914–17

<div class="mt-4">
  <img src="/assets/electricity-price-fall.svg" class="diagram" />
</div>

<div class="source">U.S. Census, Historical Statistics of the U.S., Series S 77 (nominal ¢/kWh); BLS CPI electricity vs all-items for the real/relative claim.</div>

---

<div class="kicker">Appendix · The lag, three times</div>

# Backup: diffusion vs payoff, three technologies

<div class="mt-4">
  <img src="/assets/diffusion-three-techs.svg" class="diagram" />
</div>

<div class="source">Electrification: David 1990; household figures (Smithsonian/ACEEE). Computers: Census CPS/ACS; Oliner &amp; Sichel 2000. AI: Bick-Blandin-Deming (NBER w32966); St. Louis Fed; Census BTOS. Metrics differ — see chart footnote.</div>

---

<div class="kicker">Appendix · how economists disagree about AI</div>

# Nobody serious says zero — nobody serious has it confirmed

<div class="grid grid-cols-2 gap-5 mt-7">
  <div class="box" style="border-left:5px solid #64748b;">
    <div class="text-2xl font-bold">Pessimist · Robert Gordon</div>
    <div class="mt-2 small">IT was a <b>one-time</b> boost; growth structurally slowed after ~1970. AI won't rival electricity or the motor.</div>
  </div>
  <div class="box" style="border-left:5px solid #94a3b8;">
    <div class="text-2xl font-bold">Sober · Acemoglu (2024)</div>
    <div class="mt-2 small">≤ <b>0.5–0.66% TFP over 10 yrs</b> (~0.06%/yr). Calls the big forecasts "hyperbolic."</div>
  </div>
  <div class="box" style="border-left:5px solid #0f766e;">
    <div class="text-2xl font-bold">Mismeasured · Brynjolfsson et&nbsp;al.</div>
    <div class="mt-2 small">The "productivity <b>J-curve</b>": gains are real but hidden in unmeasured intangible / reorg investment — a dip, then a surge.</div>
  </div>
  <div class="box" style="border-left:5px solid #0f766e;">
    <div class="text-2xl font-bold">Optimist · Goldman Sachs</div>
    <div class="mt-2 small"><b>~+1.5%/yr</b> productivity for a decade (~+$7T) — though GS also finds "no economy-wide effect <i>yet</i>."</div>
  </div>
</div>

<div class="mt-6 subclaim font-bold">The honest range runs ~0.5%/yr (Acemoglu) to ~1.5%/yr (Goldman) — which is exactly why the talk says "patience, but not faith."</div>

<div class="source">Gordon, NBER w19895; Acemoglu, "Simple Macroeconomics of AI," NBER w32487; Brynjolfsson, Rock &amp; Syverson, "Productivity J-Curve," NBER w25148; Goldman Sachs Global Economics (2023).</div>

---

<div class="kicker">Appendix · more "new tool vs new model" cases</div>

# Backup: the supermarket & the paperless-office trap

<div class="twocol mt-6">
  <div class="box small" style="line-height:1.55;">
    <div class="text-2xl font-bold">Supermarket</div>
    <div class="mt-2"><b>Tool on the old model:</b> clerks count stock by hand → type it in at night; cashiers key in prices. A faster filing cabinet — the numbers don't move.</div>
    <div class="mt-2"><b>New model:</b> barcode scan at checkout → inventory updates &amp; reorders itself; the database becomes the source of truth. Less cash in stock, fewer stockouts, fewer counters.</div>
  </div>
  <div class="box small" style="line-height:1.55;">
    <div class="text-2xl font-bold">The "paperless office" trap</div>
    <div class="mt-2">Predicted in 1975 — yet paper use kept rising for decades. E-signatures had no legal force until <b>UETA 1999 / ESIGN 2000</b>, so firms scanned documents <i>and still</i> printed, wet-signed, mailed, and filed them.</div>
    <div class="mt-2">A new tool bolted onto a paper process the law wouldn't let you retire — the payoff comes only when the workflow itself is rebuilt.</div>
  </div>
</div>

<div class="source">Retail/IT productivity: McKinsey Global Institute 2001; Basker 2012 (barcode scanner). E-signature law: UETA 1999, ESIGN 2000. EDP framing: David 1990 p.357, p.360; Baily &amp; Gordon 1988.</div>

<!--
(Backup, if asked.) Two more cases of "a new tool on the old model" vs. "rebuilding the model."

Supermarket: tool-on-old-model — clerks count stock by hand, type it in at night; cashiers key in prices; stock data always stale. New model — barcodes + checkout scanners: every sale updates inventory instantly, low stock reorders itself; the computer becomes where stock reality lives, not a filing cabinet you copy into. Gain: less cash in stock, fewer stockouts, fewer counters — from redesigning the store, not buying a computer.

Paperless office: e-signatures had no legal force until UETA 1999 / ESIGN 2000, so firms scanned documents and still printed, wet-signed, mailed, and filed them — a parallel process bolted on. The "paperless office" was predicted in 1975; paper use kept rising for decades. The payoff needs the workflow rebuilt, not just digitized.
-->

---

<div class="kicker">Appendix · the banking case</div>

# Banking: three waves of tech, three job outcomes

<div class="grid grid-cols-3 gap-4 mt-7">
  <div class="metric" style="border-left-color:#64748b;">
    <div class="number" style="color:#64748b;font-size:22px;">1960s–70s</div>
    <div class="mt-2 text-2xl font-bold">Back office goes digital</div>
    <div class="mt-2 small">Records computerized; bookkeeping speeds up. You still visit the branch; the teller still serves you. <b>Tellers ≈ unchanged.</b></div>
  </div>
  <div class="metric">
    <div class="number" style="font-size:22px;">1970s–2000s</div>
    <div class="mt-2 text-2xl font-bold">ATM extends the branch</div>
    <div class="mt-2 small">Tellers per branch fall (~20→13), but cheaper branches let banks open <b>~40% more</b>. Total tellers <b>rise</b> (~300k → ~600k).</div>
  </div>
  <div class="metric" style="border-left-color:#0f766e;">
    <div class="number" style="color:#0f766e;font-size:22px;">2010s–</div>
    <div class="mt-2 text-2xl font-bold">Mobile moves the bank home</div>
    <div class="mt-2 small">Travel distance ≈ 0; branches become unnecessary → closures (peak 2009). Tellers <b>fall</b> (~600k → mid-300k).</div>
  </div>
</div>

<div class="mt-5 subclaim font-bold">A new tool made the old model cheaper without cutting jobs. Headcount moved only when the model itself changed.</div>

<div class="mt-2 small muted">Why only the 2010s? smartphone + app store (2007–08), 4G (2010), and a 2004 law (Check 21) that legalized depositing a check by photo. Historically contingent — like the dynamo.</div>

<div class="source">Bessen, IMF F&amp;D 2015 (tellers 20→13 &amp; urban branches +~40%, 1988–2004; ~400k ATMs); FDIC (branch peak 2009); BLS OEWS (teller counts, rounded). Post-2009 decline also reflects 2008-crisis mergers and falling cash use.</div>

<!--
(Backup, if asked — the cleanest modern instance.) David's real target was the computer paradox, and banking is where you can watch it. Wave 1 (back office, 1960s–70s): records digitized, but you still visit the branch — tellers ≈ unchanged. Wave 2 (ATM): cut tellers per branch (~20→13), but cheaper branches → ~40% more branches → total tellers ROSE (~300k→600k). The machine expected to kill the teller grew the teller. Wave 3 (mobile, 2010s): the bank moves into your phone; branches become a cost not a weapon → closures (peak 2009) → tellers fall to mid-300k. The tool made the old model cheaper; only the new model changed the jobs. (Honest caveat: post-2008 mergers and falling cash use also drove closures.)
-->
