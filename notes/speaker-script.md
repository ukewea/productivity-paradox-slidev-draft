# Speaker Script Draft

## Slide 1 - Opening

(Open cold. Say the quote first, before any throat-clearing.)

"We see the computers everywhere but in the productivity statistics."

中文大意:「電腦到處都看得到,就是在生產力的統計數字裡看不到。」這是經濟學家 Robert Solow 在 1980 年代末講的一句話。投資很重、大家天天用、人人都覺得它重要,但攤開總體生產力的數字,卻幾乎沒有動。

(Beat.) He said that about computers, almost forty years ago. I want to argue that the exact same sentence is being said about AI today — "we see LLMs everywhere but not in the productivity statistics" — and that a short 1990 economics paper tells us whether that should worry us.

The paper is Paul David's *The Dynamo and the Computer* — "dynamo" just means the electric generator, his shorthand for the whole electrification era. The main story is not AI. It is a historical puzzle about computers, and David's way of using electrification to understand it.

That gap — visible everywhere, invisible in the numbers — is the productivity paradox.

Near the end I will come back to AI. But the foundation is the older paradox: computers were everywhere, yet the productivity statistics looked disappointing.

## Slide 2 - The Paradox

I will skip the TFP formula. For this room, an example is enough.

So the paradox is not that the technology has no value. It is that visible adoption has not yet become clear aggregate productivity.

And there are two separate reasons the numbers can lag, and David leans on both. One is real: the value has not been built yet, because the work has not been redesigned around the tool. The other is measurement: the official statistics are partly blind — they miss quality improvements and whole categories of new output, so even real gains show up late and understated. Hold onto that measurement point; it comes back.

The right question is therefore not "is there any value?" It is: has that value become system-level productivity yet — and would our numbers even see it if it had?

## Slide 3 - David's Mirror

David's move is not "computers are literally dynamos."

He uses electrification as a historical mirror. Around 1900, the electrical age was visible. Around 1990, the computer age was visible. In both cases, the visible technology was ahead of the measured productivity payoff.

There is a timing parallel worth saying out loud — but handle it carefully, because the point is the opposite of a neat clock. In both cases the payoff arrives a long time after the enabling invention, and how long varies a lot. Edison and Swan's incandescent lamp and the first central stations appear around 1879-1881, but the factory payoff does not really land until the 1920s — by David's own reckoning roughly four decades after the first central station opened. Intel's memory chip and microprocessor appear around 1969-1970, and the computer payoff shows up in the late 1990s. So the lesson is not "expect it in twenty years." It is that the lag is long, variable — anywhere from two to four decades — and not guaranteed to arrive at all. It depends on whether the complementary conditions line up.

One vocabulary note. When I say "general-purpose technology," I mean exactly this kind of thing: a technology that spreads across the whole economy, like electricity, the computer, and maybe AI. That breadth is precisely why the payoff is slow — everyone has to rebuild around it.

## Slide 4 - Diffusion Lag

This is the grounding data. Lead with the punch number: eighteen years after the lightbulb, in 1899, only about 3% of U.S. residences had electric light — 8% even in urban dwellings — and electric motors were less than 5% of factory mechanical drive.

The chart is one line: factory mechanical drive electrified. David says these aggregate measures took roughly another two decades to reach about 50% diffusion.

(Hold this for a beat, then the lesson.) So here is the first lesson, and it is the spine of this whole talk: invention is not diffusion. Diffusion is not redesign. And redesign — actually rebuilding how the work gets done around the technology — is what eventually moves productivity. Hold onto that word "redesign"; the next slide is entirely about it.

(Appendix / only if asked.) David's table also has a "secondary electric motor" series. Primary electric motors ran on purchased electricity from utilities; secondary motors ran on electricity generated inside the plant. Treat secondary-motor penetration as a proxy for deeper factory electrification and unit-drive diffusion — not as a "second motor" or a literal one-motor-per-machine count. This is Q&A material; do not spend main-talk time on it.

## Slide 5 - Retrofit Is Not Redesign

This is the most important slide. If you remember one idea, remember this one.

Group drive kept the old mechanical factory: one central prime mover, long overhead shafts, belts dropping power down to each machine. Early electrification could just swap the prime mover and leave that architecture intact — new power source, old factory geometry.

Unit drive put a motor on each individual machine. Once power arrived by wire instead of by shaft, the whole building could be redesigned: single-story layouts, flexible machine placement, easier maintenance, better lighting, safer and cleaner floors.

Here is the part that should land for engineers. This is the same distinction we live with in software. Group drive is lift-and-shift: you move the monolith to the cloud, new infrastructure, identical architecture. Unit drive is actually re-architecting around the new primitive. Bolting a motor onto the old shaft is the same move as bolting a chatbot onto an unchanged workflow — and neither one moves the numbers much.

The right-side photo is a Marconi screw-machine department whose archival caption explicitly notes individual driving motors. Describe it carefully: it is a concrete glimpse of unit-drive machinery beginning to appear, not a claim that every factory had already converted.

