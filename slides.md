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
  margin-top: 14px;
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
  height: 272px;
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
  height: 292px;
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

<div class="mt-5 text-xl text-slate-500">Robert Solow, quoted in Paul A. David (1990)</div>

<div class="source">Draft v3 | English slides | Paul A. David, "The Dynamo and the Computer"</div>

<!--
Today I want to share a short 1990 essay by Paul David, "The Dynamo and the Computer."

The main story is not AI. It is a historical puzzle about computers, and David's way of using electrification to understand that puzzle.

The entry point is Robert Solow's famous line: "We see the computers everywhere but in the productivity statistics."

That is the productivity paradox: a technology is visible, organizations invest in it, people feel it matters, but aggregate productivity numbers do not clearly move.

Near the end, I will briefly mention why this story feels relevant to AI. But the foundation is the older productivity paradox: computers were visible, yet productivity statistics looked disappointing.
-->

---

<div class="kicker">Definition</div>

# Visible adoption, unclear productivity payoff

<div class="threecol mt-8">
  <div class="box">
    <div class="text-2xl font-bold">Tools show up</div>
    <div class="mt-3 small">People buy, try, and talk about the new technology.</div>
  </div>
  <div class="box">
    <div class="text-2xl font-bold">Numbers lag</div>
    <div class="mt-3 small">Aggregate productivity does not immediately jump.</div>
  </div>
  <div class="box">
    <div class="text-2xl font-bold">Meaning stays open</div>
    <div class="mt-3 small">Too weak, too early, badly measured, or not yet redesigned around?</div>
  </div>
</div>

<div class="mt-8 claim">
The paradox is not "no value." It is value that has not yet become system-level productivity.
</div>

<div class="source">Keep TFP/MFP for Q&A. In the talk, say "productivity numbers."</div>

<!--
I would avoid starting with the TFP formula. For this audience, the intuitive version is enough.

Imagine a company buys many tools, everyone uses them, and yet overall throughput, cost, or delivery speed does not obviously improve. That is the paradox.

The important point is that the paradox does not mean "the tool has no value." It means the value is not yet visible as system-level productivity.
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
    <div class="mt-3 small">Microprocessors and EDP systems were spreading, but the productivity statistics still looked disappointing.</div>
  </div>
</div>

<div class="mt-7 subclaim font-bold">
His question: why do general-purpose technologies often pay off late?
</div>

<div class="source">David 1990, p.355-356.</div>

<!--
David's move is not "computers are literally dynamos."

He uses electrification as a historical mirror. Around 1900, the electrical age was visible. Around 1990, the computer age was visible. In both cases, the visible technology was ahead of the measured productivity payoff.

If someone asks why these two moments are being compared: both dates are roughly two decades after major enabling breakthroughs became visible. Edison and Swan's incandescent lamp and early central stations appear around 1879-1881; Intel's memory chip and microprocessor appear around 1969-1970.

Also, be precise orally if asked: in David's title, "dynamo" is a symbol for the broader electrification regime. The factory mechanism we discuss is mainly about electric motors and factory redesign.
-->

---

<div class="kicker">Diffusion Lag</div>

# In 1900, electrification was still early

<div class="mt-4">
  <img src="/assets/electrification-diffusion.svg" class="diagram" />
</div>

<div class="source">David 1990 p.356; David 1989 Table 3. Lighting note: 3% of all U.S. residences, 8% of urban dwellings in 1899.</div>

<!--
This is the grounding data.

Electric lighting and central stations existed by the early 1880s. But in 1899, only about 3% of U.S. residences had electric lighting, and electric motors were less than 5% of factory mechanical drive.

I simplified the chart to one line: factory mechanical drive electrified. The original table also has a "secondary electric motor" series, but that is too technical for the main talk. In David/Duboff's usage, primary electric motors used purchased electricity from utilities; secondary electric motors used electricity generated inside the plant. Treat secondary motor penetration as a proxy for deeper factory electrification and unit-drive diffusion, not as a literal motor type.

David says these aggregate measures took roughly another two decades to reach about 50% diffusion.

So the first lesson is simple: invention is not diffusion. Diffusion is not redesign. Redesign is what eventually matters for productivity.
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

<div class="source">David 1990 p.357-358; Devine 1983. Photos: user-provided Pfaffendorf image; NARA/Wikimedia Commons PD-US.</div>

<!--
This is the most important slide.

In old factories, a central prime mover powered long overhead shafts. Belts carried mechanical power down to machines.

Early electrification often kept that architecture. A motor was added to drive sections of the old shafting system. This was group drive: new power source, old factory geometry.

Unit drive changed the architecture. Each machine could have its own motor. Power moved by wire, then became mechanical motion at the point of use.

That made single-story layouts, flexible machine placement, easier maintenance, and safer cleaner factories possible.

The photo on the right is a Marconi screw-machine department photo whose archival caption explicitly notes individual driving motors. Caveat: it is from 1917-18, so use it as a concrete visual of unit-drive machinery beginning to appear, not as the entire 1920s diffusion story.

One caveat: David's 1920s manufacturing productivity story is not only unit drive. Secondary motor capacity statistically explains about half of the 1919-1929 manufacturing TFP acceleration; continuous process production, shift-work, electrical instrumentation, and process heat also matter.
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
This is "historically contingent": not automatic, not pure luck.
</div>

<div class="source">David 1990 p.356-358.</div>

<!--
Why did the payoff become visible in the 1920s?

Not for one reason. Several conditions lined up.

