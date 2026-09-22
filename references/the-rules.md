# The rules

What keeps a prep honest, how the script reads out loud, and the checks before the hand-over.

## The prep

- **Numbers agree everywhere.** A number appears once, or identically every time. A picture of the viewer's life stays non-specific ("thousands of photos") so it never collides with a real number.
- **The costs.** Read each pricing page the day the prep is written. The month-to-month price, never the yearly price divided by 12. The total is the rows added. The founder's own product has no pricing page: its row reads PRICE on `squad/business.md`.
- **The comments.** Read the winner file's comments before the problem and the questions. A question is a sentence the commenter ended with a question mark, or plainly asked. Fewer than 3 usable comments: the problem comes from BUYER WORDS in `squad/business.md`, and no `[COMMENT:]` line appears. BUYER WORDS empty too: the problem is said in the winner's own words, quoted from its transcript with the time (read off the `.vtt` in the week's `src/` folder), and the script says whose words they are.
- **Length.** The minutes the founder named win. Otherwise the minutes of the winner sections the outline keeps, plus the part only the founder has. Never padded to hit a number.
- **Open items.** A missing answer on a line the video stands on (a hook number, a quote, a section's content) heads that section NOT YET A BEAT. "The prep is approved." with a NOT YET A BEAT still open: write the script on the fallback screen the prep names, and say in 1 line which beat is still open and what file closes it. A /execution-genesis-demo recording as the screen that shows the work: the script says it as "This is a demo of my <product word>, with sample data."
- **Coverage.** Only a summary of the winner, no transcript: the prep says so, and the outline shrinks to match. Pull the real transcript whenever one is reachable.
- **The close is written before the prep is done.**

## The script

- **The first sentence is the MAIN title, said out loud.**
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
- **Screens for viewers.** 00_PREP.md and squad/business.md are working files and never a [SCREEN:]. A screen the video needs that no file holds (the rubric's boxes, the buyer's words, the price) is written by this agent as <episode>/screen-<name>.md, holding only the words said, and the [SCREEN:] line names it. The prep's own notes never show on camera. A moment in someone else's video is named by its words, never a caption time: `[SCREEN: YouTube, <title>, at "<its first 5 words, verbatim>"]`. Caption files can run past the video's length, and YouTube's transcript panel finds the words.
- **Only what is said.** Past the title, the `Layer:` line and the `Words:` line, `03_SCRIPT.md` holds the `## MM:SS` headings, the 3 markers, `(pause)` and the words the founder says. No notes, no blockquotes: Cut reads every other line as a line that belongs in the edit.
- **Language.** Talking to 1 friend. 4th-grade words, 8 to 12 words a sentence, nothing past 15. First person. A setup line before each section. No idioms. Every number a numeral ($2,997, 3 steps, 90%), never spelled out. No em dashes. None of the words in `references/humanizer.md`. The product word is the `product word` row.
- **The close.** What it costs, off the costs rows. The payoff against the hook's promise. The 1 link. The next video in 1 line, only when a package or a video for it exists; none: end on the payoff. Then stop. Never signal the end early.

## The checks, before the hand-over

1. **Copy lines.** Each has its `[HOLD]` line and "Screenshot this."
2. **Questions.** Each workflow section opens on its question or its setup line. Every question is in the winner file, word for word.
3. **Screens.** Every `[SCREEN:]` line names something that exists before record.
4. **Language.** Sentence length, banned words, em dashes, numerals.
5. **Length.** The word count, `grep -v -E '^(#|>|\[|Layer:|Words:)' 03_SCRIPT.md | wc -w`, at the wpm against the prep's target. Over the target by more than 10% fails. Under it passes when check 6 passes, because a script is never padded. Every `## MM:SS` recomputed from the running count.
6. **Coverage.** Walk the winner outline. Every section is covered, or marked dropped in the prep.
7. **Word for word.** The hook, the proof line, the close and every copy line match the prep character for character. A line changed while writing goes back into the prep first.

## The 3 mistakes

- **Summarising the winner instead of covering it.** A thinner video at the same length gives nobody a reason to watch yours.
- **Forcing the body into a framework.** The cage owns the hook, the proof and the close. The winner owns the order of the body.
- **Mixing layers.** 1 layer, start to finish.