(Appendix / only if asked.) David's 1920s productivity story is not only unit drive. Secondary motor capacity statistically explains about half of the 1919-1929 manufacturing TFP acceleration (David 1990, p.359); continuous-process production, shift-work, electrical instrumentation, and process heat also matter. Keep this for Q&A — saying it here only muddies the cleanest idea in the talk.

(Bridge into the next slide.) But notice the timing puzzle this sets up: unit drive existed already in the 1900s and 1910s — the Marconi photo is 1917 — yet the productivity payoff did not really land until the 1920s. The technology was available before the payoff arrived. So why the 1920s? That is the next slide.

## Slide 6 - Why The 1920s?

Why did the payoff become visible in the 1920s? Not for one reason — several conditions lined up. And each one has a direct software parallel, so this is a checklist you can apply on Monday.

Electricity got cheaper and more reliable — the tool got cheap and trustworthy enough to build on, our GPT-4-class moment. Old factories hit replacement moments — and we mostly redesign during a rewrite or a migration, not mid-flight. Factory architects learned to design around electric drive — someone has to actually learn the new architecture; it is a skill, not a switch. And the 1920s capital boom funded new plants — leadership has to fund the redesign.

This is what "historically contingent" means in plain English: the technology did not automatically produce productivity. It needed prices, capital-replacement moments, skills, and macro conditions to line up. And the crucial word is contingent — these conditions happened to align in the 1920s, but they might not have. There was no guarantee. A different macro climate could have deferred the payoff another decade or two — and remember what actually followed the 1920s. David's argument explicitly includes the possibility that the gains arrive far later than expected, or never on the schedule people hope for. So this is not "be patient and it always pays off." It is "it pays off only if the conditions align — and they may not."

## Slide 7 - Banking: three waves of tech

David's real target was not the factory — it was the computer productivity paradox. The cleanest place to watch it is one industry we all use: banking. Three waves of technology, three very different effects on jobs.

Wave one, the 1960s and 70s: banks computerize the back office. Records go digital, bookkeeping speeds up — but you still drive to the branch, and a teller still serves you. The computer made the old way faster; it did not change who does the work. Teller numbers barely move.

Wave two, the ATM, from the 1970s on. A cash machine extends the bank's reach, and it cut the number of tellers needed per branch — from about twenty to thirteen between 1988 and 2004. But here is the twist economists love: because the ATM made each branch cheaper to run, and because convenience back then meant being physically close to customers, banks opened about forty percent more branches. Fewer tellers per branch, times many more branches, means total tellers actually rose — from roughly three hundred thousand in 1970 to about six hundred thousand by 2010. The machine everyone expected to kill the teller grew the teller.

Wave three, mobile banking, in the 2010s. Now the bank moves into your phone, and travel distance drops to essentially zero. Suddenly the branch is not a competitive weapon, it is a cost. Banks start closing branches — US branch counts peaked in 2009 — and teller numbers finally fall, into the mid-three-hundred-thousands by the early 2020s. Be fair here: mergers after the 2008 crisis and falling cash use pushed in the same direction, not mobile alone.

Here is the punchline, and it is the whole talk in one line: for forty years the technology made banking cheaper without cutting the workforce. The jobs only moved when the model itself changed. A new tool makes the old model efficient; only a new model changes the work.

And one David-flavored footnote: why did mobile banking land only in the 2010s, when phone banking existed back in the late 1990s? Because the complements had to line up — the smartphone and app store in 2007 and 2008, fast mobile internet with 4G in 2010, and the underrated one: a 2004 law, Check 21, that made depositing a check by photo legal in the first place. The idea was old; the payoff was historically contingent, exactly like the dynamo waiting for the 1920s.

(Bridge to AI:) So hold that one question for AI: are we adding a new tool to the old model, or are we building a new model?

## Slide 8 - Computer Payoff

With hindsight, the computer story did get its payoff — and the numbers line up with David's framework, rather than vindicating a forecast he never made. He argued conditionally: if the redesign happens, the gains eventually register, and the statistics under-measure them along the way. That is what we see.

First, the lag, in hard data. Through the early 1990s, U.S. business computer-hardware stock was growing about 17% a year, and investment in computers more than quadrupled after 1995 — yet computers added only about a quarter of a percentage point to annual growth, because they were still a tiny share of the capital stock. Adoption everywhere, payoff missing. That is David's electrification curve, repeated.

Then it landed. Oliner and Sichel found nonfarm-business labor productivity accelerated from about 1.6% a year in the first half of the 1990s to about 2.7% in the second half. IT capital deepening accounted for roughly half of that step-up; computer hardware's own contribution rose from about a quarter point to about 0.6 of a point a year. All told, the use of IT plus computer production explains about two-thirds of the acceleration.

But it did not simply continue. From 2005 to 2019, growth slowed again despite the internet, smartphones, and cloud. And say this carefully, because it matters for the AI section in a minute: what faded was the redesign, not the technology. The silicon kept getting better — what ran out was the wave of complementary reorganization that turned it into measured productivity. The payoff is contingent, not permanent. (There is a post-2022 pickup in some series; I am not attributing that to AI — too young to call.)

