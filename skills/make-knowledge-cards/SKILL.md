---
name: make-knowledge-cards
description: Turn a user-provided article or local Markdown/TXT file into a small set of focused, source-faithful knowledge cards. Use when the user wants important ideas extracted for learning or review.
---

# Make Knowledge Cards

Convert only the content the user provided into 5–8 useful knowledge cards when the source supports that many distinct ideas. If it supports fewer, return fewer and briefly say why; never pad the set. Aim for the most important reusable concepts, not a summary of every paragraph.

## Input

- Accept text pasted by the user or a local `.md`, `.markdown`, or `.txt` file the user identifies. Read only that file as the source.
- Do not fetch webpages, follow links, process PDFs, create Anki decks, or use a graphical interface. If asked for one of these, state the limitation and offer pasted text or a supported local text file instead.
- Ignore navigation, boilerplate, repeated claims, and other material that contributes no distinct knowledge.

## Select and write cards

1. Identify the source's central claims, definitions, mechanisms, distinctions, procedures, and concrete lessons. Rank by importance to understanding or applying the article.
2. Merge duplicate or substantially overlapping points. Keep each card focused on exactly one knowledge point; split a point only when its parts can be understood independently.
3. Keep every claim grounded in the source. Do not add outside facts, invented examples, assumed context, or conclusions stronger than the text. Preserve qualifiers and uncertainty. If the source is ambiguous, keep the wording appropriately cautious.
4. Explain the idea briefly in plain language. Reuse an example from the source when it helps; otherwise provide a short self-test question whose answer is supported by the source. Do not invent an illustrative example and present it as source content.
5. Prefer 5–8 cards, but let source coverage determine the actual count. A short or repetitive source may warrant fewer. Mention briefly when fewer than five distinct, well-supported points are available.

## Output

Start with a concise source title if one is apparent; otherwise use `知识卡片`. Number the cards. Use this shape for each:

### 1. [标题]
- **核心知识：** [one knowledge point]
- **简明解释：** [short explanation grounded in the source]
- **例子或自测：** [source example, or one answerable self-test question]

Keep the full response concise. Do not add a separate broad summary unless the user asks for one.
