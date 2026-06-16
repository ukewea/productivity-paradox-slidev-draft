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
  <div class="soft">
    <div class="text-2xl font-bold">Tools show up</div>
  </div>
  <div class="soft">
    <div class="text-2xl font-bold">Numbers lag</div>
  </div>
  <div class="soft">
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
    <div class="mt-3 small">Electric light, generation, transmission, and motors were visible, but the productivity payoff had not fully arrived.</div>
  </div>
  <div class="soft">
    <div class="text-5xl font-bold text-blue-700">1990</div>
    <div class="mt-3 text-2xl font-bold">Computer Age</div>
    <div class="mt-3 small">Microprocessors and early business computers were spreading, but the productivity statistics still looked disappointing.</div>
  </div>
</div>

<div class="mt-7 subclaim font-bold">
His question: why do general-purpose technologies (electricity, computers… maybe AI) often pay off late?
</div>

<div class="mt-3 small muted">The lag is long and variable — and not guaranteed: lamp 1879 → factory payoff 1920s (~40 yrs); microchip 1970 → computer payoff late 1990s. It arrives only if the conditions align.</div>

<div class="source">David 1990, p.355-356.</div>

<!--
David's move is not "computers are literally dynamos."

He uses electrification as a historical mirror. Around 1900, the electrical age was visible. Around 1990, the computer age was visible. In both cases, the visible technology was ahead of the measured productivity payoff.

If someone asks why these two moments are being compared: each is a long interval after the enabling breakthrough — but the interval varies and is NOT a fixed clock. Edison and Swan's incandescent lamp and early central stations appear around 1879-1881, yet the factory payoff waits until the 1920s (David: roughly four decades after the first central station). Intel's memory chip and microprocessor appear around 1969-1970; the computer payoff shows up in the late 1990s. Resist any "neat twenty-year rule" — the point is contingency, not a constant.

Vocabulary: "general-purpose technology" = a technology that spreads across the whole economy (electricity, the computer, maybe AI); that breadth is why the payoff is slow. And in David's title, "dynamo" = the electric generator, his shorthand for the whole electrification regime.
-->

---

<div class="kicker">Diffusion Lag</div>

# In 1900, electrification was still early

<div class="mt-4">
  <img src="/assets/electrification-diffusion.svg" class="diagram" />
</div>

<div class="source">David 1990 p.356; David 1989 Table 3. Lighting note: 3% of all U.S. residences, 8% of urban dwellings in 1899.</div>

<!--
Lead with the punch number: eighteen years after the lightbulb, in 1899, only about 3% of U.S. residences had electric light — 8% even in urban dwellings — and electric motors were less than 5% of factory mechanical drive.

The chart is one line: factory mechanical drive electrified. David says these aggregate measures took roughly another two decades to reach about 50% diffusion.

(Beat, then the lesson — the spine of the talk.) Invention is not diffusion. Diffusion is not redesign. And redesign — rebuilding how the work is done around the tool — is what eventually moves productivity. Hold that word; the next slide is all about it.

(Appendix / only if asked.) The original table also has a "secondary electric motor" series. In David/DuBoff's usage, primary motors ran on purchased electricity from utilities; secondary motors ran on electricity generated inside the plant. Treat secondary-motor penetration as a proxy for deeper factory electrification and unit-drive diffusion, not as a literal motor type. Q&A material — do not spend main-talk time on it.
-->

---

<div class="kicker">Mechanism</div>

# The key mechanism: retrofit is not redesign

<div class="photo-pair">
  <div class="photo-panel">
    <img src="/assets/kammgarnspinnerei-pfaffendorf-1925.jpg" style="object-position:50% 40%;" />
    <div class="label">Group drive: shafts + belts</div>
    <div class="caption">Kammgarnspinnerei Pfaffendorf, Leipzig, c. 1925.</div>
  </div>
  <div class="photo-panel">
    <img src="/assets/marconi-individual-driving-motors.jpg" style="object-position:50% 48%;" />
    <div class="label">Unit drive: motors at machines</div>
    <div class="caption">Screw-machine department with individual driving motors, Marconi, 1917-18.</div>
  </div>
</div>

<div class="mt-3 subclaim font-bold">
In software: group drive = lift-and-shift; unit drive = re-architecting around the new primitive.
</div>

<div class="mt-2 small muted">Unit drive existed by the 1910s — yet the payoff waited for the 1920s. Why then? →</div>

