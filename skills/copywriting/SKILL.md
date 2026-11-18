---
name: copywriting
description: >-
  Write or edit text that people will read, in any language: articles, posts, emails, messages, announcements, presentations, web pages, UI microcopy, documentation prose. Use when drafting, rewriting, shortening or reviewing copy for a reader, and when text reads as AI-written, wordy, punchy or hard to follow. Not for fiction, or for prompts and instructions written for agents.
---

# Copywriting

The reader has only the page. They were absent from this conversation, they have other things to do, and they stop reading when the text stops helping them. Give this reader what they need, in the order they need it, in plain words, and stop.

> Vigorous writing is concise. A sentence should contain no unnecessary words, a paragraph no unnecessary sentences, for the same reason that a drawing should have no unnecessary lines and a machine no unnecessary parts. This requires not that the writer make all sentences short or avoid all detail and treat subjects only in outline, but that every word tell.
>
> William Strunk Jr., *The Elements of Style*

Work through the steps in order. For one line of copy they take a few seconds of thought. For an article they are most of the work.

## 1. Know the reader

Answer these before writing a sentence:

- **Who** reads this, and **where** do they meet it: an inbox between meetings, a button in the middle of a task, a slide in a meeting room?
- What do they **already know** about the subject?
- What do they **need to know, decide or do** once they have read it?

Then write the **point**: the one sentence this reader must take away, in words they would use.

Take the answers from the user's request and the material. When an answer is missing and the text would change with it, ask the user one question. Otherwise choose the likeliest answer and tell the user which you chose.

Done when the point fits in one sentence. If it takes more, the text has two subjects or the thinking is unfinished; settle that first.

## 2. Separate your context from the reader's

You know things from this conversation that the reader has never seen: the files, the earlier drafts, the decisions, the labels coined along the way, the user's request. Treat all of it as invisible to them. For each thing the text mentions, either put what the reader needs to follow it on the page, or leave the thing out.

Check these in particular:

- **Names and abbreviations** that first appeared in this conversation or inside the user's team. Write out what they stand for, or describe the thing.
- **Pointers** such as "the new version", "this approach", "as discussed". Put what they point to on the page.
- **Comparisons with a state the reader never saw**: "simplified", "updated", "now faster". Describe how things are.
- **Who "we" and "you" are**, and dates given as "yesterday" or "next week".
- **The story of how the work or the text came about.** Include it only when the reader needs it for the point.

Every sentence in the copy is about the subject and addressed to the reader. Remarks about the request, the drafting or the text itself go in your note to the user (step 7).

## 3. Choose the content and its order

Read the reference for the format now (see [Formats](#formats)).

- Put the point first, or as near the start as the format allows.
- Add what this reader needs in order to understand the point, trust it and act on it. Rank by their need. The effort it took to find something gives it no claim to a place.
- After each part, ask what this reader would ask next. Answer that, or end.
- Leave the rest out, including facts that are true and interesting.

The length is whatever this leaves.

## 4. Write plain statements

- **Say the thing itself.** State what something is, what happened, what to do. A sentence earns its place by carrying information the reader needs. When a sentence only prepares for the next one, announces it or comments on the last one, keep the other sentence and delete this one.
- **Use the positive form.** Say what is the case. Bring in a contrast only when this reader holds the other view, and then give the true statement first.
- **Be specific.** Name who does what. Give the number, the name or the example in place of the general claim. Use only specifics you have; an invented detail is an error. When the text cannot do its job without a fact you lack, such as the price on a pricing page, ask the user or mark the place as `[NEED: what is missing]`. Any other open question goes in your note, and the copy stays ready to use.
- **Keep the tone level.** Explain as you would to a capable colleague across a table. Emphasis works when it is rare, so let most sentences simply inform. The facts show what matters.
- **Use one term per thing**, from the first mention to the last.
- **Write in the reader's language from the first draft.** Compose in it directly and follow its own idiom, punctuation and forms of address. These steps describe what a sentence does for the reader. Apply them to that, whatever the words are.
- **Format for the destination.** Use only what renders where the text is going. Lists hold parallel items, numbered steps hold a sequence, tables hold comparisons, prose holds reasoning.
- **Write for the reader who scans.** Most readers scroll through a page before they read it, and their eye stops at headings, tables, figures, lists and bold text. Each of these has to make sense to someone who has read nothing around it. A column header says what its cells contain and in which unit. A number says what it counts. A heading says what its section tells. A caption or label names what a quote, picture or example shows.

## 5. Cut

Read the draft as the reader from step 1. For each sentence ask whether this reader would miss it, and delete the ones they would not. Then ask the same of each word.

Then read [references/habits.md](references/habits.md) and revise for the habits it describes. Read it before the first pass when you are editing a text someone gave you.

Stop where the next cut would cost the reader something. Keep the articles, connecting words and definitions that make a sentence easy to read: a text without them is shorter and takes longer to understand.

## 6. Get a cold read

You know too much to read your own draft as the reader will, so have it read by someone who knows nothing. Do this for any text the reader will meet without you there to explain it, when it is longer than a short message or when a misreading would be costly. For anything smaller, reread it once yourself as the reader and go to step 7.

1. Start one subagent that has none of this conversation. In Claude Code, name the `agent-copywriting:cold-reader` agent; a fork of yourself carries your context and cannot do this job. On other hosts, spawn one new subagent and tell it to work only from what you send.
2. Send it three things and nothing else: the brief in [references/cold-read.md](references/cold-read.md) (its full path, or its full text), the who-and-where line from step 1, and the draft. Keep the point, the request and your reasoning to yourself, so that its report shows what the page alone conveys.
3. Compare its report with step 1 and change the text:
   - Its takeaway differs from your point: the point is missing, late or unclear. Restructure.
   - It stumbled somewhere: rewrite that place so the page answers the question it had.
   - It could have skipped a passage: cut the passage.
   - It asked for something: add it if this reader needs it for the point and you have the answer. If you lack the answer, pass the question to the user in your note.
4. After a restructure, get a second cold read from a new subagent, since the first has now seen the old draft. Two rounds are enough. Tell the user about anything still open.

On a host without subagents, set the draft aside, then follow the brief yourself from the first line, using only what is on the page.

## 7. Hand over

Give the user the copy on its own, in a file or a block, ready to use. Keep your note about it outside the copy and short: the reader you assumed, the gaps that need their facts, and anything from the cold read you left open. The user is the reader of that note, and steps 1 to 5 apply to it.

## Editing someone else's text

Their claims, their degree of certainty, their conditions and their voice stay as they are. Voice is their vocabulary, their register and their opinions. The habits in [references/habits.md](references/habits.md) are separate from voice, so revise them as you would in your own draft. Your edits remove what the reader can do without and clarify what remains. Where the substance itself looks wrong or unsupported, say so in your note and leave the meaning of the text alone.

When the user asks for a review only, run step 6 and report what the reader experienced, with the changes you would make. Rewrite when they ask.

## Formats

| The text is | Read |
| --- | --- |
| An article, post, report or documentation page | [references/article.md](references/article.md) |
| An email, chat message or announcement | [references/email.md](references/email.md) |
| Slides or speaker notes | [references/presentation.md](references/presentation.md) |
| A landing page or product page | [references/web-page.md](references/web-page.md) |
| Buttons, labels, errors and other text inside a product | [references/ui-microcopy.md](references/ui-microcopy.md) |

For any other format, apply the steps and take the conventions from good examples of that format in the reader's language.
