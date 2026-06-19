# Speaker Script — 10-Minute Cut

Target: **~10 minutes, main deck only** (Q&A is separate). Delivered in **Mandarin**; this English text is the content to translate. ~1,250 words ≈ ~8:40 spoken + pauses/translation drag ≈ ~9:20. Rehearse the **Chinese** to a stopwatch once it's translated.

Thesis (unchanged, cautious): **the payoff is real but late and contingent — patience, but not faith.** Plain language; the "group drive / unit drive" terms appear **once** (Slide 5), then become "bolt-on vs. re-architect."

The full/rich script (with all the data, Klarna detail, candidates, economist range) stays in `speaker-script.md` and the appendix slides — that's your Q&A arsenal.

---

## Slide 1 — Hook · 0:45

(Open cold. Say the quote first.)

"We see the computers everywhere but in the productivity statistics." Robert Solow said that about computers, almost forty years ago. Today we'd say the same about AI: we see it everywhere — except in the productivity numbers.

That gap is the **productivity paradox**. And a short 1990 paper by Paul David — *The Dynamo and the Computer* — explains why powerful technologies so often pay off late, and what finally makes them pay off.

---

## Slide 2 — The paradox · 0:50

The paradox is not "the technology is useless." It's that **real value hasn't yet become real productivity.**

And there are two reasons the numbers can lag — David leans on both. One: the work hasn't been redesigned around the tool yet. Two: the official statistics are partly *blind* — they miss quality gains and whole new kinds of output, so even real gains show up late and understated. Hold onto that second one.

So the question isn't "is there value?" It's: **has that value become system-level productivity yet — and would our numbers even see it?**

---

## Slide 3 — David's mirror · 0:50

David's move: use **electrification** as a mirror for the computer age. Around 1900, electricity was visible everywhere — lights, motors, generators — but the productivity payoff hadn't really arrived. Around 1990, computers were everywhere — and the numbers still looked disappointing.

One caution, because it's the whole point: the lag is **long, variable, and not guaranteed.** Electricity's factory payoff came roughly *four decades* after electric light first arrived — and it landed only because the right conditions eventually lined up, which they might not have.

---

## Slide 4 — Diffusion lag · 0:45

Here's the grounding fact. The light bulb arrives around 1879. Yet in 1899 — twenty years later — under 5% of factory mechanical power was electric. Factory electrification didn't cross ~50% until about 1919, and the real productivity payoff came in the **1920s**.

So the first lesson, in three steps: **invention is not diffusion; diffusion is not redesign; and redesign is what finally moves productivity.**

---

## Slide 5 — Retrofit is not redesign · 1:30  (CENTERPIECE)

This is the most important idea. If you remember one thing, remember this.

(Left photo.) Old factories ran on **group drive**: one big steam engine turned a long overhead shaft down the length of the building, and leather belts dropped power to each machine. Every machine was mechanically chained to that one spinning shaft.

Now the key part. When electricity arrived, the obvious move was to pull out the steam engine and bolt one big electric motor onto the same shaft — and it **barely helped.** Why? Because what held the factory back was never the engine; it was the shaft. With one shaft: the whole line has to spin all day even if a single machine is working, bleeding power to friction; machines have to sit in a row near the shaft, not in the order the work flows; they can't run at different speeds; and one breakdown stops everyone. Swapping the engine changed the *power source* and left every one of those constraints in place.

(Right photo.) **Unit drive** threw the shaft away: a motor on each machine, fed by wire. Now a machine runs only when it's needed; you lay the floor out by how the work actually flows; each runs at its own speed; a breakdown is isolated; and with nothing spinning overhead you get single-story plants, cranes, daylight, clean and safe floors. *That's* where productivity jumped — not from the motor, but from the redesign the motor finally allowed.

So the lesson: the payoff didn't come from the new power source; it came from redesigning the work once the old constraint was gone. And the line to carry for the rest of the talk — **bolting a motor onto the old shaft is the same move as bolting a chatbot onto an unchanged workflow.** You've changed the engine, not the constraints.

---