<div class="source">David 1990 p.357-358 (mechanism), p.359 (TFP decomposition); Devine 1983. Photos: user-provided Pfaffendorf image; NARA/Wikimedia Commons PD-US.</div>

<!--
This is the most important slide. If they remember one idea, this is it.

In old factories, a central prime mover powered long overhead shafts; belts carried power down to machines. Early electrification often kept that architecture — a motor was added to drive sections of the old shafting. That is group drive: new power source, old factory geometry.

Unit drive changed the architecture: each machine got its own motor, power arrived by wire, and the whole building could be redesigned — single-story layouts, flexible placement, easier maintenance, safer cleaner floors.

For engineers, this is the same distinction we live with. Group drive is lift-and-shift: monolith to the cloud, new infrastructure, identical architecture. Unit drive is re-architecting around the new primitive. Bolting a motor onto the old shaft is the same move as bolting a chatbot onto an unchanged workflow — and neither moves the numbers much.

The photo on the right is a Marconi screw-machine department whose archival caption explicitly notes individual driving motors. Caveat: it is from 1917-18, so use it as a concrete visual of unit drive beginning to appear, not as the entire 1920s diffusion story.

(Appendix / only if asked.) David's 1920s story is not only unit drive. Secondary motor capacity statistically explains about half of the 1919-1929 manufacturing TFP acceleration (p.359); continuous-process production, shift-work, electrical instrumentation, and process heat also matter. Keep for Q&A — it muddies the cleanest idea in the talk.

(Bridge into the next slide.) Notice the timing puzzle: unit drive existed already in the 1900s-1910s — the Marconi photo is 1917 — yet the productivity payoff did not really land until the 1920s. The technology was available before the payoff arrived. So why the 1920s? That is the next slide.
-->

---

<div class="kicker">Why The 1920s?</div>

# The payoff needed several conditions to line up

<div class="grid grid-cols-2 gap-5 mt-8">
  <div class="box">
    <div class="text-2xl font-bold">Cheaper, reliable power</div>
    <div class="mt-3 small">After 1914-17, electricity rates fell relative to the general price level.</div>
  </div>
  <div class="box">
    <div class="text-2xl font-bold">Capital replacement moments</div>
    <div class="mt-3 small">Old plants had to depreciate, become obsolete, or be replaced during expansion.</div>
  </div>
  <div class="box">
    <div class="text-2xl font-bold">Design know-how</div>
    <div class="mt-3 small">Architects and engineers had to learn how to build around electric drive.</div>
  </div>
  <div class="box">
    <div class="text-2xl font-bold">Investment climate</div>
    <div class="mt-3 small">The 1920s fixed-capital boom created more chances to build new plants.</div>
  </div>
</div>

<div class="mt-6 subclaim font-bold">
This is "historically contingent": the conditions had to line up — and they might not have.
</div>

<div class="source">David 1990 p.356-358.</div>

<!--
Why did the payoff become visible in the 1920s? Several conditions lined up — and each has a software parallel, so this is a Monday checklist.

Cheaper, reliable power → the tool got cheap and trustworthy enough to build on (our GPT-4-class moment). Capital replacement moments → we redesign during a rewrite or migration, not mid-flight. Design know-how → someone has to actually learn the new architecture; it is a skill, not a switch. Investment climate → leadership has to fund the redesign.

This is what "historically contingent" means in plain English: the technology did not automatically produce productivity — it needed prices, capital-replacement moments, skills, and macro conditions to align, and they might not have. There was no guarantee; a different macro climate could have deferred the payoff for years (and remember what followed the 1920s). David's argument explicitly allows that the gains arrive much later than hoped, or not on the expected schedule at all. So this is not "be patient, it always pays off" — it is "it pays off only if the conditions align."
-->

---

<div class="kicker">One industry, three waves</div>

# Same bank, three waves of tech — very different effects on jobs

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

<div class="mt-2 small muted">Why only the 2010s? The pieces had to line up — smartphone + app store (2007–08), 4G (2010), and a 2004 law (Check 21) that legalized depositing a check by photo. The payoff was historically contingent — just like the dynamo.</div>

<div class="source">Bessen, IMF F&amp;D 2015 (urban branches +~40% &amp; tellers 20→13, 1988–2004; ~400k ATMs); FDIC (branch peak 2009); BLS OEWS (teller counts, rounded). Post-2009 decline also reflects 2008-crisis mergers and falling cash use.</div>

<!--
David's real target was not the factory — it was the computer productivity paradox. The cleanest place to watch it is one industry we all use: banking.

