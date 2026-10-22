---
name: human-written
description: Rewrite an article, post, or draft so it reads as human-written and not AI-generated. Use when the user asks to humanize, de-AI, or rewrite text so it does not sound like an AI wrote it. Enforces natural rhythm, plain vocabulary, no contractions, minimal em dashes, and removal of known AI structures.
---

# Human-written rewrite

Rewrite the text the user provides so a careful reader would not suspect an AI wrote it. Keep the meaning, the facts, and the line of argument. Change how it sounds.

Before rewriting, read `references/banned-phrases.md`. It holds the word and phrase lists, and the user edits it over time. If the user pastes a sample of their own writing, match its voice. If not, default to a direct, plain, slightly dry voice.

## Core principles

1. **Fix the problem, not the symptom.** Swapping a flagged word for a synonym leaves a vague sentence vague. Make the sentence specific, make it shorter, or delete it.
2. **Do not overcorrect.** Forced "human" tricks are their own tell: a fragment in every paragraph, a rhetorical question every few lines, one-line paragraphs used as drumrolls. Variation should come from the content, not from a quota.
3. **Never invent.** Do not add facts, numbers, names, quotes, anecdotes, or personal experiences that the source does not contain. Specific-sounding invented details (such as "I had 47 tabs open") are a known AI habit.

## Rules

### 1. Rhythm and structure
- Let sentence length follow the thought. Short sentences for blunt points, longer ones for reasoning. Avoid long runs of sentences with the same length and shape.
- Do not chain short punchy lines for effect. Two or three in a row reads as AI as much as uniform length does.
- Vary paragraph length to fit the content. A one-sentence paragraph is fine when it earns it, not as a habit.
- Do not start consecutive sentences or paragraphs the same way ("This", "It", "By [verb]-ing", "Additionally").
- Do not force a template (hook, three points, "In conclusion"). Let the content set the shape.
- Do not end a paragraph or section with a line that restates it. Do not add mid-article recaps ("Overall, ...", "In short, ...").
- Do not make a claim and then restate it in grander words in the next sentence.

### 2. Cut padding and signposting
- Use one word where AI would use three. "In order to" becomes "to". "Due to the fact that" becomes "because".
- Delete sentences that add no information, including throat-clearing openers and recap closers.
- Remove announcements of what is coming: "In this article, we will", "Let us dive in", "Here is why:", "Let us explore".
- Remove stacked hedges ("it is important to note that", "it could potentially be argued that"). Hedge once, where real uncertainty exists.

### 3. Vocabulary
- Apply every entry in `references/banned-phrases.md`.
- Use plain verbs. Write "is", "has", "shows", "uses". Avoid "serves as", "stands as", "boasts", "features", "represents" when a plain verb works.
- Cut reflexive transitions: moreover, furthermore, additionally, notably, consequently. Most sentences need no connector. Use "but", "so", "and", or "also" when one is needed.
- Repeat the clearest noun instead of cycling through synonyms. Calling the same thing "the company", then "the firm", then "the organization", then "the tech giant" is an AI habit (elegant variation). Use a pronoun when the reference is clear.
- Do not stuff one keyword into every sentence either. Restructure so the subject does not need naming each time.

### 4. Tone and stance
- Take a position wherever the source supports one. Do not present every topic as balanced when the source has a clear view.
- Open with the point. No dramatic scene-setting, metaphor openers, or "In today's world" framing.
- No promotional or travel-brochure language ("breathtaking", "must-visit", "rich heritage", "cutting-edge").
- Do not inflate significance. Do not tell the reader that something is important, pivotal, a testament, a turning point, or part of a broader legacy. Show why it matters with a fact from the source, or cut the claim.
- No editorial asides that announce importance ("It is worth noting", "No discussion would be complete without").
- No unearned closing call to action or motivational push ("Take the first step today").
- No manufactured suspense: "The catch?", "The kicker?", "Here is the thing:", "And honestly?", "The truth is".
- No chatbot or letter residue: "Great question", "Certainly", "I hope this helps", "Let me know if", "I hope this finds you well", knowledge-cutoff disclaimers, placeholder text such as "[insert example]".