So the lesson is two words: patience, but not faith. The payoff can be delayed, partial, or temporary — it is not a guarantee that arrives if you just wait.

## Slide 9 - AI Extension

Now apply the lens to AI. I am going to put a sharp claim on the table — but as a provocation, not a verdict, because the honest truth is we are standing inside the transition and cannot yet measure it.

The claim, stated sharply so you can argue with it: most of what we have built with LLMs so far looks like group drive. A chatbot bolted onto an old workflow. Copilot autocompleting inside the same IDE, the same review process, the same PR ritual — you type less, but the workflow is unchanged. A RAG bot in front of a knowledge base nobody reorganized. New power source, old factory geometry.

But here is the caution David forces on us, and I want to honor it. From inside a transition you genuinely cannot tell early redesign from retrofit. That 1917 unit-drive photo looked like nothing in the aggregate statistics at the time. So "most AI is group drive" is a question to hold against your own work, not a confident diagnosis of the industry. That observation does not prove AI has failed, and it does not prove it will succeed. The evidence today is strongest at the task or firm level — real, measured gains in specific writing and customer-support settings. What we cannot yet say, in 2026, is that AI has caused a durable, economy-wide productivity regime change.

So here is the question that matters: what is AI's unit-drive moment? Let me give concrete candidates and you can argue with me. One: an agent owns an end-to-end slice of work, instead of a sub-step a human stitches back together. Two: evals and tests become the source of truth, the way the database became the source of truth in the computer's unit-drive era. Three: review gates, accountability, and responsibility boundaries get redesigned — who is on the hook when the agent ships? That is an org-chart change, not a tooling change, exactly like single-story factory layouts followed from unit drive. Four: pipelines designed assuming a probabilistic component — retries, verification, fallback — instead of a deterministic one bolted in.

Let me make this concrete with real, measured cases — and one cautionary tale. Group drive: a Fortune-500 support center gave about five thousand agents an AI assistant that sits beside them in the existing queue. Measured result — roughly 14% more issues resolved per hour, and 34% for the newest agents (Brynjolfsson, Li and Raymond, 2023). That is real and valuable, but it is a tool laid over an unchanged workflow. It is group drive, and it is the strongest evidence we have. Unit drive: Klarna went further and rebuilt its whole tier-one queue around an AI agent in 2024 — it handled about two-thirds of chats and cut resolution from eleven minutes to under two. That is redesigning the work and the org. But here is the honest twist, and it is pure David: by 2025 Klarna walked it back and re-hired humans, with the CEO saying they had over-rotated on cost and quality suffered. From inside the transition, they could not yet tell good redesign from cutting too deep. So unit drive is the goal — but it is hard, and you cannot tell from inside whether you have got it right. Most "we added an AI assistant" projects, meanwhile, are not even attempting the redesign.

A test you can use: if your AI rollout did not change your org chart or your definition of done, you built group drive.

And one structural warning that is David's own sharpest point. Factories got redesigned partly because the old ones physically wore out and had to be replaced — that replacement moment forced the redesign. Information systems and workflows do not wear out. A 2009 process can run untouched for fifteen years. So nothing forces the AI rewrite. The unit-drive moment may be structurally slower for AI than it was for electricity, precisely because decay will not do the work for us.

(Optional interaction.) Ask the room: name one thing your team does differently because of AI — not faster, differently. The silence, or the rare good answer, is the most persuasive evidence in this whole talk.

## Slide 10 - Close

The close is conservative, but it should still have teeth.

David is not saying "wait long enough and every new technology will save us." He is saying: do not judge a general-purpose technology too quickly from early productivity numbers. The electricity story was never about the generator alone — it was about redesigning factories. The computer story was never about buying computers — it was about becoming digital-native.

So for AI, the question is not only "is the technology good enough?" It is "can we redesign work around it?" — and then the sharper version, the one I want you to leave with:

Factories got redesigned because the old ones fell apart. Your codebase won't. Nothing will force the AI rewrite except you — so the only question that matters is whether you will do it on purpose.

(Land the slide's line, then stop.) Are we bolting new tools onto old shafts, or redesigning the factory?

## Q&A / Appendix

Pre-load a few questions you actually want asked, so the discussion goes where the good material is:

- TFP / MFP 101 — what "total factor productivity" means, and why I avoided the formula on stage.
- The Solow quote — provenance and the canonical wording ("We can see the computer age everywhere but in the productivity statistics").
- Electrification timeline — primary vs. secondary motors, the 50% diffusion lag, the 1919-1929 TFP decomposition (≈half from secondary motor capacity, David 1990 p.359).
- EDP vs. PC vs. cloud/SaaS — why the early-computer era is the right analogy, not the smartphone era.
- "Computers are not dynamos" (David 1990, p.360) — David's own warning against pushing the analogy too far; useful if someone accuses me of over-fitting electricity onto AI.
- The strongest objection to invite: information systems do not physically depreciate, so the redesign may never be forced — is that a reason for optimism or pessimism about AI's payoff?