Wave one, 1960s–70s: banks computerize the back office. Records go digital, bookkeeping speeds up — but you still drive to the branch and a teller still serves you. The computer made the old way faster; it did not change who does the work. Teller numbers barely move.

Wave two, the ATM (1970s on): a cash machine extends the bank's reach. It cut tellers needed per branch — about 20 to 13 between 1988 and 2004 (Bessen). But the twist economists love: because the ATM made each branch cheaper, and convenience then meant being physically close, banks opened ~40% more branches. Fewer tellers per branch × many more branches = total tellers ROSE, ~300k (1970) to ~600k (2010). The machine expected to kill the teller grew the teller.

Wave three, mobile banking (2010s): the bank moves into your phone — travel distance drops to ~zero. Now the branch is a cost, not a weapon. Banks close branches (US count peaked 2009) and tellers finally fall — into the mid-300-thousands by the early 2020s. Be fair: post-2008 mergers and falling cash use pushed the same way, not mobile alone.

Punchline — the whole talk in one line: for ~40 years the technology made banking cheaper WITHOUT cutting the workforce. The jobs moved only when the model itself changed. A new tool makes the old model efficient; only a new model changes the work.

Why did mobile land only in the 2010s, when "phone banking" existed in the late 1990s? The complements had to line up: smartphone + app store (2007–08), fast mobile internet (4G, 2010), and the underrated one — a 2004 law, Check 21, that made depositing a check by photo legal at all. The idea was old; the payoff was historically contingent, exactly like the dynamo waiting for the 1920s.

(Bridge to AI:) So hold that question for AI: are we adding a new tool to the old model, or building a new model?
-->

---

<div class="kicker">35 Years On</div>

# The computer payoff came late — then faded

<div class="grid grid-cols-3 gap-4 mt-8">
  <div class="metric" style="border-left-color:#64748b;">
    <div class="number" style="color:#64748b;font-size:23px;">~1990–95</div>
    <div class="mt-2 text-2xl font-bold">Everywhere, not in the numbers</div>
    <div class="mt-2 small">Computer stock grew <b>~17%/yr</b>, investment <b>4×</b> after 1995 — yet only <b>+¼ pt/yr</b> to growth.</div>
  </div>
  <div class="metric">
    <div class="number" style="font-size:23px;">1996–2004</div>
    <div class="mt-2 text-2xl font-bold">It landed</div>
    <div class="mt-2 small">Labor productivity <b>~1.6% → ~2.7%/yr</b>. IT ≈ <b>half</b> the step-up; <b>~⅔</b> with computer production.</div>
  </div>
  <div class="metric" style="border-left-color:#64748b;">
    <div class="number" style="color:#64748b;font-size:23px;">2005–2019</div>
    <div class="mt-2 text-2xl font-bold">Faded — the redesign stalled, not the tech</div>
    <div class="mt-2 small">Growth slowed despite internet, smartphones, and cloud. Payoff is contingent, not permanent.</div>
  </div>
</div>

<div class="mt-7 claim">
Same shape as the dynamo: huge adoption first, payoff much later. Patience, but not faith.
</div>

<div class="source">Oliner & Sichel 2000 (Table 2; pp.11–12); Jorgenson, Ho & Stiroh 2008; Syverson 2017; BLS.</div>

<!--
This is the "35 years on" layer David could not see — and the numbers line up with his framework, rather than vindicating a forecast he never made.

The lag, in hard data: through the early 1990s, computer-hardware stock grew ~17%/yr and investment more than quadrupled after 1995, yet computers added only ~¼ point/yr to growth (still a tiny share of the capital stock). Adoption everywhere, payoff missing — David's electrification curve repeated.

Then it landed: Oliner & Sichel find nonfarm-business labor productivity accelerated from ~1.6%/yr (first half of the 1990s) to ~2.7%/yr (second half). IT capital deepening ≈ half the step-up; computer hardware's own contribution rose from ~¼ to ~0.6 point/yr; IT plus computer production ≈ two-thirds of the acceleration.

But it did not simply continue. From 2005 to 2019 growth slowed again despite internet, smartphones, and cloud. Frame the fade carefully: it was the redesign stalling, not the technology being exhausted — the complementary reorganization ran its course, not the silicon. (Post-2022 pickup in some series; attribution to AI is too young to call.)

The lesson is two words: patience, but not faith. The payoff can be delayed, partial, or temporary — and contingent, not permanent. Not a guarantee that arrives if you just wait.
-->

---

<div class="kicker">AI Extension</div>

# AI may still be in its group-drive phase