Electricity became cheaper and more reliable. Old factories reached replacement moments. Engineers and factory architects learned how to design around unit drive. And the 1920s investment boom created opportunities to build new plants.

This is what "historically contingent" means in plain English: the technology did not automatically produce productivity. It needed prices, capital replacement, skills, and macro conditions to align.
-->

---

<div class="kicker">Computer Bridge</div>

# EDP had its own "group drive" phase

<div class="twocol mt-6">
  <div>
    <img src="/assets/ibm-704-edp.jpg" class="edp-photo" style="object-position:50% 48%;" />
    <div class="mt-2 tiny muted">IBM 704 electronic data processing machine, NASA Langley, 1957.</div>
  </div>
  <div>
    <div class="claim">Computerizing paper work is not the same as becoming digital-native.</div>
    <div class="mt-5 box">
      <div class="text-2xl leading-tight">
        paper forms<br/>
        + batch processing<br/>
        + manual checks<br/>
        + old departments
      </div>
    </div>
  </div>
</div>

<div class="source">David 1990 p.357, p.360; Baily & Gordon 1988. Photo: NASA / Wikimedia Commons.</div>

<!--
Now bridge back to computers.

David's real target was the computer productivity paradox. EDP means electronic data processing: enterprise systems for payroll, accounting, inventory, reports, and records.

This is not today's smartphone-cloud-SaaS world. It was centralized, expensive, back-office computing.

Many organizations did not become digital-native immediately. They layered computers onto paper workflows, with manual checking and old departmental boundaries still intact.

The computer analogy only starts to look like unit drive when the workflow itself becomes computational: databases as the source of truth, ERP and supply-chain systems, real-time inventory, CAD/CAM, networked ordering, electronic payments, search, routing, and self-service. Then the gain is not "a faster filing cabinet." It is less waiting, less re-keying, fewer errors, tighter inventories, better capacity use, faster design cycles, and new operating models.

So EDP could also be a kind of group drive: new technology bolted onto old processes.
-->

---

<div class="kicker">35 Years On</div>

# The computer payoff arrived, then faded

<div class="twocol mt-8">
  <div class="metric">
    <div class="number">1995-2004</div>
    <div class="mt-3 text-2xl font-bold">IT became visible in productivity</div>
    <div class="mt-3 small">U.S. labor productivity accelerated; growth accountants found a large IT contribution.</div>
  </div>
  <div class="metric" style="border-left-color:#64748b;">
    <div class="number" style="color:#64748b;">2005-2019</div>
    <div class="mt-3 text-2xl font-bold">The boom did not simply continue</div>
    <div class="mt-3 small">Productivity growth slowed again despite internet, smartphones, and cloud.</div>
  </div>
</div>

<div class="mt-8 claim">
So the lesson is patience, but not faith.
</div>

<div class="source">Oliner & Sichel 2000; Jorgenson, Ho & Stiroh 2008; Syverson 2017; BLS.</div>

<!--
Claude's article adds a useful "35 years on" layer.

David's delayed-payoff story did get support from the later IT boom. Around 1995-2004, U.S. nonfarm business labor productivity accelerated, and work by Oliner and Sichel attributed much of the late-1990s speed-up to IT capital deepening and productivity in computer production.

But that is not the end of the story. After the mid-2000s, productivity growth slowed again. The usual careful wording is 2005-2019, because the post-pandemic period is volatile and still being interpreted. There is a post-2022 pickup in some data, but attribution to AI is still young and contested.

This is why I do not want to say "AI will just be like electricity." The right lesson is patience, but not faith.
-->

---

<div class="kicker">AI Extension</div>

# AI may still be in its group-drive phase

<div class="mt-4">
  <img src="/assets/ai-retrofit-vs-redesign.svg" class="diagram" />
</div>

<div class="source">Analogy as lens, not prophecy. David 1990 p.360: "Computers are not dynamos."</div>

<!--
Now apply the lens to AI.

If someone says, "We see LLMs everywhere, but not in the productivity statistics," that statement is plausible as a framing. But it is not a conclusion.

It does not prove AI has failed. It also does not prove AI will succeed.

Many early AI deployments look like group drive: a chatbot next to an old workflow, Copilot inside an old IDE, summarization inside an old document process.

The bigger question is: what is AI's unit-drive moment? What does it mean to redesign task decomposition, tool access, evals, review gates, responsibility boundaries, and data flow around AI?

The evidence is strongest at the task or firm level: for example, some studies find real productivity gains in specific writing or customer-support settings. What we cannot yet say, in 2026, is that AI has caused a durable economy-wide productivity regime change.

Also mention the caveat if useful: information systems do not physically wear out like factories. Old workflows can persist for a long time unless we intentionally redesign them.
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

<div class="quote mt-9">
Are we bolting new tools onto old shafts,<br/>
or redesigning the factory?
</div>

<div class="source">Closing thesis: analogy as a thinking tool, not a forecast.</div>

<!--
The conservative close is important.

David is not saying: wait long enough and every new technology will save us.

He is saying: do not judge a general-purpose technology too quickly from early productivity numbers.

The electricity story was not really about the generator alone. It was about redesigning factories. The computer story was not just about buying computers. It was about becoming digital-native.

So for AI, or any new general-purpose tool, the question is not only "is the technology good enough?" The question is: can we redesign work around it?
-->

---
layout: end
---

# Q&A

<div class="mt-8 text-2xl">Appendix candidates: TFP 101 | Solow | electrification timeline | EDP vs PC/cloud | "Computers are not dynamos"</div>