## Slide 6 — Why the 1920s · 0:30

Why did the payoff finally land in the 1920s? Several things had to line up at once: power got cheap and reliable, old plants hit replacement moments, engineers learned to design *around* electricity, and the capital was there to build new factories. That's what "historically contingent" means — it didn't happen automatically, and it might not have happened at all.

---

## Slide 7 — The computer payoff · 1:05

Now fast-forward. With computers, the same shape repeats. Through the early 1990s, business computer power was growing ~17% a year — huge adoption — yet it added almost nothing to measured growth. Adoption everywhere, payoff missing. David's curve, again.

Then it landed: from the late 1990s to about 2004, US labor productivity accelerated from about 1.6% to 2.7% a year, and IT was about half of that jump. The delayed payoff was real.

But it didn't last. From 2005 to 2019 growth slowed again, despite the internet, smartphones, and the cloud — and the honest reading is that the *redesign* stalled, not the technology. So the lesson is two words: **patience, but not faith.** (If pressed: serious economists who've modeled AI disagree by more than 10× on its payoff — nobody credible says zero, nobody credible has it confirmed.)

---

## Slide 8 — AI today · 1:30

Now apply the lens to AI — as a question, not a forecast, because we're inside the transition and can't yet measure it. And let's make it about us — gently; this is a sharing, not a report card. We run **opencode** in the terminal against our own **on-prem model.**

The honest picture: like almost everyone right now, we're mostly in the **bolt-on** phase. The agent writes and edits code faster, but it still goes through the same repo, the same pull request, the same review, the same definition of "done." That's real and useful — studies find double-digit speedups — and it's exactly where you'd expect to start. The 1920s factory first just swapped the engine, too. It's step one, not a mistake.

The fun question is what **step two — the re-architect version — looks like:** the agent owns a *ticket* end-to-end, not a snippet; your tests and CI become the gate it has to pass; and you rethink who reviews an agent's pull request and who's accountable when its code ships.

And here's the part our setup is genuinely built for: because the model is **on-prem**, we can close a learning loop a SaaS Copilot can't — capture our own code and review traces, build private evals on our codebase, even tune the model on our repo, so it gets better at *our* system over time. That's the real prize of running it in-house.

So, as a friendly self-check — not a scorecard: has AI changed our org chart or our definition of "done" yet? If not yet, that's completely normal — and the interesting question is what our re-architect moment could be.

And one honest beat: from inside, you can't yet tell good redesign from cutting too deep. Klarna rebuilt its support around AI in 2024 — then re-hired people in 2025.

---

## Slide 9 — Close · 0:55

David is not saying "wait long enough and every technology saves you." He's saying: don't judge a general-purpose technology too early from the numbers — electricity wasn't about generators, it was about redesigning factories; computers weren't about buying machines, it was about becoming digital-native.

And here's the sharpest difference, the note to end on: factories got redesigned partly because the old ones physically *wore out*. **Your codebase won't.** Nothing forces the AI rewrite except you.

So the question isn't "is AI good enough?" It's: **are we bolting new tools onto old shafts — or redesigning the factory?**

---

## Time budget

| Slide | Beat | Target |
|---|---|---|
| 1 | Hook | 0:45 |
| 2 | Paradox (+ measurement) | 0:50 |
| 3 | David's mirror | 0:50 |
| 4 | Diffusion lag | 0:45 |
| 5 | Retrofit ≠ redesign (CENTERPIECE) | 1:30 |
| 6 | Why the 1920s | 0:30 |
| 7 | Computer payoff (+ economist range) | 1:05 |
| 8 | AI today (test + 1 Klarna line) | 1:30 |
| 9 | Close | 0:55 |
| | **Total** | **~8:40 + buffer ≈ 9:20** |

Cut to Q&A (already built as appendix slides): banking three-wave, supermarket/paperless, electricity-price chart, three-tech diffusion chart, economists-disagree card, Nadella's "learning loop," TFP 101, primary/secondary motors, the four unit-drive candidates, the Klarna numbers, the "can't tell from inside" epistemics.