<div class="twocol mt-5">
  <div class="box" style="background:#fff7ed;border-color:#fdba74;">
    <div class="text-2xl font-bold" style="color:#b45309;">Group drive — bolted on</div>
    <div class="mt-3 small">Copilot in the same IDE &amp; PR ritual · a RAG bot over a knowledge base nobody reorganized · a support bot <i>beside</i> agents → <b>+14%</b> resolved/hr, real &amp; measured (Brynjolfsson et al. 2023).</div>
    <div class="mt-3 small" style="color:#b45309;font-weight:700;">You type less. Org chart &amp; "definition of done" unchanged.</div>
  </div>
  <div class="box" style="background:#ecfdf5;border-color:#5eead4;">
    <div class="text-2xl font-bold" style="color:#0f766e;">Unit drive — redesigned</div>
    <div class="mt-3 small">An agent owns an end-to-end slice · evals/tests become the source of truth · review gates &amp; accountability rebuilt · the whole queue rebuilt around the agent (Klarna 2024).</div>
    <div class="mt-3 small" style="color:#0f766e;font-weight:700;">Org chart &amp; "done" change — this is what moves the numbers.</div>
  </div>
</div>

<div class="mt-4 claim">Test: if your AI rollout didn't change your org chart or your definition of done — you built group drive.</div>

<div class="mt-2 small muted"><i>And from inside, you can't yet tell which you built: Klarna rebuilt its queue around AI in 2024 — then re-hired humans in 2025.</i></div>

<div class="source">Brynjolfsson, Li &amp; Raymond 2023 (NBER w31161); Klarna 2024–25 (company/press). Lens, not prophecy — David 1990 p.360: "Computers are not dynamos."</div>

<!--
Now apply the lens to AI. Put a sharp claim on the table — as a provocation, not a verdict, because we are standing inside the transition and cannot yet measure it.

The claim, stated sharply so you can argue with it: most of what we have built with LLMs so far looks like group drive. A chatbot bolted onto an old workflow. Copilot autocompleting inside the same IDE, same review process, same PR ritual — you type less, but the workflow is unchanged. A RAG bot in front of a knowledge base nobody reorganized. New power source, old factory geometry.

But honor David's caution: from inside a transition you genuinely cannot tell early redesign from retrofit — the 1917 unit-drive photo looked like nothing in the aggregate at the time. So "most AI is group drive" is a question to hold against your own work, not a confident diagnosis. It does not prove AI has failed, and it does not prove it will succeed. The evidence today is strongest at the task or firm level — real, measured gains in specific writing and customer-support settings. What we cannot yet say, in 2026, is that AI has caused a durable, economy-wide productivity regime change.

So: what is AI's unit-drive moment? Concrete candidates to argue about — (1) an agent owns an end-to-end slice of work, not a sub-step a human stitches together; (2) evals and tests become the source of truth, the way the database did in the computer's unit-drive era; (3) review gates, accountability, and responsibility boundaries get redesigned — who is on the hook when the agent ships? That is an org-chart change, not a tooling change; (4) pipelines designed assuming a probabilistic component (retries, verification, fallback), not a deterministic one bolted in.

One concrete shape of unit drive: a support org that does not just drop a bot beside its agents, but rebuilds the whole tier-one queue around an AI agent — defined escalation paths, a measured deflection rate, humans re-scoped to handle only what the agent hands up. That is a workflow-and-org redesign, not a tool bolted on. Most "we added an AI assistant" projects are not that.

The structural warning — David's own sharpest point. Factories got redesigned partly because the old ones physically wore out and had to be replaced; that replacement moment forced the redesign. Information systems and workflows do not wear out. A 2009 process can run untouched for fifteen years. Nothing forces the AI rewrite — so AI's unit-drive moment may be structurally slower than electricity's, because decay will not do the work for us.

(Optional interaction.) Ask the room: name one thing your team does differently because of AI — not faster, differently. The silence, or the rare good answer, is the most persuasive evidence in this whole talk.
-->

---

<div class="kicker">Takeaway</div>

# Build the unit drive

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

<div class="mt-8 text-2xl">Appendix candidates: TFP 101 | Solow | electrification timeline (primary vs. secondary motors, p.359) | EDP vs PC/cloud | "Computers are not dynamos" (p.360) | Why info systems never wear out — so the rewrite is never forced</div>

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

<div class="source">David 1990 p.355-356. Pearl Street: IEEE ETHW. The ~two-decade vantage is rhetorical symmetry, not a fixed lag.</div>

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

