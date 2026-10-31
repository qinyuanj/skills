---
name: read-a-book
description: "Reads a book or long text at Adler's levels: inspectional, analytical, syntopical. Use when asked to 精读 or 拆书 a book, judge whether a book is worth reading, or compare several books on one subject. Not for fetching URLs (read) or multi-source research write-ups (learn)."
when_to_use: "精读, 拆书, 读这本书, 这本书讲什么, 值不值得读, 主题阅读, 几本书对比, read this book, analytical reading, syntopical reading"
---

# Read a Book

Mortimer Adler's _How to Read a Book_, run by an agent. Reading is active: the reader asks the book questions and answers them in writing. Four questions drive every level:

1. What is the book about as a whole?
2. What is being said in detail, and how?
3. Is it true, in whole or part?
4. What of it?

## Ground rule: the text, not your memory

Anchor every claim about the book to a **location** (chapter, section, page) in the text the user supplied. Famous books tempt you to answer from pretraining; the source text is the only authority here. When only a title is available, ask for the text, or proceed with every output labelled _from memory, unverified_.

Long books exceed context: read chapter by chapter and write findings to the notes file as you go, so later stages read your notes rather than the whole book again.

## Choose the level

Infer from the request:

- **Inspectional**: "what is this book", "worth reading?", or a stack of candidates. Stop after inspection.
- **Analytical**: 精读, 拆书, "really understand this book". Inspection first, then [`ANALYTICAL.md`](ANALYTICAL.md).
- **Syntopical**: several books on one subject, "compare what X and Y say about Z". Inspect every book, then [`SYNTOPICAL.md`](SYNTOPICAL.md).

Every level starts with inspection.

## Inspectional reading

Two passes, each bounded so it stays fast.

**Systematic skim** (minutes, not hours):

1. Title, subtitle, preface: the author's own statement of aim.
2. Table of contents: the skeleton.
3. Index: the recurring terms, and which ones carry the most page references.
4. Blurb and introduction: the claimed contribution.
5. The pivotal chapters the contents point to: read their opening and closing paragraphs.
6. Dip in: a paragraph or two at scattered points, and the last few pages.

**Superficial read**: one straight pass through, keeping moving past whatever is hard. Mark the hard spots for later; understanding half the book now beats understanding none of it by stalling on page 30.

Inspection is done when you can write all four:

- **Kind**: practical (how to act) or theoretical (what is the case); its field; fiction or exposition.
- **Unity**: what the whole book is about, in one or two sentences.
- **Skeleton**: the major parts in order, one line each.
- **Verdict**: worth an analytical reading or not, and why, in one sentence.

## Output

Write in the user's language. When the user wants a note saved, follow the target repo's conventions (frontmatter, folder, link style); otherwise reply inline with the inspection record, plus the analytical or syntopical record when that level ran.