### 5. Sentence patterns to remove
- **Negative parallelism (contrastive negation):** "It is not just X, it is Y", "not X, but Y", "not only X but also Y", and the two-sentence version ("This is not about X. It is about Y."). State Y directly.
- **Reflexive triplets:** three adjectives, three benefits, three nouns by default. Use the number of items the content actually has.
- **Trailing participle commentary:** "..., highlighting the importance of ...", "..., reflecting broader trends", "..., ensuring ...", "..., underscoring ...". Either explain the link in a full sentence with a fact, or delete the clause.
- **False ranges:** "ranging from X to Y" or "from X to Y" where the endpoints do not define a real scale.
- **Vague attribution:** "experts say", "studies show", "critics argue", "industry reports suggest". Name the source from the text or drop the claim.
- **Rhetorical question answered at once:** "The result? Chaos."
- **Challenges-and-outlook closer:** "Despite these challenges, X continues to thrive" or "The future of X looks bright".
- **Dramatic adverbs as setup:** "quietly", "simply", "truly", "genuinely" used for effect.

### 6. Contractions (hard rule)
- Never use contractions. Always write the full form: I am, I have, I would, I will, should have, could have, would have, do not, does not, did not, cannot, will not, is not, are not, it is, that is, there is, they are, we are, you are, let us.
- Possessives are fine ("the company's revenue"). Only contractions are banned.
- Leave direct quotations from other people unchanged.
- Without contractions the text can turn stiff. Offset that with plain words and natural rhythm, not with slang.

### 7. Formatting and punctuation
- Em dashes: none in most pieces, at most one or two in a long article. Use commas, periods, colons, or parentheses.
- No bold for emphasis except in rare cases. No bolded keywords inside paragraphs.
- No bullets that start with a bold label followed by a sentence that repeats the label ("**Scalability:** The system scales easily.").
- Prefer prose to lists and headers. Keep a list only where the source had one or the content is a real sequence.
- Headings in sentence case. Do not give every heading the same template ("Why does X matter?", "How to get started").
- No emojis unless the source has them. No decorative Unicode such as arrows, check marks, or approximately-equal signs.
- Use straight quotes unless the source uses curly ones.

### 8. Voice and texture
- Prefer concrete over general: a number, a name, a date, an example. Use only specifics that appear in the source. If the source has none, write plainly instead of inventing.
- Fragments and sentences that start with "And" or "But" are allowed. Use them rarely.
- Write in first person only if the source or the user supplies that voice.
- Do not add fake typos or deliberate errors.

## Process

1. Read the full source text first. Note its facts, names, numbers, citations, and main claim.
2. Read `references/banned-phrases.md`.
3. Rewrite. Keep every fact and citation. Add nothing the source does not contain.
4. Match the original length within about 10 percent unless the user asks for a different length. AI rewrites tend to expand, so trimming is usually right.
5. Run the audit below and fix every hit.
6. Read the result once as a skeptical human editor. If any paragraph still sounds generic, cut or rewrite it.
7. Return only the rewritten text, with no preamble. If the user asks what changed, give a short list after the text.

## Final audit

- [ ] No words or phrases from `references/banned-phrases.md`.
- [ ] No contractions outside direct quotations. Scan for apostrophes followed by s, t, m, d, ll, ve, or re, and keep only possessives.
- [ ] Zero to two em dashes.
- [ ] No negative parallelism in any form, including the two-sentence version.
- [ ] No trailing "-ing" commentary clauses.
- [ ] No reflexive triplets.
- [ ] No vague attribution without a named source.
- [ ] No synonym cycling for the same subject.
- [ ] No run of three or more short punchy lines.
- [ ] No two consecutive paragraphs that open the same way.
- [ ] No closing recap, outlook paragraph, or call to action that the source did not have.
- [ ] No bold-label bullets, emojis, or decorative Unicode.
- [ ] Every fact, name, and number matches the source, and nothing new was added.
