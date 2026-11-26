# eli3-until-i-understand 🍼

**ELI3 until I understand** — not just simpler words, but explaining until the logic actually clicks.

## Wait, isn't ELI5 already a thing?

Yes. And it's great at one thing: turning hard words into easy words.

But here's what I kept running into as a developer:

> I could read every sentence of the ELI5 explanation.
> I still didn't understand *why* any of it worked.

That's the gap. **Readable is not the same as understandable.**

A typical ELI5 answer for "What is WebGPU?" looks like this:

> "WebGPU lets websites use your graphics card to draw things and do math really fast."

Every word is simple. But a beginner's brain immediately fills up with questions:

- What does a graphics card actually do that the normal processor can't?
- Couldn't websites already use it before?
- If they could, why did we need something new?

ELI5 swapped the vocabulary, but it skipped the **chain of reasons**. Without that chain, you just memorize a sentence. You don't understand anything.

## Why a developer still needs ELI3

Being a developer doesn't mean you know every field. Every week there's a new thing to learn: WebGPU, Docker, vector databases, CRDTs, zero-knowledge proofs...

When you step into a new field, you're a beginner again. Here's what usually goes wrong with ELI5 at that point:

1. **It explains *what*, not *why*.** You learn the definition, but not the problem it was born to solve.
2. **It skips prerequisite concepts.** It assumes you already know the background, and that hidden gap is exactly where you get stuck.
3. **It keeps switching analogies.** Pizza in one paragraph, highways in the next. Your brain has to rebuild the picture every time.
4. **It stops after one answer.** You still don't get it, but the explanation is "done."

As developers, we don't just want to *repeat* the explanation. We want to be able to **reason with it**: make decisions, debug, and know when to use a tool and when not to. That needs the logic, not just the vocabulary.

## The ELI3 rules

ELI3 is "even younger than five" — the explanation is allowed to slow down, go back, and fill in the basics without being embarrassed about it.

1. **Problem first.** What pain existed before this thing?
2. **Where the old way got stuck.** Why couldn't the existing solution handle it?
3. **Then the new thing.** How does it fix exactly that pain?
4. **So what?** What can we do now that we couldn't before?
5. **Prerequisites first.** If a concept is needed to understand the next step, explain it *before* that step.
6. **One analogy, all the way through.** Pick one picture and stick with it.
7. **Until I understand.** If it still doesn't click, keep going. Don't stop at "done."

## Example: WebGPU in ELI3 (short version)

Your computer has two brains. The **CPU** is a genius professor: solves anything, but only a few problems at a time. The **GPU** is a classroom of thousands of kids: each one only knows simple math, but they all work at the same time.

Your screen has millions of dots, redrawn 60 times a second. Each dot needs a simple "what color am I?" calculation. That's perfect for the classroom of kids. AI works the same way: tons of simple multiplications.

But a website is code written by strangers, so the browser can't let it walk into the classroom directly. It has to fill out a form at the **front desk**, and the desk checks it first.

The old front desk (**WebGL**) was designed when GPUs were only for drawing. It only accepted "please draw this" forms. Want the kids to do AI math? You had to disguise your numbers as colors, draw them, then read them back. And the desk checked every single form one by one, so most of the time was spent waiting in line.

**WebGPU** is the new front desk, designed for how modern GPUs actually work:
- You can directly say "please calculate these numbers" — no disguising.
- You can hand over a whole stack of forms at once, checked one time.

**So what?** Websites can now run AI models on your own machine, play real 3D games, and edit video right in the browser.

The whole chain:
screens and AI need tons of simple math → GPUs are great at that → websites must go through the browser's front desk for safety → the old desk only understood drawing and was slow → the new desk understands math and accepts batches → websites can do much more.

## Status

🚧 Work in progress. Coming next: a `/eli3` skill for Claude Code, so you can type `/eli3 <topic>` and get explanations that follow these rules automatically.
