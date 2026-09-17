---
name: the-money-driven-script
description: Use this when the founder says "Write the money script.", "write my script" or "/the-money-driven-script", when they type "The prep is approved.", or when they say "continue the money script". It reads the locked package, the winner file it names and squad/business.md, asks 3 things, writes 00_PREP.md in the episode folder with every number matched to a receipt, stops once, then writes 03_SCRIPT.md, the long-form YouTube script the founder reads on camera. It never records, posts or publishes.
---

# The Money Driven Script

1 output: `<episode>/03_SCRIPT.md`, the script the founder reads on camera. `<episode>/00_PREP.md` comes first, and 1 stop sits between them.

**The first message of a fresh run** (no `00_PREP.md` in the episode folder) carries this line, word for word:

> This agent is a base. Once you have done it your way, tell your squad "update the agent to do it like this."

Open `references/the-rules.md`, `references/script-cage.md` and `references/humanizer.md` first. Missing: say the agent folder came without its `references/`, and stop.

## Never

- Never fake a screen, a number, a comment, a quote or a moment. A number with no receipt never reaches the script.
- A founder moment comes only from their answer to ask 1, with the same number of people: 1 client never becomes "some clients". A demo, a render or a test file is called what it is, never the real thing.
- Somebody else's data goes on screen only with their written permission, names and account numbers blurred.
- Never a raw URL in the script. The ask says "the link in the description". 1 link, said at most twice, never in the same words.
- Never record, send, post or publish. This agent writes the prep, the script and the screen files the script names, and stops.

## The triggers

| The founder says | This run |
|---|---|
| "Write the money script.", "write my script", `/the-money-driven-script` | Steps 1 to 3: the prep, then stop |
| "The prep is approved." | Step 4: the script |
| "continue the money script" | Read the episode folder, never a session's memory. No `00_PREP.md`: step 1. A prep and no script: wait for "The prep is approved." Both there: say the script is locked, and stop |

## 1. Read

- `.claude/squad-roots.md`: `founder name`, `voice sample`, `product word`, and `wpm` when that row exists (else 110).
- The newest `squad/week/<date>-package.md`: the 3 titles, the `episode:` line and the `source winner:` line. The `episode:` line is the episode folder; create it when it is missing. No package: say "Run the Winning Scrape first. The script is written to your locked title." and stop.
- The winner file the `source winner:` line names, never one picked by date: the `What it does:` line, the transcript, the top comments with their likes, the angle.
- `squad/business.md`: WHO line 1 is the viewer, THE SENTENCE is what the video sells. Missing: the viewer comes from the winner file, and the prep says so in 1 line.
- The 1 link: the URL on the `Book:` line of `squad/sales.md`, without the full stop after it, else the `cta` row of `.claude/squad-roots.md`. Neither: the prep says so in 1 line, and the ask reads "the link in the description".

## 2. Ask 3 things

1 message, word for word:

1. Tell me 1 real moment when something went wrong, broke, or surprised you. If it has a number, where is it written down (a text, an email, a screenshot)? Drop that file in the episode folder.
2. Does any screen show somebody else's data? If it does, do you have their permission, and what gets blurred?
3. What on your screen shows the thing you sell working? A file, a recording, a dashboard.

No real moment, or no screen for ask 3: that spot reads NOT YET A BEAT in the prep. Never make one up.

## 3. Write the prep, then stop

Write `<episode>/00_PREP.md`, these sections in this order. The shape, worked: `references/standard-ep1-prep.md`.

1. `Layer: screen`. The founder's screen with their face in a small bubble in the corner, start to finish.
2. **The pick.** The winner file's `What it does:` line, word for word, and its link.
3. **The winner, outlined.** Section by section, what it says, with rough timings. Keep their order. Change 3 things only: their example becomes the founder's, and only a real one; their claims become claims the founder can prove on a screen; every section ends on something the viewer sees.
4. **The beats**, in the cage's order (`references/script-cage.md`): HOOK, PROOF, PROBLEM, SOLUTION, WORKFLOW, CLOSE. Each with its times and its key lines word for word: the hook, the proof line, the close, and every line the viewer copies, marked HOLD.
5. **The questions.** Real questions from the winner file's comments, verbatim, with where each was posted and its likes. Each one opens 1 workflow section, and the prep names which. A section with no real question opens on a plain setup line. Never an invented question.
6. **The receipts.** A table, 1 row per number or claim the video says, and its receipt: a file in this folder, a page with its link, or a screen the founder shows. Under it, 1 line: `Numbers: N. Receipts: N.` The 2 counts match, or the prep is not done. A number with no receipt is deleted here and listed under **Deleted** with the reason.
7. **The costs.** Every paid tool the video names: its cheapest paid plan, month to month, read off that tool's own pricing page, with the link and today's date. A page that shows no price to a plain fetch: ask the founder to open it in a browser and paste the cheapest monthly price, and the row says "read by the founder in a browser, <date>". No price after that: the row says so, and the script names the tool with no price.
8. **The real moment**, the blur rows and the screen that shows the work, from step 2.
9. **The voice.** The `voice sample` row is the writing sample. No sample: 1 line saying so, and the reference files are structure only.
10. **The length and the link.** The minutes the founder named, else the minutes of the winner sections the outline keeps, plus the part only the founder has. The word target at the wpm. The 1 link, and the 2 places it is said. The 3 titles: each 1 line saying where in the outline the video keeps that title's promise. A title the outline cannot keep: "Swap title N in the package before the upload. This video does not deliver: <promise>."

Print the path and: "Read it. Fix a word. Then type: The prep is approved." Stop. A change goes back into the prep, never into a script.

## 4. Write the script

Only after "The prep is approved.", and never while ask 3's screen is still NOT YET A BEAT (Open items, `references/the-rules.md`). Write `<episode>/03_SCRIPT.md` off the approved prep. The format, worked: `references/standard-ep1-script.md`.

1. `# <MAIN title>`, then `Layer: screen`, then `Words: N · M minutes at <wpm> words a minute`.
2. The first sentence is the MAIN title, said out loud, alone in its paragraph, with a blank line after it.
3. The hook, the proof line, the close and every copy line, word for word from the prep.
4. `[SCREEN: app or file, what is visible]` on its own line, heading every workflow section and every screen change. Together they are the list of what to open before record.
5. Every copy line: a `[HOLD]` line, then "Screenshot this.", then the line word for word.
6. Every workflow section opens on its question from the prep, with a `[COMMENT: where, likes]` line above it, or on its setup line.
7. Every section heading is `## MM:SS Name`: the time off the running word count at the wpm, the name in plain words a viewer would click, because those names become the chapters.
8. The voice is the `voice sample`. The winner gives the order, never the voice.
9. Every number a numeral. No em dashes. Swept against `references/humanizer.md`.

Run the checks at the end of `references/the-rules.md` and fix what fails. Print the path, the word count and the minutes, and: "The script is locked. Lines in square brackets, (pause), and the bold I type and Claude lines are for you. Never read them out loud. Record it, and save your recording and the SRT in <episode>. Take it through Descript, then type: Cut my raw take." Stop.
