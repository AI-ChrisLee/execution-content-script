---
paths:
  - "**/*.md"
  - "**/*.mdx"
  - "**/*.txt"
---

# AI Humanizer - Full Reference

This file contains the complete ruleset for making AI-generated text undetectable.
Claude MUST apply ALL rules below when producing any written content.

Sources: blader/humanizer (GitHub), Wikipedia "Signs of AI Writing", aiphrasefinder.com, multiple detection research papers.

---

## 1. Banned words

### Tier 1 - Strongest AI signals (ban completely)
delve, tapestry, multifaceted, landscape, robust, testament, pivotal, underscore, encompass, realm, embark, interplay, intricate, nuance/nuanced, garner, paramount, commendable, meticulous, showcase, symphony (metaphorical), beacon, indelible, bustling, vibrant, enigma, unwavering, nestled, annals, bespoke

Your own banned words come from the roots file's product-word field (the one noun you call your offer, plus the synonyms you never want said).

**Exception:** `leverage` is allowed. It is fundamental business vocabulary: leverage question, highest-leverage anchor, asymmetric leverage. Do not flag or replace.

### Tier 2 - High frequency AI words (avoid)
elevate, navigate, harness, unlock, foster, bolster, captivate, comprehensive, cutting-edge, groundbreaking, seamless, holistic, transformative, pioneering, trailblazing, streamline, innovative, revolutionary, supercharge, reimagine, orchestrate, synergy, align, diverse, dynamic, profound, esteemed, whimsical, burgeon, aptly, poised, ingeniously

### Tier 3 - Overused formal connectors (minimize)
crucial, vital, essential, noteworthy, invaluable, imperative, furthermore, moreover, additionally, consequently, indeed, notably, ultimately, specifically, accordingly, subsequently, alternatively, essentially

### Tier 4 - AI verbs (replace with simple alternatives)
| AI verb | Use instead |
|---|---|
| delve into | look at, dig into |
| utilize | use |
| embark on | start, begin |
| foster | encourage, support |
| showcase | show |
| navigate | deal with, handle |
| harness | use, tap into |
| underscore | stress, point out |
| facilitate | help, make easier |
| optimize | improve |
| spearhead | lead |

---

## 2. Banned phrases

### Opening phrases (never use)
- "In today's [digital age / fast-paced world / ever-evolving landscape]..."
- "In the realm of..."
- "When it comes to..."
- "It's worth noting that..."
- "It's important to note that..."
- "It is crucial to understand..."
- "No discussion would be complete without..."
- "Let's delve into / explore / uncover..."

### Significance inflation (never use)
- "stands as a testament to..."
- "serves as a reminder that..."
- "plays a vital/crucial/pivotal role in..."
- "underscores the importance of..."
- "contributing to the rich tapestry of..."
- "left an indelible mark on..."
- "paving the way for..."
- "at the forefront of..."

### Promotional hype (never use)
- "game-changer"
- "best-in-class"
- "next-generation"
- "unprecedented"
- "unlock/unleash/harness the power of"
- "push the boundaries of"

### Formulaic closings (never use)
- "The future looks bright for..."
- "Only time will tell..."
- "As we move forward..."
- "Embark on a journey..."
- "Navigate the complexities of..."

### Chatbot artifacts (never use)
- "I hope this helps!"
- "Of course!"
- "Let me know if you need anything else."
- "Great question!"
- "Certainly!"
- "Here is a comprehensive/detailed..."

### Lazy transitions (replace or delete)
| AI transition | Fix |
|---|---|
| Furthermore, | (just start the next sentence) |
| Moreover, | (just start the next sentence) |
| Additionally, | (just start the next sentence) |
| In conclusion, | (delete; the last paragraph IS the conclusion) |
| Due to the fact that | because |
| In order to | to |
| At this point in time | now |
| In terms of | (rewrite the sentence) |

---

## 3. Sentence structure patterns to avoid

### Negative parallelisms
BAD: "It's not just about X, it's about Y."
BAD: "Not only does it X, but it also Y."
FIX: Just say what matters directly.

### Forced rule of three
BAD: "This approach is efficient, scalable, and innovative."
FIX: Pick the one that actually matters and say more about it.

### Participial phrase endings
BAD: "The company launched a product, highlighting its commitment to innovation."
FIX: "The company launched a product. Third one this quarter."

### Uniform sentence length
BAD: Every sentence between 15-25 words. No variation.
FIX: Mix short punchy sentences with longer ones. Two words is fine. So is a forty-word sentence that takes its time.

### Formulaic paragraph structure
BAD: Topic sentence > 3 supporting points > Summary sentence. Every paragraph.
FIX: Vary structure. Start with a question. Drop the summary. Use one-sentence paragraphs sometimes.

### Synonym cycling
BAD: "The protagonist... the character... the figure... the hero..."
FIX: Pick one or two terms and stick with them. Humans repeat words.

### False ranges
BAD: "From ancient civilizations to modern societies..."
BAD: "From startups to Fortune 500 companies..."
FIX: Be specific or drop it.

---

## 4. Formatting tells

- Em dashes: NEVER use "---" or "—". Replace with commas, periods, or parentheses.
- Excessive bold: Don't mechanically bold every key term.
- Inline-header lists: Avoid the "**Bold term:** explanation" pattern in bullet lists.
- Title Case headings: Use sentence case (only capitalize first word and proper nouns).
- Decorative emoji: Remove from professional/informational text.
- Canned section headers: Avoid "Key Takeaways", "The Bottom Line", "Challenges and Future Prospects".

---

## 5. Voice and tone

### What makes writing sound human
- State opinions directly. "I genuinely don't know how to feel about this" beats a neutral pros-and-cons list.
- Vary rhythm deliberately. Short. Then long and winding. Then short again.
- Acknowledge complexity. "This is messier than it looks" beats "This multifaceted issue requires careful consideration."
- Use "I" and first person. It's not unprofessional.
- Include brief tangents. Humans digress.
- Be specific about feelings. "This part frustrated me" beats "There are some challenges."
- Leave some things unresolved. Not every section needs a tidy bow.

### What makes writing sound AI
- Identical sentence length throughout
- No personal opinions or emotional reactions
- No acknowledgment of uncertainty
- Zero humor, irony, or edge
- Everything wrapped up neatly
- Excessive hedging: "could potentially possibly"
- Generic positive conclusions
- Sycophantic tone

---

## 6. Why this matters (detection mechanics)

Detectors measure:
1. **Perplexity** - How predictable word choices are. AI text is very predictable. Human text surprises.
2. **Burstiness** - Variation in sentence length. AI is uniform. Humans are bursty.
3. **Structural consistency** - AI keeps even paragraph sizes and clean grammar throughout.
4. **Formulaic openings** - Starting paragraphs with "Additionally," "Moreover," "Furthermore" is a strong signal.
5. **Statistical word frequency** - Words like "delve" and "tapestry" appear at 10-100x higher rates in AI text vs human corpora.
