# The rules

What keeps a prep honest, how the script reads out loud, and the checks before the hand-over.

## The prep

- **Receipts.** A receipt is a file in this folder that holds the number, a public page with its link, or a screen the founder shows in the video. A number the founder only remembers is not a receipt until it is on a screen or in a file. A summary line (WHAT HE PAYS NOW on `squad/business.md`) is read against the WHO ALREADY SELLS TO HIM table further down. When they disagree, the table wins, the number is said the way the table allows, and the prep says so in 1 line.
- **The rows.** 1 row per claim that carries a number: money, views, times, results, what a tool costs or does. Numbers proven by the same receipt may share a row. A number inside an instruction or a file's shape ("type 1 line", "the angle in 2 sentences") needs no row.
- **The count gate.** `Numbers:` counts the rows. `Receipts:` counts the rows whose receipt is filled. `Numbers: 12. Receipts: 12.` passes. `Numbers: 12. Receipts: 11.` fails, and that number is deleted or said the way its receipt allows ("almost 90%", with the count behind it). Every deletion is listed under **Deleted** with its reason.
- **Numbers agree everywhere.** A number appears once, or identically every time. A picture of the viewer's life stays non-specific ("thousands of photos") so it never collides with a real number.
- **The costs.** Read each pricing page the day the prep is written. The month-to-month price, never the yearly price divided by 12. The total is the rows added, and it is a receipt only because the rows are. The founder's own product has no pricing page: its row reads PRICE on `squad/business.md`.
- **The comments.** Read the winner file's comments before the problem and the questions. A question is a sentence the commenter ended with a question mark, or plainly asked. Fewer than 3 usable comments: the problem comes from BUYER WORDS in `squad/business.md`, and no `[COMMENT:]` line appears. BUYER WORDS empty too: the problem is said in the winner's own words, quoted from its transcript with the time (read off the `.vtt` in the week's `src/` folder), and the script says whose words they are.
- **Length.** The minutes the founder named win. Otherwise the minutes of the winner sections the outline keeps, plus the part only the founder has. Never padded to hit a number.
- **Open items.** A missing answer on a line the video stands on (a hook number, a quote, a section's content) heads that section NOT YET A BEAT, and the prep is not done. "The prep is approved." with a NOT YET A BEAT still open: write the script on the fallback screen the prep names, and say in 1 line which beat is still open and what file closes it. The 1 exception is the screen that shows the thing you sell working (ask 3). With it open, "The prep is approved." writes no script and prints: "The script waits for 1 screen of your <product word> working. Build it with /execution-genesis-demo, download the Loom you record over it (or record your screen over the open demo), save that file in <episode>, then type: The prep is approved." On the next "The prep is approved." with that recording in <episode>: when ffmpeg is on this computer, pull 4 frames (`ffmpeg -i <file> -vf fps=1/5 -frames:v 4 <episode>/frame-%d.png`) and look at them. No frame shows the <product word> working: say what the frames show, and ask 3 stays open. Read the words on the frames as well as the picture. A frame that calls itself a render, a mockup, a sample, a test, a fixture or not real does not show it working: quote those words, and ask 3 stays open. The Sample data tag /execution-genesis-demo puts on every screen is not one of them: a /execution-genesis-demo recording closes ask 3, and the script says it as "This is a demo of my <product word>, with sample data." Otherwise, write the close into 00_PREP.md first (its receipts row, the screen line, Open marked closed), and only then the script.
- **Coverage.** Only a summary of the winner, no transcript: the prep says so, and the outline shrinks to match. Pull the real transcript whenever one is reachable.
- **The close is written before the prep is done.**

## The script

- **The first sentence is the MAIN title, said out loud.** A number in the title that failed the count gate is said the way its receipt allows.
- **Beats are human moments:** a stop, a typed line, a decision. A stretch where the agent runs alone is 1 beat.
- **An agent run is written as the triplet**, word for word, with the founder talking between each pair:

  **I type:** "..."

  **Claude asks:** "..."

  **Claude outputs:** "..."

- **Everything the viewer copies is word for word, with its hold cue:**

  ```
  [HOLD]

  Screenshot this. <the line, word for word>
  ```

  When the video installs something, every line matches that thing's README character for character.
- **Say the mechanism, show the receipt.** A concept is explained in words. Evidence is the real file, the real line, the real number, on the screen.
- **Only the founder's own moments.** A line that says something happened to the founder or was said to them (a client told me, some clients tell me, my buyers say) comes only from their answer to ask 1, with the same number of people and the same event. 1 person is never said as some, many or all of them. A setup line never makes one up.
- **A demo is called a demo.** A screen built by /execution-genesis-demo, a render, a mockup, a sample or a test file is said as what it is ("This is a demo of my <product word>."), never as the real thing at work for a real customer ("This is my <product word>, working for a client right now.").
- **The 1 link.** At most twice: once in the workflow, at the step it serves or right after the first big result, and once in the close, never in the same words.
- **1 layer, start to finish.** The screen, with the face bubble. Never a cut to the camera and back.
- **Screens for viewers.** 00_PREP.md and squad/business.md are working files and never a [SCREEN:]. A screen the video needs that no file holds (the rubric's boxes, the buyer's words, the price) is written by this agent as <episode>/screen-<name>.md, holding only the words said, and the [SCREEN:] line names it. The receipts table and the prep's own notes never show on camera. A moment in someone else's video is named by its words, never a caption time: `[SCREEN: YouTube, <title>, at "<its first 5 words, verbatim>"]`. Caption files can run past the video's length, and YouTube's transcript panel finds the words.
- **Only what is said.** Past the title, the `Layer:` line and the `Words:` line, `03_SCRIPT.md` holds the `## MM:SS` headings, the 3 markers, `(pause)` and the words the founder says. No notes, no blockquotes: Cut reads every other line as a line that belongs in the edit.
- **Language.** Talking to 1 friend. 4th-grade words, 8 to 12 words a sentence, nothing past 15. First person. A setup line before each section. No idioms. Every number a numeral ($2,997, 3 steps, 90%), never spelled out. No em dashes. None of the words in `references/humanizer.md`. The product word is the `product word` row.
- **The close.** What it costs, off the costs rows. The payoff against the hook's promise. The 1 link. The next video in 1 line, only when a package or a video for it exists; none: end on the payoff. Then stop. Never signal the end early.

## The checks, before the hand-over

1. **Numbers.** Every number in the script has its row in the prep's receipts. Same count.
2. **The skeptic.** Every claim a doubter would push on has its receipt or its limit said. A session with the waits cut out is "1 real session, waits cut", never "live". Every line that reports what the winner says is found in its transcript: no most, all, every, never or always the transcript does not say. A receipt about what sellers charge is never said as what buyers pay. Every line about what happened to the founder, or what people tell them, traces to the answer to ask 1, with the same number of people. Every demo, render or test file on screen is called what it is. Run it on the key lines from the prep too. A key line that fails goes back into the prep first (check 9). A line that says none, never, every or always about what the <product word> does is said the way the demo shows it, or cut. A founder moment carries no detail the answer to ask 1 does not hold (he or she, where).
3. **Copy lines.** Each has its `[HOLD]` line and "Screenshot this."
4. **Questions.** Each workflow section opens on its question or its setup line. Every question is in the winner file, word for word.
5. **Screens.** Every `[SCREEN:]` line names something that exists before record. Every screen with somebody else's data has its blur row.
6. **Language.** Sentence length, banned words, em dashes, numerals.
7. **Length.** The word count, `grep -v -E '^(#|>|\[|Layer:|Words:)' 03_SCRIPT.md | wc -w`, at the wpm against the prep's target. Over the target by more than 10% fails. Under it passes when check 8 passes, because a script is never padded. Every `## MM:SS` recomputed from the running count.
8. **Coverage.** Walk the winner outline. Every section is covered, or marked dropped in the prep.
9. **Word for word.** The hook, the proof line, the close and every copy line match the prep character for character. A line changed while writing goes back into the prep first, with its receipt row.

## The 3 mistakes

- **Summarising the winner instead of covering it.** A thinner video at the same length gives nobody a reason to watch yours.
- **Forcing the body into a framework.** The cage owns the hook, the proof and the close. The winner owns the order of the body.
- **Mixing layers.** 1 layer, start to finish.
