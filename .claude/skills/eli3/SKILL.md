---
name: eli3
description: Explain a topic so a total beginner actually understands the logic, not just the words. Builds a chain of reasons (problem → where the old way got stuck → the new thing → so what), fills in prerequisite concepts first, and sticks to one analogy. Use when the user types /eli3 <topic> or says they can read an explanation but still don't get why it works.
argument-hint: <topic>
---

# ELI3 — until I understand

Explain **$ARGUMENTS** to someone who has never touched this field.

The goal is not "simple words". The goal is that the reader can follow the **chain of reasons** and could re-explain it, make a decision with it, or spot when it doesn't apply.

If no topic was given, ask what they want explained and stop.

## Before you write

Quietly answer these for yourself (don't print them):

1. What problem was this thing born to solve?
2. What did people use before, and exactly where did that get stuck?
3. What concepts does a beginner need *before* step 1 makes sense? (These are the hidden gaps where ELI5 usually loses people.)
4. Which **one** everyday analogy can carry the whole explanation from start to finish?

## How to write it

Walk through these steps in order. Each step should be short and build directly on the one before it.

1. **Prerequisites first.** Introduce only the background concepts the reader needs, using the chosen analogy. Skip anything they don't need.
2. **The problem.** What pain existed? Make it concrete.
3. **Where the old way got stuck.** Why couldn't the existing solution handle it? Be specific about the limitation.
4. **The new thing.** How does it fix *exactly* that limitation? Connect each change back to a pain from step 3.
5. **So what?** What can people do now that they couldn't before?
6. **The chain.** End with one line that links every step with arrows, e.g. `A needs B → B was blocked by C → D removes C → now we can E`.

## Rules

- **One analogy, all the way through.** Never switch pictures halfway. If the analogy breaks at some point, say so honestly instead of swapping to a new one.
- **Every step answers "why?"**, not just "what?".
- **Introduce each concept before you use it.** Never use a term the reader hasn't met yet.
- **Use the real names too.** After the analogy lands, mention the real term once (e.g. "the front desk — this is what WebGL is") so the reader can search it later.
- **No jargon walls, no tables, no heavy formatting.** Short paragraphs, plain talk.
- **Answer in the user's language.**
- **Be honest about limits.** If something is simplified, say "this is a simplification" in one short line.

## Until I understand

Finish by asking which step didn't click, naming the steps briefly so it's easy to point at one.

When the user says a step is unclear:

- Re-explain **only that step**, slower, with the **same analogy**.
- Look for a missing prerequisite behind it and fill that in first.
- Don't repeat the whole explanation, and don't just reword the same sentences.
- Keep going until they say it clicks.
